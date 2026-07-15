---
acting_count: 0
action_class_counts:
  connected: 16
api_specs:
- filename: financialmodelingprep-openapi.yml
  format: yaml
  label: Financial Modeling Prep Financial Statements API
  slug: financialmodelingprep-financial-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/financialmodelingprep/refs/heads/main/openapi/financialmodelingprep-openapi.yml
- filename: financialmodelingprep-openapi.yml
  format: yaml
  label: Financial Modeling Prep Quotes and Prices API
  slug: financialmodelingprep-quotes-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/financialmodelingprep/refs/heads/main/openapi/financialmodelingprep-openapi.yml
- filename: financialmodelingprep-openapi.yml
  format: yaml
  label: Financial Modeling Prep SEC Filings API
  slug: financialmodelingprep-sec-filings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/financialmodelingprep/refs/heads/main/openapi/financialmodelingprep-openapi.yml
- filename: financialmodelingprep-openapi.yml
  format: yaml
  label: Financial Modeling Prep Fundamentals API
  slug: financialmodelingprep-fundamentals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/financialmodelingprep/refs/heads/main/openapi/financialmodelingprep-openapi.yml
- filename: financialmodelingprep-openapi.yml
  format: yaml
  label: Financial Modeling Prep Analyst Estimates API
  slug: financialmodelingprep-analyst-estimates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/financialmodelingprep/refs/heads/main/openapi/financialmodelingprep-openapi.yml
- filename: financialmodelingprep-openapi.yml
  format: yaml
  label: Financial Modeling Prep Economic Data API
  slug: financialmodelingprep-economic-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/financialmodelingprep/refs/heads/main/openapi/financialmodelingprep-openapi.yml
- filename: financialmodelingprep-asyncapi.yml
  format: yaml
  label: Financial Modeling Prep Real-Time WebSocket API
  slug: financialmodelingprep-realtime-websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/financialmodelingprep/refs/heads/main/asyncapi/financialmodelingprep-asyncapi.yml
consequence_counts:
  read: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Financialmodelingprep Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'Financial Modeling Prep exposes 16 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Financial Modeling Prep
provider_slug: financialmodelingprep
slug: financialmodelingprep-agentic-access
source_filename: financialmodelingprep-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/financialmodelingprep-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 16\n  by_consequence:\n    read: 16\n  human_in_the_loop_required: 0\noperations:\n- path: /income-statement\n  method: get\n  operationId: getIncomeStatement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /balance-sheet-statement\n  method: get\n  operationId: getBalanceSheetStatement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cash-flow-statement\n\
  \  method: get\n  operationId: getCashFlowStatement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /quote\n  method: get\n  operationId: getQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /historical-price-eod/full\n  method: get\n  operationId: getHistoricalPriceEodFull\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sec-filings-search/symbol\n  method: get\n  operationId: getSecFilingsBySymbol\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sec-filings-search/cik\n  method: get\n  operationId: getSecFilingsByCik\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /financials-latest\n  method: get\n  operationId: getLatestFinancialFilings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile\n  method: get\n  operationId: getCompanyProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /key-metrics\n  method: get\n  operationId: getKeyMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ratios\n  method: get\n  operationId: getFinancialRatios\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analyst-estimates\n  method:\
  \ get\n  operationId: getAnalystEstimates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /financial-estimates\n  method: get\n  operationId: getFinancialEstimates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /economic-indicators\n  method: get\n  operationId: getEconomicIndicators\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /treasury-rates\n  method: get\n  operationId: getTreasuryRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /economic-calendar\n  method: get\n  operationId: getEconomicCalendar\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/financialmodelingprep/refs/heads/main/agentic-access/financialmodelingprep-agentic-access.yml
summary_line: 16 operations
tags:
- Financial Data
- Market Data
- Fundamentals
- SEC Filings
- Stocks
- Economic Indicators
- Quotes
- Regulatory Filings
---
