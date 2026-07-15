---
acting_count: 0
action_class_counts:
  connected: 7
api_specs:
- filename: openexchangerates-openapi.yml
  format: yaml
  label: Open Exchange Rates Latest Rates API
  slug: openexchangerates-latest-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openexchangerates/refs/heads/main/openapi/openexchangerates-openapi.yml
- filename: openexchangerates-openapi.yml
  format: yaml
  label: Open Exchange Rates Historical Rates API
  slug: openexchangerates-historical-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openexchangerates/refs/heads/main/openapi/openexchangerates-openapi.yml
- filename: openexchangerates-openapi.yml
  format: yaml
  label: Open Exchange Rates Time Series API
  slug: openexchangerates-time-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openexchangerates/refs/heads/main/openapi/openexchangerates-openapi.yml
- filename: openexchangerates-openapi.yml
  format: yaml
  label: Open Exchange Rates Convert API
  slug: openexchangerates-convert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openexchangerates/refs/heads/main/openapi/openexchangerates-openapi.yml
- filename: openexchangerates-openapi.yml
  format: yaml
  label: Open Exchange Rates Currencies API
  slug: openexchangerates-currencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openexchangerates/refs/heads/main/openapi/openexchangerates-openapi.yml
- filename: openexchangerates-openapi.yml
  format: yaml
  label: Open Exchange Rates OHLC API
  slug: openexchangerates-ohlc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openexchangerates/refs/heads/main/openapi/openexchangerates-openapi.yml
- filename: openexchangerates-openapi.yml
  format: yaml
  label: Open Exchange Rates Usage API
  slug: openexchangerates-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openexchangerates/refs/heads/main/openapi/openexchangerates-openapi.yml
consequence_counts:
  read: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Openexchangerates Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Open Exchange Rates exposes 7 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Open Exchange Rates
provider_slug: openexchangerates
slug: openexchangerates-agentic-access
source_filename: openexchangerates-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openexchangerates-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 7\n  by_consequence:\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /latest.json\n  method: get\n  operationId: getLatestRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /historical/{date}.json\n  method: get\n  operationId: getHistoricalRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /time-series.json\n  method: get\n  operationId:\
  \ getTimeSeries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /convert/{value}/{from}/{to}\n  method: get\n  operationId: convertCurrency\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /currencies.json\n  method: get\n  operationId: getCurrencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ohlc.json\n  method: get\n  operationId: getOhlc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /usage.json\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openexchangerates/refs/heads/main/agentic-access/openexchangerates-agentic-access.yml
summary_line: 7 operations
tags:
- Foreign Exchange
- Currency
- Exchange Rates
- FX
- Currency Conversion
- Forex
- Financial Data
---
