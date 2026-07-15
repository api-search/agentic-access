---
acting_count: 0
action_class_counts:
  connected: 14
api_specs:
- filename: marketdata-app-openapi.yml
  format: yaml
  label: Market Data Stocks API
  slug: marketdata-app-stocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketdata-app/refs/heads/main/openapi/marketdata-app-openapi.yml
- filename: marketdata-app-openapi.yml
  format: yaml
  label: Market Data Options API
  slug: marketdata-app-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketdata-app/refs/heads/main/openapi/marketdata-app-openapi.yml
- filename: marketdata-app-openapi.yml
  format: yaml
  label: Market Data Indices API
  slug: marketdata-app-indices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketdata-app/refs/heads/main/openapi/marketdata-app-openapi.yml
- filename: marketdata-app-openapi.yml
  format: yaml
  label: Market Data Markets API
  slug: marketdata-app-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketdata-app/refs/heads/main/openapi/marketdata-app-openapi.yml
consequence_counts:
  read: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Marketdata App Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'Market Data exposes 14 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Market Data
provider_slug: marketdata-app
slug: marketdata-app-agentic-access
source_filename: marketdata-app-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/marketdata-app-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 14\n  by_consequence:\n    read: 14\n  human_in_the_loop_required: 0\noperations:\n- path: /stocks/candles/{resolution}/{symbol}/\n  method: get\n  operationId: getStockCandles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stocks/quotes/{symbol}/\n  method: get\n  operationId: getStockQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stocks/bulkquotes/\n\
  \  method: get\n  operationId: getStockBulkQuotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stocks/bulkcandles/{resolution}/\n  method: get\n  operationId: getStockBulkCandles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stocks/earnings/{symbol}/\n  method: get\n  operationId: getStockEarnings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stocks/news/{symbol}/\n  method: get\n  operationId: getStockNews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /options/expirations/{underlyingSymbol}/\n  method: get\n  operationId: getOptionExpirations\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /options/lookup/{userInput}/\n  method: get\n  operationId: getOptionLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /options/strikes/{underlyingSymbol}/\n  method: get\n  operationId: getOptionStrikes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /options/chain/{underlyingSymbol}/\n  method: get\n  operationId: getOptionChain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /options/quotes/{optionSymbol}/\n  method: get\n  operationId: getOptionQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /indices/candles/{resolution}/{symbol}/\n  method: get\n  operationId: getIndexCandles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /indices/quotes/{symbol}/\n  method: get\n  operationId: getIndexQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/status/\n  method: get\n  operationId: getMarketStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marketdata-app/refs/heads/main/agentic-access/marketdata-app-agentic-access.yml
summary_line: 14 operations
tags:
- Market Data
- Financial Data
- Stocks
- Options
- Indices
- Real-Time Data
- Historical Data
- Quotes
---
