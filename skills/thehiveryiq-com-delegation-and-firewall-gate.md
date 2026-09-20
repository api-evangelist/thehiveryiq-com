---
name: thehiveryiq-com-delegation-and-firewall-gate
description: Issue a scoped delegation for an agent, dry-run it against the firewall, check it before acting, and
  revoke it.
api: openapi/thehiveryiq-com-hivemorph-openapi.yml
base_url: https://receipts.thehiveryiq.com
operations:
- hktn_lookup_v1_hktn_lookup_get
- issue_v1_delegation_issue_post
- verify_v1_delegation_verify_post
- enforce_preview_v1_firewall_enforce_preview_post
- sandbox_run_v1_firewall_sandbox_run_post
- delegation_check_v1_delegation_check_post
- revoke_v1_delegation_revoke__jti__post
generated: '2026-09-19'
method: generated
grounding: every operationId below was checked against the served contract; nothing was invented
---

# Gate an agent's actions with a Hive delegation

Use this when one party (an operator) must bound what an agent may do (spend cap, allowed actions/endpoints/counterparties/jurisdictions, proof tier, TTL) and later prove that each action was checked.

## Rules that apply to every step
- Delegation issue, verify, check and revoke are all **free** and need no credential (per the operation descriptions and /agents).
- A delegation is identified by `jti`. Revocation is immediate and has **no stated undo window**: after revoke, `verify` returns `verified:false` with `reasons` including `revoked`.
- Use `enforce/preview` and `sandbox/run` before anything that settles: both record nothing on any settlement layer.

## Steps
1. `hktn_lookup_v1_hktn_lookup_get` — `GET /v1/hktn/lookup?agent_did=did:hive:<agent>` to read the counterparty's trust tier (Cold / Warm / Hot / Regulated) before deciding the caps.
2. `issue_v1_delegation_issue_post` — `POST /v1/delegation/issue` with `{"agent_id": "<agent>", "operator_did": "did:hive:<you>", "allowed_actions": [...], "max_spend_usdc": <n>, "allowed_endpoints": [...], "allowed_counterparties": [...], "allowed_jurisdictions": [...], "max_proof_tier": "standard", "ttl_seconds": <n>}`. Only `agent_id` is required. Store the returned envelope and its `jti`.
3. `verify_v1_delegation_verify_post` — `POST /v1/delegation/verify` with the envelope to confirm signature and TTL.
4. `enforce_preview_v1_firewall_enforce_preview_post` — `POST /v1/firewall/enforce/preview` with `{"jti": "<jti>", "request": {...the action you intend...}}` for a dry-run decision.
5. `sandbox_run_v1_firewall_sandbox_run_post` — `POST /v1/firewall/sandbox/run` to exercise the same request end-to-end with a synthetic result and no settlement.
6. Before each real action: `delegation_check_v1_delegation_check_post` — `POST /v1/delegation/check` with `{"jti": "<jti>", "request": {...}}` (single call: envelope verification + firewall decision + `next_best_actions`).
7. When done or compromised: `revoke_v1_delegation_revoke__jti__post` — `POST /v1/delegation/revoke/{jti}`.

## Errors to handle
- 422 → `detail[].loc` names the offending field.
- `verified:false` with `reasons` → read the reasons (expired, revoked, scope) rather than retrying.
