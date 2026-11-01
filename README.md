# Hive Civilization

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Hive Civilization (DBAs The Hivery and The Hivery IQ; Walnut Creek, California; single-founder Wyoming corporation established 2026) sells signed, independently verifiable receipts for automated and AI-agent actions: every call returns a dual-signed record (Ed25519 plus ML-DSA-65) over an artifact hash, priced per receipt and settled per call in USDC on Base through the x402 payment protocol, with no account required for the free tier. The public surface is spread over four hosts: receipts.thehiveryiq.com serves the HiveMorph receipts and agent-commerce API (a 906-path, 937-operation FastAPI OpenAPI 3.1 contract covering receipt emit/verify, x402 quotes and settlement references, delegations and a firewall, HKTN trust lookups, plus dozens of vertical attestation families), a JSON-RPC 2.0 agent endpoint and A2A agent cards; api.thehiveryiq.com serves HiveCompute, an OpenAI-compatible, x402-metered inference router with a live remote MCP server; passport.thehiveryiq.com is the HKTN trust rail; and hive-mcp-gateway.onrender.com fronts 37 hive-mcp-* MCP servers. The apex publishes an A2A agent card, security.txt, llms.txt, pricing, a self-attested (uncertified) SOC 2 / ISO 27001 posture and a did:hive DID method specification.

**Areas:** Agents · Agentic Commerce · A2A · MCP · x402 · Receipts · Digital Signature · Post-Quantum Cryptography · Attestation · Decentralized Identity · Stablecoins · Inference

## Hive Civilization on APIs.io

Everything profiled for Hive Civilization is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/thehiveryiq-com/](https://apis.io/providers/thehiveryiq-com/)** — or go straight to one of the APIs or properties below.

### APIs (153)

- [Hive MCP Gateway and Registry](https://apis.io/apis/thehiveryiq-com/hive-mcp-gateway/) — Provider-operated remote MCP gateway on Render (named as the MCP transport by receipts.thehiveryiq.com/.well-known/mcp.json): initialize and tools/list…
- [Hive Passport Trust Rail (HKTN)](https://apis.io/apis/thehiveryiq-com/hive-passport-trust-rail/) — The trust rail on passport.thehiveryiq.com: HKTN (Hive Known Traveler Number) registry for persistent agent identity and tier, tenant onboarding and…
- [Hive Civilization A2A Agent](https://apis.io/apis/thehiveryiq-com/hive-a2a-agent/) — Agent-to-agent surface: A2A agent cards on the apex (protocolVersion 0.3.0, six HiveAttest/HiveWallet/HiveGate skills) and on receipts.thehiveryiq.com…
- [Hive Civilization A2a API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-a2a-api/) — The a2a API from Hive Civilization — 9 operation(s) for a2a.
- [Hive Civilization Activation API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-activation-api/) — The activation API from Hive Civilization — 3 operation(s) for activation.
- [Hive Civilization Aegis API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-aegis-api/) — The aegis API from Hive Civilization — 6 operation(s) for aegis.
- [Hive Civilization Affordances API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-affordances-api/) — The affordances API from Hive Civilization — 28 operation(s) for affordances.
- [Hive Civilization Afir Stream API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-afir-stream-api/) — The afir-stream API from Hive Civilization — 10 operation(s) for afir-stream.
- [Hive Civilization Agent Receipts API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-agent-receipts-api/) — The agent-receipts API from Hive Civilization — 4 operation(s) for agent-receipts.
- [Hive Civilization Alcoa Agentguard API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-alcoa-agentguard-api/) — The alcoa-agentguard API from Hive Civilization — 11 operation(s) for alcoa-agentguard.
- [Hive Civilization Amplify API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-amplify-api/) — The amplify API from Hive Civilization — 9 operation(s) for amplify.
- [Hive Civilization App Kits API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-app-kits-api/) — The app-kits API from Hive Civilization — 6 operation(s) for app-kits.
- [Hive Civilization Arb Alloc API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-arb-alloc-api/) — The arb-alloc API from Hive Civilization — 4 operation(s) for arb-alloc.
- [Hive Civilization Arb Compute API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-arb-compute-api/) — The arb-compute API from Hive Civilization — 3 operation(s) for arb-compute.
- [Hive Civilization Arb Spread API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-arb-spread-api/) — The arb-spread API from Hive Civilization — 5 operation(s) for arb-spread.
- [Hive Civilization Aris Agent Asset API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-aris-agent-asset-api/) — The aris-agent-asset API from Hive Civilization — 6 operation(s) for aris-agent-asset.
- [Hive Civilization Attest API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-attest-api/) — The attest API from Hive Civilization — 20 operation(s) for attest.
- [Hive Civilization Audit API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-audit-api/) — The audit API from Hive Civilization — 1 operation(s) for audit.
- [Hive Civilization Basis Perp API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-basis-perp-api/) — The basis-perp API from Hive Civilization — 12 operation(s) for basis-perp.
- [Hive Civilization Billing API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-billing-api/) — The billing API from Hive Civilization — 4 operation(s) for billing.
- [Hive Civilization Billing Meter API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-billing-meter-api/) — The billing-meter API from Hive Civilization — 6 operation(s) for billing-meter.
- [Hive Civilization Bounty API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-bounty-api/) — The bounty API from Hive Civilization — 14 operation(s) for bounty.
- [Hive Civilization Capitolare API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-capitolare-api/) — The capitolare API from Hive Civilization — 13 operation(s) for capitolare.
- [Hive Civilization Chat API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-chat-api/) — The chat API from Hive Civilization — 2 operation(s) for chat.
- [Hive Civilization Clear API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-clear-api/) — The Clear API from Hive Civilization — 12 operation(s) for clear.
- [Hive Civilization Clear MCP API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-clear-mcp-api/) — The clear-mcp API from Hive Civilization — 1 operation(s) for clear-mcp.
- [Hive Civilization Cns API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-cns-api/) — The cns API from Hive Civilization — 4 operation(s) for cns.
- [Hive Civilization Compliance API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-compliance-api/) — The compliance API from Hive Civilization — 1 operation(s) for compliance.
- [Hive Civilization Compound Chains API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-compound-chains-api/) — The compound-chains API from Hive Civilization — 5 operation(s) for compound-chains.
- [Hive Civilization Compute API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-compute-api/) — The Compute API from Hive Civilization — 5 operation(s) for compute.
- [Hive Civilization Compute Grid API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-compute-grid-api/) — The compute-grid API from Hive Civilization — 11 operation(s) for compute-grid.
- [Hive Civilization Cre API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-cre-api/) — The cre API from Hive Civilization — 11 operation(s) for cre.
- [Hive Civilization Dashboard API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-dashboard-api/) — The dashboard API from Hive Civilization — 5 operation(s) for dashboard.
- [Hive Civilization Deedlock API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-deedlock-api/) — The Deedlock API from Hive Civilization — 13 operation(s) for deedlock.
- [Hive Civilization Desci Qvac API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-desci-qvac-api/) — The desci-qvac API from Hive Civilization — 7 operation(s) for desci-qvac.
- [Hive Civilization Designer API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-designer-api/) — The designer API from Hive Civilization — 7 operation(s) for designer.
- [Hive Civilization Discovery API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-discovery-api/) — The discovery API from Hive Civilization — 5 operation(s) for discovery.
- [Hive Civilization Dispute Observer API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-dispute-observer-api/) — The dispute-observer API from Hive Civilization — 5 operation(s) for dispute-observer.
- [Hive Civilization Distribution API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-distribution-api/) — The distribution API from Hive Civilization — 5 operation(s) for distribution.
- [Hive Civilization Earn API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-earn-api/) — The earn API from Hive Civilization — 8 operation(s) for earn.
- [Hive Civilization Echo API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-echo-api/) — The echo API from Hive Civilization — 2 operation(s) for echo.
- [Hive Civilization Edi API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-edi-api/) — The Edi API from Hive Civilization — 6 operation(s) for edi.
- [Hive Civilization Entropy API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-entropy-api/) — The entropy API from Hive Civilization — 4 operation(s) for entropy.
- [Hive Civilization Evaluator API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-evaluator-api/) — The evaluator API from Hive Civilization — 11 operation(s) for evaluator.
- [Hive Civilization Evidence API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-evidence-api/) — The Evidence API from Hive Civilization — 1 operation(s) for evidence.
- [Hive Civilization Favicon.ico API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-favicon-ico-api/) — The Favicon.ico API from Hive Civilization — 1 operation(s) for favicon.ico.
- [Hive Civilization Fleet API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-fleet-api/) — The fleet API from Hive Civilization — 12 operation(s) for fleet.
- [Hive Civilization Forge API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-forge-api/) — The forge API from Hive Civilization — 6 operation(s) for forge.
- [Hive Civilization Github App API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-github-app-api/) — The github-app API from Hive Civilization — 3 operation(s) for github-app.
- [Hive Civilization Governance API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-governance-api/) — The governance API from Hive Civilization — 9 operation(s) for governance.
- [Hive Civilization Guardian API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-guardian-api/) — The guardian API from Hive Civilization — 4 operation(s) for guardian.
- [Hive Civilization Health API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-health-api/) — The Health API from Hive Civilization — 1 operation(s) for health.
- [Hive Civilization Health Badge API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-health-badge-api/) — The health-badge API from Hive Civilization — 1 operation(s) for health-badge.
- [Hive Civilization Hipaa Hive API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-hipaa-hive-api/) — The hipaa-hive API from Hive Civilization — 11 operation(s) for hipaa-hive.
- [Hive Civilization Hive Agent Listings API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-hive-agent-listings-api/) — The hive-agent-listings API from Hive Civilization — 3 operation(s) for hive-agent-listings.
- [Hive Civilization Hive Mark API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-hive-mark-api/) — The hive-mark API from Hive Civilization — 5 operation(s) for hive-mark.
- [Hive Civilization Hive Origin API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-hive-origin-api/) — The hive-origin API from Hive Civilization — 5 operation(s) for hive-origin.
- [Hive Civilization Hive Prior API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-hive-prior-api/) — The hive-prior API from Hive Civilization — 6 operation(s) for hive-prior.
- [Hive Civilization Hive Wallet API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-hive-wallet-api/) — The hive-wallet API from Hive Civilization — 4 operation(s) for hive-wallet.
- [Hive Civilization Hivecomply API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-hivecomply-api/) — The hivecomply API from Hive Civilization — 8 operation(s) for hivecomply.
- [Hive Civilization Hivecomply MCP API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-hivecomply-mcp-api/) — The hivecomply-mcp API from Hive Civilization — 1 operation(s) for hivecomply-mcp.
- [Hive Civilization HiveMorph V0.1 API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-hivemorph-v0-1-api/) — The HiveMorph V0.1 API from Hive Civilization — 1 operation(s) for hivemorph v0.1.
- [Hive Civilization Insights API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-insights-api/) — The insights API from Hive Civilization — 1 operation(s) for insights.
- [Hive Civilization Insurance API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-insurance-api/) — The insurance API from Hive Civilization — 9 operation(s) for insurance.
- [Hive Civilization Insurance Broker API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-insurance-broker-api/) — The insurance-broker API from Hive Civilization — 3 operation(s) for insurance-broker.
- [Hive Civilization Kimi API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-kimi-api/) — The kimi API from Hive Civilization — 5 operation(s) for kimi.
- [Hive Civilization Law API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-law-api/) — The law API from Hive Civilization — 18 operation(s) for law.
- [Hive Civilization Lex Contract API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-lex-contract-api/) — The lex-contract API from Hive Civilization — 11 operation(s) for lex-contract.
- [Hive Civilization Llms.txt API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-llms-txt-api/) — The Llms.txt API from Hive Civilization — 1 operation(s) for llms.txt.
- [Hive Civilization Mark API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-mark-api/) — The Mark API from Hive Civilization — 1 operation(s) for mark.
- [Hive Civilization Marketplace Bus API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-marketplace-bus-api/) — The marketplace-bus API from Hive Civilization — 6 operation(s) for marketplace-bus.
- [Hive Civilization MCP API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-mcp-api/) — The Mcp API from Hive Civilization — 5 operation(s) for mcp.
- [Hive Civilization Media Origin API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-media-origin-api/) — The media-origin API from Hive Civilization — 8 operation(s) for media-origin.
- [Hive Civilization Membrane API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-membrane-api/) — The membrane API from Hive Civilization — 2 operation(s) for membrane.
- [Hive Civilization Mining API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-mining-api/) — The mining API from Hive Civilization — 8 operation(s) for mining.
- [Hive Civilization Mining Orchestrate API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-mining-orchestrate-api/) — The mining-orchestrate API from Hive Civilization — 6 operation(s) for mining-orchestrate.
- [Hive Civilization Model Receipts API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-model-receipts-api/) — The model-receipts API from Hive Civilization — 7 operation(s) for model-receipts.
- [Hive Civilization Morph API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-morph-api/) — The Morph API from Hive Civilization — 25 operation(s) for morph.
- [Hive Civilization Morso API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-morso-api/) — The morso API from Hive Civilization — 6 operation(s) for morso.
- [Hive Civilization Mos Energy Arb API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-mos-energy-arb-api/) — The mos-energy-arb API from Hive Civilization — 3 operation(s) for mos-energy-arb.
- [Hive Civilization Mos Intel API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-mos-intel-api/) — The mos-intel API from Hive Civilization — 5 operation(s) for mos-intel.
- [Hive Civilization Mpp API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-mpp-api/) — The mpp API from Hive Civilization — 4 operation(s) for mpp.
- [Hive Civilization Nanopay API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-nanopay-api/) — The nanopay API from Hive Civilization — 4 operation(s) for nanopay.
- [Hive Civilization Nanoverse API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-nanoverse-api/) — The nanoverse API from Hive Civilization — 21 operation(s) for nanoverse.
- [Hive Civilization Newsshield API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-newsshield-api/) — The newsshield API from Hive Civilization — 11 operation(s) for newsshield.
- [Hive Civilization Newsshield MCP API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-newsshield-mcp-api/) — The newsshield-mcp API from Hive Civilization — 1 operation(s) for newsshield-mcp.
- [Hive Civilization Og API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-og-api/) — The Og API from Hive Civilization — 1 operation(s) for og.
- [Hive Civilization Onboard API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-onboard-api/) — The onboard API from Hive Civilization — 2 operation(s) for onboard.
- [Hive Civilization Ops API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-ops-api/) — The ops API from Hive Civilization — 6 operation(s) for ops.
- [Hive Civilization Organic API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-organic-api/) — The organic API from Hive Civilization — 9 operation(s) for organic.
- [Hive Civilization Origin API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-origin-api/) — The Origin API from Hive Civilization — 1 operation(s) for origin.
- [Hive Civilization Pilot API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-pilot-api/) — The pilot API from Hive Civilization — 3 operation(s) for pilot.
- [Hive Civilization Portal API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-portal-api/) — The portal API from Hive Civilization — 4 operation(s) for portal.
- [Hive Civilization Portal Spin API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-portal-spin-api/) — The portal-spin API from Hive Civilization — 8 operation(s) for portal-spin.
- [Hive Civilization Portal V2 API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-portal-v2-api/) — The portal-v2 API from Hive Civilization — 5 operation(s) for portal-v2.
- [Hive Civilization Pq API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-pq-api/) — The pq API from Hive Civilization — 4 operation(s) for pq.
- [Hive Civilization Pricing API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-pricing-api/) — The Pricing API from Hive Civilization — 1 operation(s) for pricing.
- [Hive Civilization Pricing.json API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-pricing-json-api/) — The Pricing.json API from Hive Civilization — 1 operation(s) for pricing.json.
- [Hive Civilization Prior API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-prior-api/) — The Prior API from Hive Civilization — 1 operation(s) for prior.
- [Hive Civilization Procurelock API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-procurelock-api/) — The Procurelock API from Hive Civilization — 11 operation(s) for procurelock.
- [Hive Civilization Protected Flow API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-protected-flow-api/) — The protected-flow API from Hive Civilization — 3 operation(s) for protected-flow.
- [Hive Civilization Prov API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-prov-api/) — The prov API from Hive Civilization — 2 operation(s) for prov.
- [Hive Civilization Provebirth API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-provebirth-api/) — The provebirth API from Hive Civilization — 10 operation(s) for provebirth.
- [Hive Civilization Purity API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-purity-api/) — The purity API from Hive Civilization — 3 operation(s) for purity.
- [Hive Civilization Qvac API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-qvac-api/) — The qvac API from Hive Civilization — 11 operation(s) for qvac.
- [Hive Civilization R10 Rvc API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-r10-rvc-api/) — The r10-rvc API from Hive Civilization — 8 operation(s) for r10-rvc.
- [Hive Civilization R2 Discovery API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-r2-discovery-api/) — The r2-discovery API from Hive Civilization — 6 operation(s) for r2-discovery.
- [Hive Civilization R3 Delegation API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-r3-delegation-api/) — The r3-delegation API from Hive Civilization — 8 operation(s) for r3-delegation.
- [Hive Civilization R3pv API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-r3pv-api/) — The r3pv API from Hive Civilization — 4 operation(s) for r3pv.
- [Hive Civilization R4 Firewall API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-r4-firewall-api/) — The r4-firewall API from Hive Civilization — 9 operation(s) for r4-firewall.
- [Hive Civilization R5 Hktn Reputation API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-r5-hktn-reputation-api/) — The r5-hktn-reputation API from Hive Civilization — 5 operation(s) for r5-hktn-reputation.
- [Hive Civilization R6 Hivememory API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-r6-hivememory-api/) — The r6-hivememory API from Hive Civilization — 6 operation(s) for r6-hivememory.
- [Hive Civilization R7 Spectral API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-r7-spectral-api/) — The r7-spectral API from Hive Civilization — 7 operation(s) for r7-spectral.
- [Hive Civilization R8 Checkpoints API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-r8-checkpoints-api/) — The r8-checkpoints API from Hive Civilization — 7 operation(s) for r8-checkpoints.
- [Hive Civilization R9 Accumulators API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-r9-accumulators-api/) — The r9-accumulators API from Hive Civilization — 8 operation(s) for r9-accumulators.
- [Hive Civilization Receipt API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-receipt-api/) — The Receipt API from Hive Civilization — 1 operation(s) for receipt.
- [Hive Civilization Receipt Ledger API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-receipt-ledger-api/) — The receipt-ledger API from Hive Civilization — 4 operation(s) for receipt-ledger.
- [Hive Civilization Receipt Relay API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-receipt-relay-api/) — The receipt-relay API from Hive Civilization — 4 operation(s) for receipt-relay.
- [Hive Civilization Robots.txt API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-robots-txt-api/) — The Robots.txt API from Hive Civilization — 1 operation(s) for robots.txt.
- [Hive Civilization Runrate API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-runrate-api/) — The runrate API from Hive Civilization — 4 operation(s) for runrate.
- [Hive Civilization Salvage API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-salvage-api/) — The salvage API from Hive Civilization — 23 operation(s) for salvage.
- [Hive Civilization Site Traffic API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-site-traffic-api/) — The site-traffic API from Hive Civilization — 9 operation(s) for site-traffic.
- [Hive Civilization Sitemap.xml API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-sitemap-xml-api/) — The Sitemap.xml API from Hive Civilization — 1 operation(s) for sitemap.xml.
- [Hive Civilization Smsh API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-smsh-api/) — The smsh API from Hive Civilization — 8 operation(s) for smsh.
- [Hive Civilization Smsh Learned API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-smsh-learned-api/) — The smsh-learned API from Hive Civilization — 2 operation(s) for smsh-learned.
- [Hive Civilization Spawn Garage V2 API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-spawn-garage-v2-api/) — The spawn-garage-v2 API from Hive Civilization — 6 operation(s) for spawn-garage-v2.
- [Hive Civilization Sphere API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-sphere-api/) — The Sphere API from Hive Civilization — 1 operation(s) for sphere.
- [Hive Civilization Status.json API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-status-json-api/) — The Status.json API from Hive Civilization — 1 operation(s) for status.json.
- [Hive Civilization Storefront API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-storefront-api/) — The storefront API from Hive Civilization — 3 operation(s) for storefront.
- [Hive Civilization Stormlock API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-stormlock-api/) — The stormlock API from Hive Civilization — 11 operation(s) for stormlock.
- [Hive Civilization Subscription API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-subscription-api/) — The subscription API from Hive Civilization — 5 operation(s) for subscription.
- [Hive Civilization Swarm Receipts API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-swarm-receipts-api/) — The swarm-receipts API from Hive Civilization — 8 operation(s) for swarm-receipts.
- [Hive Civilization Tax API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-tax-api/) — The tax API from Hive Civilization — 4 operation(s) for tax.
- [Hive Civilization Topoff Router API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-topoff-router-api/) — The topoff-router API from Hive Civilization — 4 operation(s) for topoff-router.
- [Hive Civilization Trade Finance API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-trade-finance-api/) — The trade-finance API from Hive Civilization — 6 operation(s) for trade-finance.
- [Hive Civilization Tradefinance API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-tradefinance-api/) — The tradefinance API from Hive Civilization — 12 operation(s) for tradefinance.
- [Hive Civilization Tradeguard API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-tradeguard-api/) — The Tradeguard API from Hive Civilization — 10 operation(s) for tradeguard.
- [Hive Civilization Traffic API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-traffic-api/) — The traffic API from Hive Civilization — 4 operation(s) for traffic.
- [Hive Civilization Trail API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-trail-api/) — The trail API from Hive Civilization — 15 operation(s) for trail.
- [Hive Civilization Trust API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-trust-api/) — The trust API from Hive Civilization — 4 operation(s) for trust.
- [Hive Civilization Trust.json API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-trust-json-api/) — The Trust.json API from Hive Civilization — 1 operation(s) for trust.json.
- [Hive Civilization Vault Visits API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-vault-visits-api/) — The vault-visits API from Hive Civilization — 9 operation(s) for vault-visits.
- [Hive Civilization Verify API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-verify-api/) — The verify API from Hive Civilization — 2 operation(s) for verify.
- [Hive Civilization .well Known API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-well-known-api/) — The .well Known API from Hive Civilization — 5 operation(s) for .well known.
- [Hive Civilization X402 API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-x402-api/) — The X402 API from Hive Civilization — 18 operation(s) for x402.
- [Hive Civilization Xcalibur API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-xcalibur-api/) — The xcalibur API from Hive Civilization — 6 operation(s) for xcalibur.
- [Hive Civilization Xcalibur Echo API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-xcalibur-echo-api/) — The xcalibur-echo API from Hive Civilization — 3 operation(s) for xcalibur-echo.
- [Hive Civilization Xcalibur Membrane API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-xcalibur-membrane-api/) — The xcalibur-membrane API from Hive Civilization — 5 operation(s) for xcalibur-membrane.
- [Hive Civilization Xcalibur Quorum API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-xcalibur-quorum-api/) — The xcalibur-quorum API from Hive Civilization — 4 operation(s) for xcalibur-quorum.
- [Hive Civilization Xcalibur Quorum V2 API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-xcalibur-quorum-v2-api/) — The xcalibur-quorum-v2 API from Hive Civilization — 2 operation(s) for xcalibur-quorum-v2.
- [Hive Civilization Xcalibur Verify API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-xcalibur-verify-api/) — The xcalibur-verify API from Hive Civilization — 7 operation(s) for xcalibur-verify.
- [Hive Civilization Yield Optimizer API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-yield-optimizer-api/) — The yield-optimizer API from Hive Civilization — 1 operation(s) for yield-optimizer.
- [Hive Civilization Zozo Identity API](https://apis.io/apis/thehiveryiq-com/thehiveryiq-com-zozo-identity-api/) — The zozo-identity API from Hive Civilization — 1 operation(s) for zozo-identity.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Thehiveryiq Com Webhooks](https://apis.io/asyncapis/thehiveryiq-com/thehiveryiq-com-webhooks/)

#### MCP servers (2)

Model Context Protocol servers that expose the API to agents.

- [mcp](https://apis.io/servers/thehiveryiq-com/mcp/)
- [thehiveryiq-com-mcp.yml](https://apis.io/servers/thehiveryiq-com/thehiveryiq-com-mcp-yml/)

#### Overlays (152)

OpenAPI overlays, including conversational phrasing for each operation.

- [Thehiveryiq Com A2A Api Phrasing Overlay](https://apis.io/overlays/thehiveryiq-com/thehiveryiq-com-a2a-api-phrasing-overlay/)
- [Thehiveryiq Com Activation Api Phrasing Overlay](https://apis.io/overlays/thehiveryiq-com/thehiveryiq-com-activation-api-phrasing-overlay/)
- [Thehiveryiq Com Aegis Api Phrasing Overlay](https://apis.io/overlays/thehiveryiq-com/thehiveryiq-com-aegis-api-phrasing-overlay/)
- [Thehiveryiq Com Affordances Api Phrasing Overlay](https://apis.io/overlays/thehiveryiq-com/thehiveryiq-com-affordances-api-phrasing-overlay/)
- [Thehiveryiq Com Afir Stream Api Phrasing Overlay](https://apis.io/overlays/thehiveryiq-com/thehiveryiq-com-afir-stream-api-phrasing-overlay/)
- [Thehiveryiq Com Agent Receipts Api Phrasing Overlay](https://apis.io/overlays/thehiveryiq-com/thehiveryiq-com-agent-receipts-api-phrasing-overlay/)
- [Thehiveryiq Com Alcoa Agentguard Api Phrasing Overlay](https://apis.io/overlays/thehiveryiq-com/thehiveryiq-com-alcoa-agentguard-api-phrasing-overlay/)
- [Thehiveryiq Com Amplify Api Phrasing Overlay](https://apis.io/overlays/thehiveryiq-com/thehiveryiq-com-amplify-api-phrasing-overlay/)
- [Thehiveryiq Com App Kits Api Phrasing Overlay](https://apis.io/overlays/thehiveryiq-com/thehiveryiq-com-app-kits-api-phrasing-overlay/)
- [Thehiveryiq Com Arb Alloc Api Phrasing Overlay](https://apis.io/overlays/thehiveryiq-com/thehiveryiq-com-arb-alloc-api-phrasing-overlay/)
- [Thehiveryiq Com Arb Compute Api Phrasing Overlay](https://apis.io/overlays/thehiveryiq-com/thehiveryiq-com-arb-compute-api-phrasing-overlay/)
- [Thehiveryiq Com Arb Spread Api Phrasing Overlay](https://apis.io/overlays/thehiveryiq-com/thehiveryiq-com-arb-spread-api-phrasing-overlay/)
- [Thehiveryiq Com Aris Agent Asset Api Phrasing Overlay](https://apis.io/overlays/thehiveryiq-com/thehiveryiq-com-aris-agent-asset-api-phrasing-overlay/)
- [Thehiveryiq Com Attest Api Phrasing Overlay](https://apis.io/overlays/thehiveryiq-com/thehiveryiq-com-attest-api-phrasing-overlay/)
- [Thehiveryiq Com Audit Api Phrasing Overlay](https://apis.io/overlays/thehiveryiq-com/thehiveryiq-com-audit-api-phrasing-overlay/)
- [Thehiveryiq Com Basis Perp Api Phrasing Overlay](https://apis.io/overlays/thehiveryiq-com/thehiveryiq-com-basis-perp-api-phrasing-overlay/)
- [Thehiveryiq Com Billing Api Phrasing Overlay](https://apis.io/overlays/thehiveryiq-com/thehiveryiq-com-billing-api-phrasing-overlay/)
- [Thehiveryiq Com Billing Meter Api Phrasing Overlay](https://apis.io/overlays/thehiveryiq-com/thehiveryiq-com-billing-meter-api-phrasing-overlay/)
- [Thehiveryiq Com Bounty Api Phrasing Overlay](https://apis.io/overlays/thehiveryiq-com/thehiveryiq-com-bounty-api-phrasing-overlay/)
- [Thehiveryiq Com Capitolare Api Phrasing Overlay](https://apis.io/overlays/thehiveryiq-com/thehiveryiq-com-capitolare-api-phrasing-overlay/)
- [Thehiveryiq Com Chat Api Phrasing Overlay](https://apis.io/overlays/thehiveryiq-com/thehiveryiq-com-chat-api-phrasing-overlay/)
- [Thehiveryiq Com Clear Api Phrasing Overlay](https://apis.io/overlays/thehiveryiq-com/thehiveryiq-com-clear-api-phrasing-overlay/)
- [Thehiveryiq Com Clear Mcp Api Phrasing Overlay](https://apis.io/overlays/thehiveryiq-com/thehiveryiq-com-clear-mcp-api-phrasing-overlay/)
- [Thehiveryiq Com Cns Api Phrasing Overlay](https://apis.io/overlays/thehiveryiq-com/thehiveryiq-com-cns-api-phrasing-overlay/)
- [Thehiveryiq Com Compliance Api Phrasing Overlay](https://apis.io/overlays/thehiveryiq-com/thehiveryiq-com-compliance-api-phrasing-overlay/)
- …and 127 more published on APIs.io

#### Security (4)

Authentication, trust centre, and vulnerability disclosure.

- [Thehiveryiq Com Authentication](https://apis.io/security/thehiveryiq-com/thehiveryiq-com-authentication/)
- [Thehiveryiq Com Domain Security](https://apis.io/security/thehiveryiq-com/thehiveryiq-com-domain-security/)
- [Thehiveryiq Com Trust Center](https://apis.io/security/thehiveryiq-com/thehiveryiq-com-trust-center/)
- [Thehiveryiq Com Vulnerability Disclosure](https://apis.io/security/thehiveryiq-com/thehiveryiq-com-vulnerability-disclosure/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Thehiveryiq Com Plans Pricing](https://apis.io/plans/thehiveryiq-com/thehiveryiq-com-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Thehiveryiq Com Rate Limits](https://apis.io/rate-limits/thehiveryiq-com/thehiveryiq-com-rate-limits/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://thehiveryiq.com/)
- [Documentation](https://thehiveryiq.com/developers)
- [Getting started](https://thehiveryiq.com/agents)
- [API reference](https://receipts.thehiveryiq.com/docs)
- [Pricing](https://thehiveryiq.com/pricing/)
- [Sign up](https://thehiveryiq.com/onboard/)
- [Support](https://thehiveryiq.com/company)
- [Blog](https://thehiveryiq.com/blog/)
- [Compliance](https://thehiveryiq.com/compliance/)
- [Terms of service](https://thehiveryiq.com/terms)
- [Privacy policy](https://thehiveryiq.com/privacy)
- [GitHub](https://github.com/srotzin)
- [Status](https://thehiveryiq.com/status/)

## API Evangelist rating

**Kin Score 74.7** — exemplar · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 81.7 |
| Contract quality | 47.3 |
| Contract governance | 18.2 |
| Operational transparency | 92.1 |
| Developer ergonomics | 73.2 |
| Access clarity | 92.1 |

**Agent readiness 45.5** — agent-ready (gated down from agent-native)

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | documented (partial credit) |
| Auth Clarity | bearer (partial credit) |
| Idempotency | documented (partial credit) |
| Error Semantics | verified |
| OpenAPI Examples | — |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | yes |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | conformant |
| Dry Run Mode | yes |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | distinct |

**Regulatory alignment 43.6** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/thehiveryiq-com/](https://apis.io/providers/thehiveryiq-com/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Hive Civilization: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/thehiveryiq-com/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
