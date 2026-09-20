---
name: thehiveryiq-com-free-receipt-sign-and-verify
description: Sign any string with a free, unauthenticated dual-signed Hive receipt, then verify it offline-capably
  against the published key.
api: openapi/thehiveryiq-com-hivemorph-openapi.yml
base_url: https://receipts.thehiveryiq.com
operations:
- issue_free_receipt_v1_receipt_free_post
- get_receipt_v1_receipt__receipt_id__get
- verify_receipt_route_v1_receipt_verify_post
- prov_pubkey_v1_prov_pubkey_get
generated: '2026-09-19'
method: generated
grounding: every operationId below was checked against the served contract; nothing was invented
---

# Sign and verify a free Hive receipt

Use this when an agent needs a tamper-evident, timestamped record of a payload (a decision, a log line, a diff, a contract clause) and does not need a paid receipt profile.

## Rules that apply to every step
- No credential. The free tier is anonymous and limited to **100 receipts per IP per UTC day**; on exhaustion the API returns **429** (no Retry-After header; read `free_tier.remaining_today` from each 201 body and stop before it reaches 0).
- Every call mints a **new** `receipt_id`. A retried POST is a second receipt, not a replay: this write is not idempotent (see conventions/).
- Send **public or synthetic text only**. The provider states the payload reaches the service in readable form.
- Receipts are append-only; there is no delete, void or amend.

## Steps
1. `issue_free_receipt_v1_receipt_free_post` — `POST /v1/receipt/free` with `{"payload": "<string, max 8192 chars>", "label": "<optional, max 120>"}`. Expect **201** with `receipt_id`, `payload_hash`, `verify_url`, `verify_api`, `signatures.classical` (Ed25519, RFC 8032) and `signatures.pq` (ML-DSA-65, FIPS 204), and `free_tier.remaining_today`.
2. `get_receipt_v1_receipt__receipt_id__get` — `GET /v1/receipt/{receipt_id}` to re-read the stored envelope later (404 `{"detail":"Not Found"}` if unknown).
3. `prov_pubkey_v1_prov_pubkey_get` — `GET /v1/prov/pubkey` once, cache the Ed25519 key (`issuer did:hive:hivemorph`, also in `/trust.json` with epoch and rotation policy) so verification does not depend on the API being up.
4. `verify_receipt_route_v1_receipt_verify_post` — `POST /v1/receipt/verify` with `{"envelope": <the envelope object from step 1>}`. A `400 {"detail":"receipt_id, payload_sha256, sig_b64u, ts are required"}` means you sent the classical-verify shape without those fields; a `422` means a malformed body (`detail[].loc` names the field).

## Errors to handle
- 429 quota exhausted (free tier) → wait for UTC rollover or move to the paid skill.
- 422 validation → fix the field named in `detail[0].loc`.
- The `verify_url` points at the browser verifier on thehiveryiq.com; `verify_api` is the machine path.
