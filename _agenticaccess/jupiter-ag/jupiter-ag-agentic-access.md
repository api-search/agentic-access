---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 1
api_specs:
- filename: jupiter-ag-events-api-openapi.yml
  format: yaml
  label: Jupiter Events API
  slug: jupiter-ag-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jupiter-ag/openapi/jupiter-ag-events-api-openapi.yml
- filename: jupiter-ag-forecast-api-openapi.yml
  format: yaml
  label: Jupiter Forecast API
  slug: jupiter-ag-forecast-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jupiter-ag/openapi/jupiter-ag-forecast-api-openapi.yml
- filename: jupiter-ag-history-api-openapi.yml
  format: yaml
  label: Jupiter History API
  slug: jupiter-ag-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jupiter-ag/openapi/jupiter-ag-history-api-openapi.yml
- filename: jupiter-ag-leaderboards-api-openapi.yml
  format: yaml
  label: Jupiter Leaderboards API
  slug: jupiter-ag-leaderboards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jupiter-ag/openapi/jupiter-ag-leaderboards-api-openapi.yml
- filename: jupiter-ag-markets-api-openapi.yml
  format: yaml
  label: Jupiter Markets API
  slug: jupiter-ag-markets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jupiter-ag/openapi/jupiter-ag-markets-api-openapi.yml
- filename: jupiter-ag-orderbook-api-openapi.yml
  format: yaml
  label: Jupiter Orderbook API
  slug: jupiter-ag-orderbook-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jupiter-ag/openapi/jupiter-ag-orderbook-api-openapi.yml
- filename: jupiter-ag-orders-api-openapi.yml
  format: yaml
  label: Jupiter Orders API
  slug: jupiter-ag-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jupiter-ag/openapi/jupiter-ag-orders-api-openapi.yml
- filename: jupiter-ag-positions-api-openapi.yml
  format: yaml
  label: Jupiter Positions API
  slug: jupiter-ag-positions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jupiter-ag/openapi/jupiter-ag-positions-api-openapi.yml
- filename: jupiter-ag-profile-api-openapi.yml
  format: yaml
  label: Jupiter Profile API
  slug: jupiter-ag-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jupiter-ag/openapi/jupiter-ag-profile-api-openapi.yml
- filename: jupiter-ag-trades-api-openapi.yml
  format: yaml
  label: Jupiter Trades API
  slug: jupiter-ag-trades-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jupiter-ag/openapi/jupiter-ag-trades-api-openapi.yml
- filename: jupiter-ag-trading-api-openapi.yml
  format: yaml
  label: Jupiter Trading API
  slug: jupiter-ag-trading-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jupiter-ag/openapi/jupiter-ag-trading-api-openapi.yml
- filename: jupiter-ag-vault-api-openapi.yml
  format: yaml
  label: Jupiter Vault API
  slug: jupiter-ag-vault-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jupiter-ag/openapi/jupiter-ag-vault-api-openapi.yml
consequence_counts:
  read: 1
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Jupiter Ag Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 2
overview: 'Jupiter exposes 2 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Jupiter
provider_slug: jupiter-ag
slug: jupiter-ag-agentic-access
source_filename: jupiter-ag-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/jupiter-ag-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 2\n  by_action_class:\n    connected: 1\n    acting: 1\n  by_consequence:\n    read: 1\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /quote\n  method: get\n  operationId: getQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /swap\n  method: post\n  operationId: postSwap\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/jupiter-ag/agentic-access/jupiter-ag-agentic-access.yml
summary_line: 2 operations · 1 acting
tags:
- Solana
- DeFi
- DEX Aggregator
- Swap
- Perpetuals
- Limit Orders
- DCA
- Lending
---
