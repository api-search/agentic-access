---
acting_count: 0
action_class_counts:
  connected: 37
api_specs:
- filename: tiingo-openapi.yml
  format: yaml
  label: Tiingo End-of-Day API
  slug: end-of-day-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiingo/refs/heads/main/openapi/tiingo-openapi.yml
- filename: tiingo-openapi.yml
  format: yaml
  label: Tiingo IEX Intraday API
  slug: iex-intraday-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiingo/refs/heads/main/openapi/tiingo-openapi.yml
- filename: tiingo-openapi.yml
  format: yaml
  label: Tiingo Crypto API
  slug: crypto-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiingo/refs/heads/main/openapi/tiingo-openapi.yml
- filename: tiingo-openapi.yml
  format: yaml
  label: Tiingo Forex API
  slug: forex-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiingo/refs/heads/main/openapi/tiingo-openapi.yml
- filename: tiingo-openapi.yml
  format: yaml
  label: Tiingo Fundamentals API
  slug: fundamentals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiingo/refs/heads/main/openapi/tiingo-openapi.yml
- filename: tiingo-openapi.yml
  format: yaml
  label: Tiingo News API
  slug: news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiingo/refs/heads/main/openapi/tiingo-openapi.yml
consequence_counts:
  read: 37
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tiingo Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 37
overview: 'Tiingo exposes 37 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 37 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Tiingo
provider_slug: tiingo
slug: tiingo-agentic-access
source_filename: tiingo-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: generated\nsource: openapi/tiingo-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 37\n  by_action_class:\n    connected: 37\n  by_consequence:\n    read: 37\n  human_in_the_loop_required: 0\noperations:\n- path: /tiingo/daily/{ticker}\n  method: get\n  operationId: getDailyMeta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tiingo/daily/{ticker}/prices\n  method: get\n  operationId: getDailyPrices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tiingo/corporate-actions/{ticker}/distribution-yield\n\
  \  method: get\n  operationId: getDistributionYield\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tiingo/corporate-actions/{ticker}/distributions\n  method: get\n  operationId: getTickerDistributions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tiingo/corporate-actions/distributions\n  method: get\n  operationId: getBulkDistributions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tiingo/corporate-actions/{ticker}/splits\n  method: get\n  operationId: getTickerSplits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tiingo/corporate-actions/splits\n  method:\
  \ get\n  operationId: getBulkSplits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tiingo/news\n  method: get\n  operationId: listNews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tiingo/news/bulk_download\n  method: get\n  operationId: listNewsBulkFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tiingo/news/bulk_download/{id}\n  method: get\n  operationId: downloadNewsBulkFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tiingo/crypto\n  method: get\n  operationId: listCryptoMeta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tiingo/crypto/top\n  method: get\n  operationId: getCryptoTopOfBook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tiingo/crypto/prices\n  method: get\n  operationId: getCryptoPrices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tiingo/crypto-yield/platforms\n  method: get\n  operationId: listCryptoYieldPlatforms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tiingo/crypto-yield/pools\n  method: get\n  operationId: listCryptoYieldPools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /tiingo/crypto-yield/ticks\n  method: get\n  operationId: getCryptoYieldTicks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tiingo/crypto-yield/{poolCode}/metrics\n  method: get\n  operationId: getCryptoYieldMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iex\n  method: get\n  operationId: getIexTopOfBook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iex/{ticker}/prices\n  method: get\n  operationId: getIexHistoricalPrices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /boats\n  method: get\n  operationId: getBoatsTopOfBook\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /boats/{ticker}/prices\n  method: get\n  operationId: getBoatsHistoricalPrices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tiingo/equity/intraday\n  method: get\n  operationId: getEquityRealtimeTopOfBook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tiingo/equity/intraday/{ticker}/prices\n  method: get\n  operationId: getEquityRealtimeHistoricalPrices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /smallx/meta\n  method: get\n  operationId: getSmallXMeta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /smallx/tops\n  method: get\n  operationId: getSmallXTopOfBook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /smallx/{ticker}/prices\n  method: get\n  operationId: getSmallXIntradayPrices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /smallx/{ticker}/eod\n  method: get\n  operationId: getSmallXEodPrices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tiingo/fx/top\n  method: get\n  operationId: getForexTopOfBook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tiingo/fx/{ticker}/prices\n\
  \  method: get\n  operationId: getForexPrices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tiingo/fundamentals/definitions\n  method: get\n  operationId: getFundamentalsDefinitions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tiingo/fundamentals/meta\n  method: get\n  operationId: getFundamentalsMeta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tiingo/fundamentals/{ticker}/statements\n  method: get\n  operationId: getFundamentalsStatements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tiingo/fundamentals/{ticker}/daily\n  method: get\n  operationId: getFundamentalsDaily\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tiingo/funds/{ticker}\n  method: get\n  operationId: getFundFees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tiingo/funds/{ticker}/metrics\n  method: get\n  operationId: getFundFeeMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tiingo/utilities/search\n  method: get\n  operationId: searchAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/test\n  method: get\n  operationId: testConnection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tiingo/refs/heads/main/agentic-access/tiingo-agentic-access.yml
summary_line: 37 operations
tags:
- Fintech
- Market Data
- Stocks
- Crypto
- FX
- News
- Fundamentals
- WebSockets
---
