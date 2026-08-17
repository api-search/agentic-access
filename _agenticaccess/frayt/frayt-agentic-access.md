---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 1
api_specs:
- filename: frayt-matches-openapi.yml
  format: yaml
  label: FRAYT Client API
  slug: frayt-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frayt/refs/heads/main/openapi/frayt-matches-openapi.yml
consequence_counts:
  read: 1
  safety-critical: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 7
kind: agentic-access
layout: agentic-access
method: generated
name: Frayt Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2.2/matches
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2.2/matches/estimate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/v2.2/matches/estimate/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v2.2/matches/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/v2.2/matches/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/v2.2/matches/{match_id}/stops/{stop_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2.2/oauth/token
operation_count: 8
overview: 'FRAYT exposes 8 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 7 safety-critical.


  7 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: FRAYT
provider_slug: frayt
slug: frayt-agentic-access
source_filename: frayt-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-16'\nmethod: generated\nsource: openapi/frayt-match-estimates-openapi.yml, openapi/frayt-matches-openapi.yml, openapi/frayt-oauth-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nx-apievangelist-review:\n  reviewed: '2026-08-16'\n  by: enrichment pipeline (human-readable curation note, classifications left unmodified)\n  note: >-\n    The heuristic classifier raised every write operation on this API to\n    consequence \"safety-critical\" because the FRAYT vocabulary is dense with\n    dispatch/delivery keywords. Two of those are over-classified against what the\n    operations actually do, and an implementer should downgrade them before use:\n    (1) POST /api/v2.2/matches/estimate only PRICES a delivery — it books nothing,\n    charges\
  \ nothing and dispatches nobody, so it is effectively a read;\n    (2) POST /api/v2.2/oauth/token is a credential exchange, not a physical action.\n    The genuinely consequential operations are POST /api/v2.2/matches and\n    PATCH /api/v2.2/matches/estimate/{id} (both dispatch a real driver),\n    DELETE /api/v2.2/matches/{id} (irreversible, up to 50% cancellation charge per\n    FRAYT's EULA), and PATCH /api/v2.2/matches/{match_id}/stops/{stop_id} (a\n    monetary tip change). Those four are correctly flagged.\n    Note also that FRAYT supports no idempotency key, which raises the real risk of\n    every write here: a retry is a duplicate dispatch. See\n    conventions/frayt-conventions.yml.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 7\n    connected: 1\n  by_consequence:\n    safety-critical: 7\n    read: 1\n  human_in_the_loop_required: 7\noperations:\n- path: /api/v2.2/matches/estimate\n  method: post\n  operationId: FraytElixirWeb.API.V2x2.MatchEstimateController.create\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2.2/matches/estimate/{id}\n  method: patch\n  operationId: FraytElixirWeb.API.V2x2.MatchEstimateController.update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2.2/matches\n  method: post\n  operationId: FraytElixirWeb.API.V2x2.MatchController.create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2.2/matches/{id}\n  method: delete\n  operationId: FraytElixirWeb.API.V2x2.MatchController.delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2.2/matches/{id}\n  method: get\n  operationId: FraytElixirWeb.API.V2x2.MatchController.show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2.2/matches/{id}\n  method: patch\n  operationId: FraytElixirWeb.API.V2x2.MatchController.update\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2.2/matches/{match_id}/stops/{stop_id}\n  method: patch\n  operationId: FraytElixirWeb.API.V2x2.MatchStopController.update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2.2/oauth/token\n  method: post\n  operationId: FraytElixirWeb.API.OauthController.authenticate\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n   \
  \   exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/frayt/refs/heads/main/agentic-access/frayt-agentic-access.yml
summary_line: 8 operations · 7 acting · 7 human-in-the-loop
tags:
- Company
- Last Mile Delivery
- Logistics
- Courier
- On Demand Delivery
- Shipping
- Freight
- Supply Chain
- Transportation
- Third Party Logistics
- Delivery Tracking
- Webhooks
---
