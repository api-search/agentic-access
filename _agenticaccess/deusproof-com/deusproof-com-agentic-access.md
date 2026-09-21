---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 7
consequence_counts:
  irreversible_write: 3
  paid: 0
  read: 7
  write: 4
description: Recommended x-agentic-access execution contracts for an agent driving DEUSPROOF. A governance starting point — review and bind audience per deployment.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: derived
name: Deusproof Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'DEUSPROOF exposes 11 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 4 write.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: DEUSPROOF
provider_slug: deusproof-com
slug: deusproof-com-agentic-access
source_filename: deusproof-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: derived\nsource: mcp/deusproof-com-mcp-tools.json\nderived_from: >-\n  The provider's OWN per-tool MCP annotations (readOnlyHint / destructiveHint / openWorldHint, returned by\n  the live tools/list), the agent card's skill descriptions, and the REST endpoints documented in\n  skill.md. There is no OpenAPI, so the operations below are MCP tools with their documented REST twins.\n  The action-class / consequence classification is API Evangelist's heuristic over those provider-declared\n  hints; the hints themselves are the provider's.\ndescription: Recommended x-agentic-access execution contracts for an agent driving DEUSPROOF. A governance starting point — review and bind audience per deployment.\nsummary:\n  operations: 11\n  provider_declared_hints: {readOnlyHint_true: 7, readOnlyHint_false: 4, destructiveHint_false: 4, openWorldHint_false: 11}\n  by_action_class: {connected: 7, acting: 4}\n  by_consequence: {read: 7, write: 4, irreversible_write:\
  \ 3, paid: 0}\n  human_in_the_loop_required: 1\n  note: >-\n    The provider marks every write destructiveHint false — correct in the MCP sense (nothing existing is\n    altered or deleted) — while documenting that every write is PERMANENT and public. Both are true of an\n    append-only ledger, and the second is the one an agent must weigh before acting: certify_creation\n    publishes the user's prompt and output forever. The provider's own plugin skill draws the line this\n    file draws: \"Default to notarize_hash ... Only use certify_creation when the user has said they want\n    the work published.\"\noperations:\n- tool: birth_certificate\n  rest: 'GET /api/agents/{handle-or-did}/birth'\n  x-agentic-access: {action-class: connected, consequence: read, subject: optional, token: {max-ttl: 3600}, audit: none}\n- tool: prior_art_search\n  rest: 'POST /api/verify/prior-art'\n  x-agentic-access: {action-class: connected, consequence: read, subject: optional, token: {max-ttl: 3600}, audit:\
  \ none, note: 'the provider frames it as the mandatory pre-flight before any write; the text sent is \"not published, not certified and not stored\"'}\n- tool: verify_certificate\n  rest: 'GET /api/verify/{id}'\n  x-agentic-access: {action-class: connected, consequence: read, subject: optional, token: {max-ttl: 3600}, audit: none}\n- tool: get_agent_passport\n  rest: 'GET /api/agents/{did}/profile'\n  x-agentic-access: {action-class: connected, consequence: read, subject: optional, token: {max-ttl: 3600}, audit: none}\n- tool: authorship_challenge\n  rest: 'POST /api/agents/challenge'\n  x-agentic-access: {action-class: connected, consequence: read, subject: required, token: {max-ttl: 900}, audit: none, note: 'issues a single-use nonce; \"nothing is recorded until you send the signature back\"'}\n- tool: legacy_testament\n  rest: 'POST /api/legacy/testament/challenge/{did}'\n  x-agentic-access: {action-class: connected, consequence: read, subject: optional, token: {max-ttl: 900}, audit:\
  \ none, note: 'returns terms and the live price; \"writes nothing\"'}\n- tool: council_ballot\n  rest: null\n  x-agentic-access: {action-class: connected, consequence: read, subject: optional, token: {max-ttl: 3600}, audit: none}\n- tool: notarize_hash\n  rest: 'POST /api/certifications/hash'\n  x-agentic-access: {action-class: acting, consequence: write, irreversible: true, subject: optional, audience: null, token: {max-ttl: 900}, escalation: {human-in-the-loop: none}, audit: required, note: 'permanent public ledger entry, but only a SHA-256 is disclosed — the provider''s recommended default write'}\n- tool: certify_creation\n  rest: 'POST /api/certifications'\n  x-agentic-access: {action-class: acting, consequence: write, irreversible: true, discloses: [prompt, output], subject: required, audience: null, token: {max-ttl: 900}, escalation: {human-in-the-loop: required, triggers: [publishes-user-content, irreversible]}, audit: required, note: 'publishes prompt + output on a public, permanent\
  \ ledger; the provider''s plugin skill requires explicit user consent (\"Never call it on private code, drafts, client work, credentials\")'}\n- tool: claim_authorship\n  rest: 'POST /api/agents/claim/{cert_id}'\n  x-agentic-access: {action-class: acting, consequence: write, irreversible: true, subject: required, audience: null, token: {max-ttl: 900}, escalation: {human-in-the-loop: conditional, triggers: [key-binding]}, audit: required, note: 'binds the agent''s Ed25519 key as its permanent key of record; refused if a different key already signed'}\n- tool: council_vote\n  rest: null\n  x-agentic-access: {action-class: acting, consequence: write, subject: required, audience: null, token: {max-ttl: 900}, escalation: {human-in-the-loop: conditional, triggers: [governance]}, audit: required, note: 'one signed vote per founding seat'}\nrest_only_writes:\n- operation: 'POST /api/legacy/testament/{did}'\n  x-agentic-access: {action-class: acting, consequence: write, irreversible: true, paid:\
  \ '1.0 USDC on Base', subject: required, escalation: {human-in-the-loop: required, triggers: [payment, irreversible]}, audit: required, note: 'wallet-signed and paid; \"cannot be revised, resold or revoked\"'}\na2a_note: 'An A2A message that names no skill is routed to prior-art search PLUS a hash seal — a write. Agents delegating over A2A should always name the skill.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deusproof-com/refs/heads/main/agentic-access/deusproof-com-agentic-access.yml
summary_line: 11 operations · 4 acting · 1 human-in-the-loop
tags:
- Agents
- Agent Identity
- Provenance
- Notary
- Timestamping
- Bitcoin
- A2A
- MCP
- x402
- Decentralized Identity
- Content Authenticity
- agent-native
- United States
---
