---
acting_count: 0
action_class_counts:
  connected: 29
api_specs:
- filename: polygon-stocks-openapi.yml
  format: yaml
  label: Polygon Stocks API
  slug: stocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-stocks-openapi.yml
- filename: polygon-options-openapi.yml
  format: yaml
  label: Polygon Options API
  slug: options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-options-openapi.yml
- filename: polygon-indices-openapi.yml
  format: yaml
  label: Polygon Indices API
  slug: indices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-indices-openapi.yml
- filename: polygon-forex-openapi.yml
  format: yaml
  label: Polygon Forex API
  slug: forex-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-forex-openapi.yml
- filename: polygon-crypto-openapi.yml
  format: yaml
  label: Polygon Crypto API
  slug: crypto-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-crypto-openapi.yml
- filename: polygon-reference-openapi.yml
  format: yaml
  label: Polygon Reference API
  slug: reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-reference-openapi.yml
- filename: polygon-websocket-asyncapi.yml
  format: yaml
  label: Polygon WebSocket API
  slug: websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/asyncapi/polygon-websocket-asyncapi.yml
consequence_counts:
  read: 29
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Polygon Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 29
overview: 'Polygon exposes 29 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 29 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Polygon
provider_slug: polygon
slug: polygon-agentic-access
source_filename: polygon-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/polygon-crypto-openapi.yml, openapi/polygon-forex-openapi.yml, openapi/polygon-indices-openapi.yml,\n  openapi/polygon-options-openapi.yml, openapi/polygon-reference-openapi.yml, openapi/polygon-stocks-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 29\n  by_action_class:\n    connected: 29\n  by_consequence:\n    read: 29\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/aggs/ticker/{cryptoTicker}/range/{multiplier}/{timespan}/{from}/{to}\n  method: get\n  operationId: getCryptoAggregateBars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/open-close/crypto/{from}/{to}/{date}\n\
  \  method: get\n  operationId: getCryptoDailyOpenClose\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/snapshot/locale/global/markets/crypto/tickers/{ticker}\n  method: get\n  operationId: getCryptoSnapshotForTicker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/snapshot/locale/global/markets/crypto/tickers/{ticker}/book\n  method: get\n  operationId: getCryptoL2Book\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/aggs/ticker/{forexTicker}/range/{multiplier}/{timespan}/{from}/{to}\n  method: get\n  operationId: getForexAggregateBars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/conversion/{from}/{to}\n  method: get\n  operationId: getForexConversion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/aggs/ticker/{forexTicker}/prev\n  method: get\n  operationId: getForexPreviousClose\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/last_quote/currencies/{from}/{to}\n  method: get\n  operationId: getForexLastQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/snapshot/indices\n  method: get\n  operationId: getIndicesSnapshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/aggs/ticker/{indicesTicker}/range/{multiplier}/{timespan}/{from}/{to}\n\
  \  method: get\n  operationId: getIndicesAggregateBars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/aggs/ticker/{indicesTicker}/prev\n  method: get\n  operationId: getIndicesPreviousClose\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/reference/options/contracts\n  method: get\n  operationId: listOptionsContracts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/snapshot/options/{underlyingAsset}/{optionContract}\n  method: get\n  operationId: getOptionContractSnapshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/snapshot/options/{underlyingAsset}\n\
  \  method: get\n  operationId: getOptionsChainSnapshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/aggs/ticker/{optionsTicker}/range/{multiplier}/{timespan}/{from}/{to}\n  method: get\n  operationId: getOptionsAggregateBars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/reference/tickers\n  method: get\n  operationId: listTickers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/reference/tickers/{ticker}\n  method: get\n  operationId: getTickerDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/reference/tickers/types\n  method: get\n  operationId:\
  \ listTickerTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/reference/markets\n  method: get\n  operationId: listMarkets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/reference/exchanges\n  method: get\n  operationId: listExchanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/marketstatus/upcoming\n  method: get\n  operationId: listUpcomingMarketHolidays\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/marketstatus/now\n  method: get\n  operationId: getCurrentMarketStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/reference/splits\n  method: get\n  operationId: listStockSplits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/reference/dividends\n  method: get\n  operationId: listDividends\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/reference/news\n  method: get\n  operationId: listTickerNews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/aggs/ticker/{stocksTicker}/range/{multiplier}/{timespan}/{from}/{to}\n  method: get\n  operationId: getStocksAggregateBars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/open-close/{stocksTicker}/{date}\n  method: get\n  operationId: getStocksDailyOpenClose\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/aggs/grouped/locale/us/market/stocks/{date}\n  method: get\n  operationId: getStocksGroupedDailyBars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/aggs/ticker/{stocksTicker}/prev\n  method: get\n  operationId: getStocksPreviousClose\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/agentic-access/polygon-agentic-access.yml
summary_line: 29 operations
tags:
- Finance
- Fintech
- Market Data
- Stocks
- Options
- Forex
- Crypto
- Indices
- Futures
- WebSockets
- Real-time
- Historical
- Public APIs
---
