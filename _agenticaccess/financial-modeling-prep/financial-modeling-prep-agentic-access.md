---
acting_count: 0
action_class_counts:
  connected: 10
api_specs:
- filename: financial-modeling-prep-balance-sheet-statement-api-openapi.yml
  format: yaml
  label: Financial Modeling Prep Balance Sheet Statement API
  slug: financial-modeling-prep-balance-sheet-statement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/financial-modeling-prep/refs/heads/main/openapi/financial-modeling-prep-balance-sheet-statement-api-openapi.yml
- filename: financial-modeling-prep-cash-flow-statement-api-openapi.yml
  format: yaml
  label: Financial Modeling Prep Cash Flow Statement API
  slug: financial-modeling-prep-cash-flow-statement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/financial-modeling-prep/refs/heads/main/openapi/financial-modeling-prep-cash-flow-statement-api-openapi.yml
- filename: financial-modeling-prep-historical-price-full-api-openapi.yml
  format: yaml
  label: Financial Modeling Prep Historical Price Full API
  slug: financial-modeling-prep-historical-price-full-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/financial-modeling-prep/refs/heads/main/openapi/financial-modeling-prep-historical-price-full-api-openapi.yml
- filename: financial-modeling-prep-income-statement-api-openapi.yml
  format: yaml
  label: Financial Modeling Prep Income Statement API
  slug: financial-modeling-prep-income-statement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/financial-modeling-prep/refs/heads/main/openapi/financial-modeling-prep-income-statement-api-openapi.yml
- filename: financial-modeling-prep-insider-trading-api-openapi.yml
  format: yaml
  label: Financial Modeling Prep Insider Trading API
  slug: financial-modeling-prep-insider-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/financial-modeling-prep/refs/heads/main/openapi/financial-modeling-prep-insider-trading-api-openapi.yml
- filename: financial-modeling-prep-profile-api-openapi.yml
  format: yaml
  label: Financial Modeling Prep Profile API
  slug: financial-modeling-prep-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/financial-modeling-prep/refs/heads/main/openapi/financial-modeling-prep-profile-api-openapi.yml
- filename: financial-modeling-prep-quote-api-openapi.yml
  format: yaml
  label: Financial Modeling Prep Quote API
  slug: financial-modeling-prep-quote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/financial-modeling-prep/refs/heads/main/openapi/financial-modeling-prep-quote-api-openapi.yml
- filename: financial-modeling-prep-ratios-api-openapi.yml
  format: yaml
  label: Financial Modeling Prep Ratios API
  slug: financial-modeling-prep-ratios-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/financial-modeling-prep/refs/heads/main/openapi/financial-modeling-prep-ratios-api-openapi.yml
- filename: financial-modeling-prep-search-api-openapi.yml
  format: yaml
  label: Financial Modeling Prep Search API
  slug: financial-modeling-prep-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/financial-modeling-prep/refs/heads/main/openapi/financial-modeling-prep-search-api-openapi.yml
- filename: financial-modeling-prep-stock-api-openapi.yml
  format: yaml
  label: Financial Modeling Prep Stock API
  slug: financial-modeling-prep-stock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/financial-modeling-prep/refs/heads/main/openapi/financial-modeling-prep-stock-api-openapi.yml
consequence_counts:
  read: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Financial Modeling Prep Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'Financial Modeling Prep exposes 10 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Financial Modeling Prep
provider_slug: financial-modeling-prep
slug: financial-modeling-prep-agentic-access
source_filename: financial-modeling-prep-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: generated\nsource: openapi/financial-modeling-prep-balance-sheet-statement-api-openapi.yml, openapi/financial-modeling-prep-cash-flow-statement-api-openapi.yml,\n  openapi/financial-modeling-prep-historical-price-full-api-openapi.yml, openapi/financial-modeling-prep-income-statement-api-openapi.yml,\n  openapi/financial-modeling-prep-insider-trading-api-openapi.yml, openapi/financial-modeling-prep-profile-api-openapi.yml,\n  openapi/financial-modeling-prep-quote-api-openapi.yml, openapi/financial-modeling-prep-ratios-api-openapi.yml,\n  openapi/financial-modeling-prep-search-api-openapi.yml, openapi/financial-modeling-prep-stock-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n\
  \    connected: 10\n  by_consequence:\n    read: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /balance-sheet-statement\n  method: get\n  operationId: getBalanceSheet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cash-flow-statement\n  method: get\n  operationId: getCashFlowStatement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /historical-price-eod/full\n  method: get\n  operationId: getHistoricalPrice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /income-statement\n  method: get\n  operationId: getIncomeStatement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /insider-trading/search\n  method: get\n  operationId: getInsiderTrading\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile\n  method: get\n  operationId: getCompanyProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /quote\n  method: get\n  operationId: getQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ratios\n  method: get\n  operationId: getFinancialRatios\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search-symbol\n  method: get\n  operationId: searchSymbols\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stock-list\n  method: get\n  operationId: listStocks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/financial-modeling-prep/refs/heads/main/agentic-access/financial-modeling-prep-agentic-access.yml
summary_line: 10 operations
tags:
- Financial Data
- Market Data
- Stocks
- Quotes
- Fundamentals
- Financial Statements
- Historical
---
