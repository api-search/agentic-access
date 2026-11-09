---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 20
api_specs:
- filename: bitcompare-net-benchmarks-api-openapi.yml
  format: yaml
  label: Bitcompare Benchmarks API
  slug: bitcompare-net-benchmarks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitcompare-net/openapi/bitcompare-net-benchmarks-api-openapi.yml
- filename: bitcompare-net-coins-api-openapi.yml
  format: yaml
  label: Bitcompare Coins API
  slug: bitcompare-net-coins-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitcompare-net/openapi/bitcompare-net-coins-api-openapi.yml
- filename: bitcompare-net-earn-api-openapi.yml
  format: yaml
  label: Bitcompare Earn API
  slug: bitcompare-net-earn-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitcompare-net/openapi/bitcompare-net-earn-api-openapi.yml
- filename: bitcompare-net-market-api-openapi.yml
  format: yaml
  label: Bitcompare Market API
  slug: bitcompare-net-market-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitcompare-net/openapi/bitcompare-net-market-api-openapi.yml
- filename: bitcompare-net-mcp-api-openapi.yml
  format: yaml
  label: Bitcompare MCP API
  slug: bitcompare-net-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitcompare-net/openapi/bitcompare-net-mcp-api-openapi.yml
- filename: bitcompare-net-prices-api-openapi.yml
  format: yaml
  label: Bitcompare Prices API
  slug: bitcompare-net-prices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitcompare-net/openapi/bitcompare-net-prices-api-openapi.yml
- filename: bitcompare-net-rates-api-openapi.yml
  format: yaml
  label: Bitcompare Rates API
  slug: bitcompare-net-rates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitcompare-net/openapi/bitcompare-net-rates-api-openapi.yml
- filename: bitcompare-net-stablecoins-api-openapi.yml
  format: yaml
  label: Bitcompare Stablecoins API
  slug: bitcompare-net-stablecoins-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitcompare-net/openapi/bitcompare-net-stablecoins-api-openapi.yml
- filename: bitcompare-net-symbols-api-openapi.yml
  format: yaml
  label: Bitcompare Symbols API
  slug: bitcompare-net-symbols-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitcompare-net/openapi/bitcompare-net-symbols-api-openapi.yml
consequence_counts:
  read: 20
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bitcompare Net Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 22
overview: 'Bitcompare exposes 22 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bitcompare
provider_slug: bitcompare-net
slug: bitcompare-net-agentic-access
source_filename: bitcompare-net-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/bitcompare-net.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 20\n    acting: 2\n  by_consequence:\n    read: 20\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/rates\n  method: get\n  operationId: get_rates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/rates/{symbol}\n  method: get\n  operationId: get_rate_by_symbol\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/rates/{symbol}/history\n\
  \  method: get\n  operationId: get_rate_history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/providers\n  method: get\n  operationId: list_providers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/coins/{coinId}\n  method: get\n  operationId: get_coin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/coins\n  method: get\n  operationId: list_coins\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/coins/top\n  method: get\n  operationId: top_coins\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/coins/{coinId}/similar\n  method: get\n  operationId: similar_coins\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/coins/{coinId}/history\n  method: get\n  operationId: coin_history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/prices/summary\n  method: get\n  operationId: get_price\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/prices/{symbol}\n  method: get\n  operationId: get_price_by_symbol\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/global-stats/summary\n\
  \  method: get\n  operationId: market_summary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/global-stats/fear-greed\n  method: get\n  operationId: fear_greed_index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/global-stats/movers\n  method: get\n  operationId: top_movers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/stablecoins/index\n  method: get\n  operationId: stablecoin_index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/stablecoins/peg-stability\n  method: get\n  operationId: stablecoin_peg_stability\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/symbols/resolve\n  method: get\n  operationId: resolve_symbol\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/symbols/resolve/batch\n  method: post\n  operationId: resolve_symbols_batch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/benchmarks/stablecoin\n  method: get\n  operationId: stablecoin_earn_benchmark\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/rates/changes\n  method:\
  \ get\n  operationId: get_rate_changes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/earn/products\n  method: get\n  operationId: list_earn_products\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp\n  method: post\n  operationId: mcpEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/bitcompare-net/agentic-access/bitcompare-net-agentic-access.yml
summary_line: 22 operations · 2 acting
tags:
- Cryptocurrency
- Finance
- Data
- Yield
---
