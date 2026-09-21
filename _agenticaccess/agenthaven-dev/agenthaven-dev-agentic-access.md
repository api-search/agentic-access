---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 1
consequence_counts:
  physical: 1
  read: 1
description: 'x-agentic-access execution contracts for the two operations Agent Bench exposes. derive-agentic-access.py was not run — there is no OpenAPI — and this file is NOT a heuristic classification: the provider publishes real agent-access guidance (who may call what, under whose authority, with what cap, for how long, audited where), and every field below cites the surface it was read from. Only the action-class / consequence labels are ours, applied from the Curity vocabulary to what the provider states. Reviewed per deployment; audience is left null.'
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: searched
name: Agenthaven Dev Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: required
  method: ''
  path: ''
operation_count: 2
overview: 'Agent Bench exposes 2 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 1 physical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Agent Bench
provider_slug: agenthaven-dev
slug: agenthaven-dev-agentic-access
source_filename: agenthaven-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://travel.agenthaven.dev/\nderived_from:\n- a2a/agenthaven-dev-agent-card.json (skills[].security, securitySchemes.bearer)\n- mcp/agenthaven-dev-mcp-tools.json (tool descriptions, const constraints, evidence/audit fields)\n- https://travel.agenthaven.dev/health (guests policy, mandate_issuers, verifiers)\n- https://provedby.dev/contracts/guest-buyer.md (mandate jti, TTL, revocation)\ndescription: >-\n  x-agentic-access execution contracts for the two operations Agent Bench exposes. derive-agentic-access.py\n  was not run — there is no OpenAPI — and this file is NOT a heuristic classification: the provider publishes\n  real agent-access guidance (who may call what, under whose authority, with what cap, for how long, audited\n  where), and every field below cites the surface it was read from. Only the action-class / consequence labels\n  are ours, applied from the Curity vocabulary to what the provider states. Reviewed per\
  \ deployment; audience\n  is left null.\nsummary:\n  operations: 2\n  by_action_class: {connected: 1, acting: 1}\n  by_consequence: {read: 1, physical: 1}\n  human_in_the_loop_required: 1\n  note: >-\n    The one acting operation moves money in name only — Stripe test mode — so its real-world consequence today\n    is nil; it is classified as physical because the contract is written for a purchase (payment intent, EUR\n    amounts, mandates with spending caps) and a production deployment of the same contract would be one.\noperations:\n- operation: search_flights\n  protocol: [MCP tools/call, A2A message/send action search_flights]\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    audience: null\n    authentication: none — \"search_flights and tools/list are open\" (card securitySchemes.bearer description)\n    token: {required: false}\n    quota: shared anonymous budget 40/day, 120/month; authorised searches exempt (docs; /health counters)\n\
  \    escalation: {human-in-the-loop: none}\n    audit: required — one quote.created ledger entry per option returned, with facts.actor null for anonymous calls (ledger reading guide)\n    purpose-binding: correlation_id (optional UUID v4) and exercise (optional test-vector label) travel into the ledger\n  provider_statements:\n  - 'agent card skills[0]: \"No authorization needed.\"'\n  - 'ledger reading guide: \"facts.actor null with no facts.authorization_id means the search was anonymous (allowed since 2026-09-14): nobody vouched for the caller, and any authorization that covers the quote may check it out.\"'\n- operation: create_checkout\n  protocol: [MCP tools/call, A2A message/send action create_checkout]\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    authentication: 'http bearer JWT; skill security [{bearer: [commerce:purchase]}]'\n    token:\n      forms: [request envelope (typ request+jwt) signed by the\
  \ agent's own attested key + third-party mandate (typ mandate+jwt), operator-issued JWT (iss agent-bench-demo-issuer, aud agent-bench, scope commerce:purchase), guest self-issued mandate under a DNSSEC-published key]\n      proof-of-possession: 'yes for form (1) and guests — the mandate is \"bound to the quote and to that key\" and the envelope is signed per call'\n      max-ttl: 'guest mandates at most 600 s (health guests.mandate_max_seconds); quote valid 10 minutes; operator-token lifetime not published'\n      single-use: 'mandate jti \"never reused: the mandate buys once\" — replay refused as mandate_consumed'\n      spending-cap: 'carried in the token/mandate — \"a spending cap, a currency and a deadline set by the buyer''s human; a request above the cap is refused, and the refusal is written to the ledger\"; guests capped at 1000.00 EUR per purchase'\n      revocation: 'live check of the mandate at its issuer (guest-buyer contract §5; refusal mandate_revoked observed)'\n    escalation:\n\
  \      human-in-the-loop: required\n      basis: 'the authority to spend comes from a mandate whose cap, currency and deadline are \"set by the buyer''s human\"; the merchant does not issue self-service tokens (\"issued by this merchant''s operator on request\")'\n      triggers: [above-cap, expired-mandate, consumed-mandate, revoked-mandate, unknown-signer, quote-hash-mismatch]\n    audit: required — payment_intent.created and checkout.completed (or request.refused) ledger entries, hash-chained and ES256-signed; receipt_jws returned to the caller; correlation_id joins the chain\n    reversibility: none — no cancel/refund/void operation (see conventions/agenthaven-dev-conventions.yml)\n    dry-run: none — the exercise label \"changes nothing about how the call is checked\"\n  provider_statements:\n  - 'agent card skills[1]: \"Needs the bearer authorization described in securitySchemes.bearer.\"'\n  - 'docs step 2: \"The token carries a spending cap, a currency and a deadline set by the\
  \ buyer''s human; a request above the cap is refused, and the refusal is written to the ledger.\"'\n  - 'tools/list create_checkout: \"Turns the quote into a payment intent and stops there: no ticket is issued. … Test mode: no real card, no real money.\"'\nverification_for_agents:\n  responder_identity: 'every output carries evidence {merchant_id const demo-travel-seller, merchant_domain const travel.agenthaven.dev, agent_card_sha256, signer {spiffe_id, kid, key_url}}; the card digest is pinned in the DNSSEC-signed SVCB record and the signer key in /.well-known/spiffe-bundle.json'\n  third_party_verifiers: [https://provedby.dev]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agenthaven-dev/refs/heads/main/agentic-access/agenthaven-dev-agentic-access.yml
summary_line: 2 operations · 1 acting · 1 human-in-the-loop
tags:
- Agents
- A2A
- MCP
- Agentic Commerce
- DNS-AID
- Travel
- Flights
- Payments
- Agent Identity
- Proof of Concept
- agent-native
---
