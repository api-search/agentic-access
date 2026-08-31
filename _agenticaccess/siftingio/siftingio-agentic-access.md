---
acting_count: 0
action_class_counts:
  connected: 37
api_specs:
- filename: siftingio-asyncapi.yaml
  format: yaml
  label: SiftingIO Live Stream
  slug: siftingio-live-stream
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/siftingio/refs/heads/main/asyncapi/siftingio-asyncapi.yaml
- filename: siftingio-commodities-api-openapi.yml
  format: yaml
  label: SiftingIO Commodities API
  slug: siftingio-commodities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siftingio/refs/heads/main/openapi/siftingio-commodities-api-openapi.yml
- filename: siftingio-convert-api-openapi.yml
  format: yaml
  label: SiftingIO Convert API
  slug: siftingio-convert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siftingio/refs/heads/main/openapi/siftingio-convert-api-openapi.yml
- filename: siftingio-crypto-api-openapi.yml
  format: yaml
  label: SiftingIO Crypto API
  slug: siftingio-crypto-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siftingio/refs/heads/main/openapi/siftingio-crypto-api-openapi.yml
- filename: siftingio-dex-api-openapi.yml
  format: yaml
  label: SiftingIO DEX API
  slug: siftingio-dex-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siftingio/refs/heads/main/openapi/siftingio-dex-api-openapi.yml
- filename: siftingio-economiccalendar-api-openapi.yml
  format: yaml
  label: SiftingIO Economic Calendar API
  slug: siftingio-economiccalendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siftingio/refs/heads/main/openapi/siftingio-economiccalendar-api-openapi.yml
- filename: siftingio-filers-api-openapi.yml
  format: yaml
  label: SiftingIO Filers API
  slug: siftingio-filers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siftingio/refs/heads/main/openapi/siftingio-filers-api-openapi.yml
- filename: siftingio-forex-api-openapi.yml
  format: yaml
  label: SiftingIO Forex API
  slug: siftingio-forex-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siftingio/refs/heads/main/openapi/siftingio-forex-api-openapi.yml
- filename: siftingio-live-api-openapi.yml
  format: yaml
  label: SiftingIO Live API
  slug: siftingio-live-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siftingio/refs/heads/main/openapi/siftingio-live-api-openapi.yml
- filename: siftingio-markets-api-openapi.yml
  format: yaml
  label: SiftingIO Markets API
  slug: siftingio-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siftingio/refs/heads/main/openapi/siftingio-markets-api-openapi.yml
- filename: siftingio-signals-api-openapi.yml
  format: yaml
  label: SiftingIO Signals API
  slug: siftingio-signals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siftingio/refs/heads/main/openapi/siftingio-signals-api-openapi.yml
- filename: siftingio-stocks-api-openapi.yml
  format: yaml
  label: SiftingIO Stocks API
  slug: siftingio-stocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siftingio/refs/heads/main/openapi/siftingio-stocks-api-openapi.yml
consequence_counts:
  read: 37
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Siftingio Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 37
overview: 'SiftingIO exposes 37 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 37 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SiftingIO
provider_slug: siftingio
slug: siftingio-agentic-access
source_filename: siftingio-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: generated\nsource: openapi/siftingio-commodities-api-openapi.yml, openapi/siftingio-convert-api-openapi.yml,\n  openapi/siftingio-crypto-api-openapi.yml, openapi/siftingio-dex-api-openapi.yml, openapi/siftingio-economiccalendar-api-openapi.yml,\n  openapi/siftingio-filers-api-openapi.yml, openapi/siftingio-forex-api-openapi.yml, openapi/siftingio-live-api-openapi.yml,\n  openapi/siftingio-markets-api-openapi.yml, openapi/siftingio-signals-api-openapi.yml, openapi/siftingio-stocks-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 37\n  by_action_class:\n    connected: 37\n  by_consequence:\n    read: 37\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/hist/commodities/{symbol}/bars\n  method:\
  \ get\n  operationId: getCommodityBars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/convert/{from}/{to}\n  method: get\n  operationId: convertAmount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/hist/crypto/{symbol}/bars\n  method: get\n  operationId: getCryptoBars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/hist/dex/{symbol}/bars\n  method: get\n  operationId: getDexBars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fnd/dex/wallet/{chain}/{address}\n  method: get\n  operationId: getWalletPortfolio\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fnd/economic-calendar\n  method: get\n  operationId: getEconomicCalendar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fnd/filers/{filer}/holdings\n  method: get\n  operationId: getFilerHoldings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/hist/forex/{pair}/bars\n  method: get\n  operationId: getForexBars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/last/trade/{venue}/{symbol}\n  method: get\n  operationId: getLastTrade\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/last/quote/{venue}/{symbol}\n  method: get\n  operationId: getLastQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/last/close/{venue}/{symbol}\n  method: get\n  operationId: getLastClose\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/last/tvl/{chain}/{pair}\n  method: get\n  operationId: getLastTVL\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/snapshot/{venue}\n  method: get\n  operationId: getSnapshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fnd/markets\n  method: get\n  operationId: listMarkets\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fnd/markets/status\n  method: get\n  operationId: getAllMarketStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fnd/markets/{market}/status\n  method: get\n  operationId: getMarketStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fnd/markets/{market}/hours\n  method: get\n  operationId: getMarketHours\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fnd/markets/{market}/calendar\n  method: get\n  operationId: getMarketCalendar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/last/signals/{venue}/{symbol}\n  method: get\n  operationId: getLiveSignal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/hist/{venue}/{symbol}/signals\n  method: get\n  operationId: getSignalHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fnd/stocks/search\n  method: get\n  operationId: searchStocks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fnd/stocks/screener/{concept}/{period}\n  method: get\n  operationId: getScreener\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fnd/stocks/{ticker}/profile\n\
  \  method: get\n  operationId: getCompanyProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fnd/stocks/{ticker}/filings\n  method: get\n  operationId: listFilings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fnd/stocks/{ticker}/filings/{accession}\n  method: get\n  operationId: getFiling\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fnd/stocks/{ticker}/filings/{accession}/sections\n  method: get\n  operationId: getFilingSections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fnd/stocks/{ticker}/filings/{accession}/sections/{section}\n  method:\
  \ get\n  operationId: getFilingSection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fnd/stocks/{ticker}/risk-factors-diff\n  method: get\n  operationId: getRiskFactorsDiff\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fnd/stocks/{ticker}/ratios\n  method: get\n  operationId: getRatios\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fnd/stocks/{ticker}/earnings\n  method: get\n  operationId: listEarnings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fnd/stocks/{ticker}/financials\n  method: get\n  operationId: getFinancials\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fnd/stocks/{ticker}/financials/{concept}\n  method: get\n  operationId: getFinancialConcept\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fnd/stocks/{ticker}/insiders\n  method: get\n  operationId: listInsiders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fnd/stocks/{ticker}/ownership\n  method: get\n  operationId: listOwnership\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fnd/stocks/{ticker}/events\n  method: get\n  operationId: listEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n \
  \   subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fnd/stocks/{ticker}/compensation\n  method: get\n  operationId: listCompensation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/hist/stocks/{ticker}/bars\n  method: get\n  operationId: getStockBars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/siftingio/refs/heads/main/agentic-access/siftingio-agentic-access.yml
summary_line: 37 operations
tags:
- Financial market data
- Stocks/equities
- Forex
- Cryptocurrency
- DeFi/on-chain
- Commodities
- SEC filings
- XBRL
- Fundamentals
- Fintech
- Quant/trading infrastructure
- Real-time streaming
- WebSocket
- FIX
- financial data
- Market Data
- stocks
- DeFi
- Real-Time
- REST API
- MCP server
- agent-native
---
