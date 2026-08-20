---
acting_count: 0
action_class_counts:
  connected: 6
api_specs:
- filename: bargo-congress-trades-api-members-api-openapi.yml
  format: yaml
  label: Bargo Congress Trades API Members API
  slug: bargo-congress-trades-api-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bargo-congress-trades-api/refs/heads/main/openapi/bargo-congress-trades-api-members-api-openapi.yml
- filename: bargo-congress-trades-api-statistics-api-openapi.yml
  format: yaml
  label: Bargo Congress Trades API Statistics API
  slug: bargo-congress-trades-api-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bargo-congress-trades-api/refs/heads/main/openapi/bargo-congress-trades-api-statistics-api-openapi.yml
- filename: bargo-congress-trades-api-trades-api-openapi.yml
  format: yaml
  label: Bargo Congress Trades API Trades API
  slug: bargo-congress-trades-api-trades-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bargo-congress-trades-api/refs/heads/main/openapi/bargo-congress-trades-api-trades-api-openapi.yml
consequence_counts:
  read: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bargo Congress Trades Api Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Bargo Congress Trades API exposes 6 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bargo Congress Trades API
provider_slug: bargo-congress-trades-api
slug: bargo-congress-trades-api-agentic-access
source_filename: bargo-congress-trades-api-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: generated\nsource: openapi/bargo-congress-trades-api-congress-trades-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 6\n  by_consequence:\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /trades\n  method: get\n  operationId: listCongressTrades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trades/{ticker}\n  method: get\n  operationId: listCongressTradesByTicker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /members\n  method:\
  \ get\n  operationId: listCongressMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /members/{member_slug}\n  method: get\n  operationId: getCongressMember\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats\n  method: get\n  operationId: getCongressTradeStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: getCongressApiHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bargo-congress-trades-api/refs/heads/main/agentic-access/bargo-congress-trades-api-agentic-access.yml
summary_line: 6 operations
tags:
- Congress
- Finance
- Stocks
- Government
- stock-act
- MCP
- Congressional Trading
- financial-disclosure
- Market Data
- Public Data
- Free API
- Open Data
---
