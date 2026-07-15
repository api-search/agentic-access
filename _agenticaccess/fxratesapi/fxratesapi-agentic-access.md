---
acting_count: 0
action_class_counts:
  connected: 5
api_specs:
- filename: fxratesapi-openapi.yml
  format: yaml
  label: FXRatesAPI Latest Rates API
  slug: fxratesapi-latest-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fxratesapi/refs/heads/main/openapi/fxratesapi-openapi.yml
- filename: fxratesapi-openapi.yml
  format: yaml
  label: FXRatesAPI Historical Rates API
  slug: fxratesapi-historical-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fxratesapi/refs/heads/main/openapi/fxratesapi-openapi.yml
- filename: fxratesapi-openapi.yml
  format: yaml
  label: FXRatesAPI Time-Series API
  slug: fxratesapi-time-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fxratesapi/refs/heads/main/openapi/fxratesapi-openapi.yml
- filename: fxratesapi-openapi.yml
  format: yaml
  label: FXRatesAPI Convert API
  slug: fxratesapi-convert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fxratesapi/refs/heads/main/openapi/fxratesapi-openapi.yml
- filename: fxratesapi-openapi.yml
  format: yaml
  label: FXRatesAPI Currencies API
  slug: fxratesapi-currencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fxratesapi/refs/heads/main/openapi/fxratesapi-openapi.yml
consequence_counts:
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Fxratesapi Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'FXRatesAPI exposes 5 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: FXRatesAPI
provider_slug: fxratesapi
slug: fxratesapi-agentic-access
source_filename: fxratesapi-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/fxratesapi-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 5\n  by_consequence:\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /latest\n  method: get\n  operationId: getLatestRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /historical\n  method: get\n  operationId: getHistoricalRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /timeseries\n  method: get\n  operationId: getTimeSeriesRates\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /convert\n  method: get\n  operationId: convertCurrency\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /currencies\n  method: get\n  operationId: listCurrencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fxratesapi/refs/heads/main/agentic-access/fxratesapi-agentic-access.yml
summary_line: 5 operations
tags:
- Foreign Exchange
- FX
- Currency
- Exchange Rates
- Forex
- Currency Conversion
- Historical Rates
- Financial Data
- Cryptocurrencies
---
