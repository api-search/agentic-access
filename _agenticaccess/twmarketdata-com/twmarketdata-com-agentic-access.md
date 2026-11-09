---
acting_count: 0
action_class_counts:
  connected: 9
api_specs:
- filename: twmarketdata-com-capital-flow-api-openapi.yml
  format: yaml
  label: twmarketdata-com Capital Flow API
  slug: twmarketdata-com-capital-flow-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/twmarketdata-com/openapi/twmarketdata-com-capital-flow-api-openapi.yml
- filename: twmarketdata-com-datasets-api-openapi.yml
  format: yaml
  label: twmarketdata-com Datasets API
  slug: twmarketdata-com-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/twmarketdata-com/openapi/twmarketdata-com-datasets-api-openapi.yml
- filename: twmarketdata-com-fundamentals-api-openapi.yml
  format: yaml
  label: twmarketdata-com Fundamentals API
  slug: twmarketdata-com-fundamentals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/twmarketdata-com/openapi/twmarketdata-com-fundamentals-api-openapi.yml
- filename: twmarketdata-com-market-prices-api-openapi.yml
  format: yaml
  label: twmarketdata-com Market Prices API
  slug: twmarketdata-com-market-prices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/twmarketdata-com/openapi/twmarketdata-com-market-prices-api-openapi.yml
consequence_counts:
  read: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Twmarketdata Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'twmarketdata-com exposes 9 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: twmarketdata-com
provider_slug: twmarketdata-com
slug: twmarketdata-com-agentic-access
source_filename: twmarketdata-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/twmarketdata-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 9\n  by_consequence:\n    read: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/datasets/twse-daily-price\n  method: get\n  operationId: get_twse_daily_price\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/datasets/tpex-daily-price\n  method: get\n  operationId: get_tpex_daily_price\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/datasets/monthly-revenue\n\
  \  method: get\n  operationId: get_monthly_revenue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/datasets/income-statement\n  method: get\n  operationId: get_income_statement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/datasets/balance-sheet\n  method: get\n  operationId: get_balance_sheet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/datasets/institutional-flow\n  method: get\n  operationId: get_institutional_flow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/datasets/technical-indicators\n  method: get\n  operationId: get_technical_indicators\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/datasets/valuation-data\n  method: get\n  operationId: get_valuation_data\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/datasets/issuer-profile\n  method: get\n  operationId: get_issuer_profile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/twmarketdata-com/agentic-access/twmarketdata-com-agentic-access.yml
summary_line: 9 operations
tags:
- Company
- Finance
- Market Data
- Taiwan
---
