---
acting_count: 0
action_class_counts:
  connected: 26
api_specs:
- filename: twelvedata-openapi.yml
  format: yaml
  label: Twelve Data Time Series API
  slug: twelvedata-time-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twelvedata/refs/heads/main/openapi/twelvedata-openapi.yml
- filename: twelvedata-openapi.yml
  format: yaml
  label: Twelve Data Quotes and Price API
  slug: twelvedata-quotes-price-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twelvedata/refs/heads/main/openapi/twelvedata-openapi.yml
- filename: twelvedata-openapi.yml
  format: yaml
  label: Twelve Data Technical Indicators API
  slug: twelvedata-technical-indicators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twelvedata/refs/heads/main/openapi/twelvedata-openapi.yml
- filename: twelvedata-openapi.yml
  format: yaml
  label: Twelve Data Reference Data API
  slug: twelvedata-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twelvedata/refs/heads/main/openapi/twelvedata-openapi.yml
- filename: twelvedata-openapi.yml
  format: yaml
  label: Twelve Data Fundamentals API
  slug: twelvedata-fundamentals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twelvedata/refs/heads/main/openapi/twelvedata-openapi.yml
- filename: twelvedata-asyncapi.yml
  format: yaml
  label: Twelve Data WebSocket Streaming API
  slug: twelvedata-websocket-streaming-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/twelvedata/refs/heads/main/asyncapi/twelvedata-asyncapi.yml
consequence_counts:
  read: 26
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Twelvedata Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 26
overview: 'Twelve Data exposes 26 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 26 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Twelve Data
provider_slug: twelvedata
slug: twelvedata-agentic-access
source_filename: twelvedata-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/twelvedata-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 26\n  by_action_class:\n    connected: 26\n  by_consequence:\n    read: 26\n  human_in_the_loop_required: 0\noperations:\n- path: /time_series\n  method: get\n  operationId: getTimeSeries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /time_series/cross\n  method: get\n  operationId: getTimeSeriesCross\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /eod\n  method: get\n  operationId: getEndOfDay\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /quote\n  method: get\n  operationId: getQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /price\n  method: get\n  operationId: getPrice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /market_movers/{market}\n  method: get\n  operationId: getMarketMovers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /market_state\n  method: get\n  operationId: getMarketState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rsi\n  method: get\n\
  \  operationId: getRSI\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /macd\n  method: get\n  operationId: getMACD\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bbands\n  method: get\n  operationId: getBBands\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /technical_indicators\n  method: get\n  operationId: listTechnicalIndicators\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stocks\n  method: get\n  operationId: listStocks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /forex_pairs\n  method: get\n  operationId: listForexPairs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cryptocurrencies\n  method: get\n  operationId: listCryptocurrencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /etfs\n  method: get\n  operationId: listEtfs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /indices\n  method: get\n  operationId: listIndices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exchanges\n  method: get\n  operationId: listExchanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /symbol_search\n  method: get\n  operationId: symbolSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /earliest_timestamp\n  method: get\n  operationId: getEarliestTimestamp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile\n  method: get\n  operationId: getProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dividends\n  method: get\n  operationId: getDividends\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /earnings\n  method: get\n  operationId: getEarnings\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /income_statement\n  method: get\n  operationId: getIncomeStatement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /balance_sheet\n  method: get\n  operationId: getBalanceSheet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cash_flow\n  method: get\n  operationId: getCashFlow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /statistics\n  method: get\n  operationId: getStatistics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/twelvedata/refs/heads/main/agentic-access/twelvedata-agentic-access.yml
summary_line: 26 operations
tags:
- Market Data
- Financial Data
- Stocks
- Forex
- Crypto
- Real-Time Data
- Technical Indicators
- Fundamentals
---
