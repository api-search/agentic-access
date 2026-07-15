---
acting_count: 0
action_class_counts:
  connected: 24
api_specs:
- filename: barchart-openapi.yml
  format: yaml
  label: Barchart Quotes API
  slug: barchart-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-openapi.yml
- filename: barchart-openapi.yml
  format: yaml
  label: Barchart History API
  slug: barchart-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-openapi.yml
- filename: barchart-openapi.yml
  format: yaml
  label: Barchart Reference & Equities API
  slug: barchart-reference-equities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-openapi.yml
- filename: barchart-openapi.yml
  format: yaml
  label: Barchart Futures & Options API
  slug: barchart-futures-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-openapi.yml
- filename: barchart-openapi.yml
  format: yaml
  label: Barchart Fundamentals API
  slug: barchart-fundamentals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-openapi.yml
- filename: barchart-openapi.yml
  format: yaml
  label: Barchart Corporate Actions & Earnings API
  slug: barchart-corporate-actions-earnings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-openapi.yml
- filename: barchart-openapi.yml
  format: yaml
  label: Barchart Cryptocurrency API
  slug: barchart-cryptocurrency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-openapi.yml
- filename: barchart-openapi.yml
  format: yaml
  label: Barchart Commodities & Agriculture API
  slug: barchart-commodities-agriculture-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-openapi.yml
- filename: barchart-openapi.yml
  format: yaml
  label: Barchart Technicals & Charts API
  slug: barchart-technicals-charts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-openapi.yml
- filename: barchart-openapi.yml
  format: yaml
  label: Barchart News & Filings API
  slug: barchart-news-filings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-openapi.yml
- filename: barchart-openapi.yml
  format: yaml
  label: Barchart Weather API
  slug: barchart-weather-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-openapi.yml
consequence_counts:
  read: 24
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Barchart Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 24
overview: 'Barchart exposes 24 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 24 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Barchart
provider_slug: barchart
slug: barchart-agentic-access
source_filename: barchart-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/barchart-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 24\n  by_action_class:\n    connected: 24\n  by_consequence:\n    read: 24\n  human_in_the_loop_required: 0\noperations:\n- path: /getQuote.json\n  method: get\n  operationId: getQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getQuoteEod.json\n  method: get\n  operationId: getQuoteEod\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getHistory.json\n  method: get\n  operationId: getHistory\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getEquitiesByExchange.json\n  method: get\n  operationId: getEquitiesByExchange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getInstrumentDefinition.json\n  method: get\n  operationId: getInstrumentDefinition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getFuturesOptions.json\n  method: get\n  operationId: getFuturesOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getFuturesByExchange.json\n  method: get\n  operationId: getFuturesByExchange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getOptionsScreener.json\n  method: get\n  operationId: getOptionsScreener\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getProfile.json\n  method: get\n  operationId: getProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getFinancialHighlights.json\n  method: get\n  operationId: getFinancialHighlights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getIncomeStatements.json\n  method: get\n  operationId: getIncomeStatements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getRatings.json\n\
  \  method: get\n  operationId: getRatings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getCorporateActions.json\n  method: get\n  operationId: getCorporateActions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getEarningsCalendar.json\n  method: get\n  operationId: getEarningsCalendar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getCrypto.json\n  method: get\n  operationId: getCrypto\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getCryptoHistory.json\n  method: get\n  operationId: getCryptoHistory\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getGrainBids.json\n  method: get\n  operationId: getGrainBids\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getCmdtyStats.json\n  method: get\n  operationId: getCmdtyStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getFuelPrices.json\n  method: get\n  operationId: getFuelPrices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getTechnicals.json\n  method: get\n  operationId: getTechnicals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getSignal.json\n  method: get\n\
  \  operationId: getSignal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getNews.json\n  method: get\n  operationId: getNews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getSECFilings.json\n  method: get\n  operationId: getSECFilings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getWeather.json\n  method: get\n  operationId: getWeather\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/agentic-access/barchart-agentic-access.yml
summary_line: 24 operations
tags:
- Market Data
- Financial Data
- Commodities
- Futures
- Options
- Reference Data
- Equities
- Historical Data
- Cryptocurrency
- Agriculture
---
