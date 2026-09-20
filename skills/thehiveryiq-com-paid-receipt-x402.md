---
name: thehiveryiq-com-paid-receipt-x402
description: Price, pay for (x402 on Base) and emit a Hive receipt at the nano, standard or pq profile, then verify
  it.
api: openapi/thehiveryiq-com-hivemorph-openapi.yml
base_url: https://receipts.thehiveryiq.com
operations:
- get_pricing_v1_x402_pricing_get
- get_rails_v1_x402_rails_get
- rubric_select_v1_rubric_select_post
- quote_v1_x402_quote_post
- receipt_emit_preflight_v1_receipt_emit_get
- receipt_emit_v1_receipt_emit_post
- submit_proof_v1_x402_proof_submit_post
- verify_token_v1_x402_proof_verify_get
- verify_receipt_route_v1_receipt_verify_post
generated: '2026-09-19'
method: generated
grounding: every operationId below was checked against the served contract; nothing was invented
---

# Emit a paid receipt through the x402 flow

Use this when a receipt must carry a paid profile (`nano` $0.0001, `standard` $0.0008 default, `pq` $0.0012 per call; retention 30 / 365 / 2555 days per `GET /pricing`).

## Rules that apply to every step
- Payment is **on-chain USDC (or USDT) on Base 8453**, scheme `exact`, EIP-3009. It is final: there is no refund operation in the contract. Confirm the amount before paying.
- A 402 nonce has an `expires_at`; the access token returned after proof lasts **5 minutes** and is bound to the **same path**.
- Emit is not idempotent: retrying after a timeout may mint and charge twice. Persist `receipt_id` from any 200 you receive before retrying.
- The `hive-rosetta` SDK (npm/PyPI 0.1.0) implements the 402 → sign → retry loop if you would rather not hand-roll it.

## Steps
1. `get_pricing_v1_x402_pricing_get` — `GET /v1/x402/pricing` (free) and `get_rails_v1_x402_rails_get` — `GET /v1/x402/rails` (free) to read the current per-path prices and the accepted chain/asset pairs and treasury address.
2. Optional: `rubric_select_v1_rubric_select_post` — `POST /v1/rubric/select` with `{"intent": "...", "amount_usd": <n>}` to get `recommended_profile` (nano | standard | pq).
3. `quote_v1_x402_quote_post` — `POST /v1/x402/quote` with `{"receipt_profile": "standard", "agent_did": "did:hive:<you>", "amount_usdc": <optional>}` (free). Returns `amount_usdc`, `treasury`, `asset_address`, `hktn_discount_pct` and an ERC-681 `deeplink_erc681`.
4. `receipt_emit_preflight_v1_receipt_emit_get` — `GET /v1/receipt/emit?profile=standard` to check the path is live for that profile without paying.
5. `receipt_emit_v1_receipt_emit_post` — `POST /v1/receipt/emit?profile=standard` with `{"agent_did": "did:hive:<you>", "artifact": "<string or hash>", "artifact_type": "text/plain", "metadata": {}}`. Unpaid, this returns **402** with `x-payment-required: true` and a body `payment` object (`nonce`, `amount_usd`, `accepts[]`, `payment_endpoint`).
6. Pay per `accepts[]` (EIP-3009 `transferWithAuthorization` to `recipient` for `amount_atomic`), then either retry step 5 with the proof in an `X-Payment` header, or `submit_proof_v1_x402_proof_submit_post` — `POST /v1/x402/proof/submit` with the nonce and proof to receive an access token, and retry step 5 with `X-Hive-Access: <token>` within 5 minutes.
7. `verify_token_v1_x402_proof_verify_get` — `GET /v1/x402/proof/verify` if you need to check a token before reuse.
8. `verify_receipt_route_v1_receipt_verify_post` — `POST /v1/receipt/verify` with `{"envelope": <returned envelope>}` to confirm the signature before storing the receipt.

## Errors to handle
- 402 after paying → nonce expired or wrong path; re-quote.
- 422 → body validation (`agent_did` and `artifact` are required).
- The `pq` profile is "gated by regulated-tier delegation" (`regulated_envelope_jti`): obtain a delegation first (see the delegation skill).
