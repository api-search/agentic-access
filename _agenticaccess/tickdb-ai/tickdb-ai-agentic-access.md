---
acting_count: 0
action_class_counts:
  connected: 46
api_specs:
- filename: tickdb-ai-account-api-openapi.yml
  format: yaml
  label: tickdb-ai Account API
  slug: tickdb-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickdb-ai/openapi/tickdb-ai-account-api-openapi.yml
- filename: tickdb-ai-fundamentals-capital-actions-api-openapi.yml
  format: yaml
  label: tickdb-ai Fundamentals Capital Actions API
  slug: tickdb-ai-fundamentals-capital-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickdb-ai/openapi/tickdb-ai-fundamentals-capital-actions-api-openapi.yml
- filename: tickdb-ai-fundamentals-company-api-openapi.yml
  format: yaml
  label: tickdb-ai Fundamentals Company API
  slug: tickdb-ai-fundamentals-company-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickdb-ai/openapi/tickdb-ai-fundamentals-company-api-openapi.yml
- filename: tickdb-ai-fundamentals-events-api-openapi.yml
  format: yaml
  label: tickdb-ai Fundamentals Events API
  slug: tickdb-ai-fundamentals-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickdb-ai/openapi/tickdb-ai-fundamentals-events-api-openapi.yml
- filename: tickdb-ai-fundamentals-financials-api-openapi.yml
  format: yaml
  label: tickdb-ai Fundamentals Financials API
  slug: tickdb-ai-fundamentals-financials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickdb-ai/openapi/tickdb-ai-fundamentals-financials-api-openapi.yml
- filename: tickdb-ai-fundamentals-holders-api-openapi.yml
  format: yaml
  label: tickdb-ai Fundamentals Holders API
  slug: tickdb-ai-fundamentals-holders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickdb-ai/openapi/tickdb-ai-fundamentals-holders-api-openapi.yml
- filename: tickdb-ai-fundamentals-valuation-industry-api-openapi.yml
  format: yaml
  label: tickdb-ai Fundamentals Valuation Industry API
  slug: tickdb-ai-fundamentals-valuation-industry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickdb-ai/openapi/tickdb-ai-fundamentals-valuation-industry-api-openapi.yml
- filename: tickdb-ai-market-api-openapi.yml
  format: yaml
  label: tickdb-ai Market API
  slug: tickdb-ai-market-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickdb-ai/openapi/tickdb-ai-market-api-openapi.yml
- filename: tickdb-ai-symbols-api-openapi.yml
  format: yaml
  label: tickdb-ai Symbols API
  slug: tickdb-ai-symbols-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickdb-ai/openapi/tickdb-ai-symbols-api-openapi.yml
consequence_counts:
  read: 46
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tickdb Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 46
overview: 'tickdb-ai exposes 46 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 46 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: tickdb-ai
provider_slug: tickdb-ai
slug: tickdb-ai-agentic-access
source_filename: tickdb-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/tickdb-ai-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 46\n  by_action_class:\n    connected: 46\n  by_consequence:\n    read: 46\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/apikeys/subscriptions\n  method: get\n  operationId: getAPIKeyStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/market/ticker\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/market/ticker/cn-stock\n  method: get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/market/ticker/hk-stock\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/market/ticker/us-stock\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/market/kline\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/market/depth\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/market/trades\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/symbols/available\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/market/kline/latest\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/market/kline/ex-factors\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/market/intraday\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/market/trading-sessions\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /v1/market/trade-days\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/market/stock-info\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/market/calc-index\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/market/capital-flow\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fundamentals/profile\n  method: get\n  operationId: getFundamentalsProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/fundamentals/executives\n  method: get\n  operationId: getFundamentalsExecutives\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fundamentals/financials/latest\n  method: get\n  operationId: getFundamentalsFinancialsLatest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fundamentals/financials/annual\n  method: get\n  operationId: getFundamentalsFinancialsAnnual\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fundamentals/financials/ttm\n  method: get\n  operationId: getFundamentalsFinancialsTTM\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n- path: /v1/fundamentals/segments/latest\n  method: get\n  operationId: getFundamentalsSegmentsLatest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fundamentals/segments/history\n  method: get\n  operationId: getFundamentalsSegmentsHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fundamentals/valuation/latest\n  method: get\n  operationId: getFundamentalsValuationLatest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fundamentals/valuation/ts\n  method: get\n  operationId: getFundamentalsValuationTimeSeries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /v1/fundamentals/industry/peers\n  method: get\n  operationId: getFundamentalsIndustryPeers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fundamentals/industry/dist\n  method: get\n  operationId: getFundamentalsIndustryDistribution\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fundamentals/industries/rank\n  method: get\n  operationId: getFundamentalsIndustriesRank\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fundamentals/industries/tree\n  method: get\n  operationId: getFundamentalsIndustriesTree\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /v1/fundamentals/dividends\n  method: get\n  operationId: getFundamentalsDividends\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fundamentals/dividends/ttm\n  method: get\n  operationId: getFundamentalsDividendsTTM\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fundamentals/buyback\n  method: get\n  operationId: getFundamentalsBuyback\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fundamentals/shareholders/latest\n  method: get\n  operationId: getFundamentalsShareholdersLatest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/fundamentals/shareholders/top\n  method: get\n  operationId: getFundamentalsShareholdersTop\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fundamentals/shareholders/detail\n  method: get\n  operationId: getFundamentalsShareholderDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fundamentals/fund-holdings/latest\n  method: get\n  operationId: getFundamentalsFundHoldingsLatest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fundamentals/corp-actions\n  method: get\n  operationId: getFundamentalsCorporateActions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/fundamentals/news\n  method: get\n  operationId: getFundamentalsNews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fundamentals/news/{news_id}\n  method: get\n  operationId: getFundamentalsNewsDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fundamentals/calendar/report\n  method: get\n  operationId: getFundamentalsCalendarReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fundamentals/calendar/dividend\n  method: get\n  operationId: getFundamentalsCalendarDividend\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/fundamentals/calendar/split\n  method: get\n  operationId: getFundamentalsCalendarSplit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fundamentals/calendar/ipo\n  method: get\n  operationId: getFundamentalsCalendarIPO\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fundamentals/calendar/other\n  method: get\n  operationId: getFundamentalsCalendarOther\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fundamentals/market/status\n  method: get\n  operationId: getFundamentalsMarketStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/tickdb-ai/agentic-access/tickdb-ai-agentic-access.yml
summary_line: 46 operations
tags:
- Company
- Finance
- Market Data
- Real-Time
---
