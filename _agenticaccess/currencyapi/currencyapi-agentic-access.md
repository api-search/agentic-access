---
acting_count: 0
action_class_counts:
  connected: 6
api_specs:
- filename: currencyapi-openapi.yml
  format: yaml
  label: CurrencyAPI Latest Exchange Rates API
  slug: currencyapi-latest-exchange-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/currencyapi/refs/heads/main/openapi/currencyapi-openapi.yml
- filename: currencyapi-openapi.yml
  format: yaml
  label: CurrencyAPI Historical Exchange Rates API
  slug: currencyapi-historical-exchange-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/currencyapi/refs/heads/main/openapi/currencyapi-openapi.yml
- filename: currencyapi-openapi.yml
  format: yaml
  label: CurrencyAPI Range Exchange Rates API
  slug: currencyapi-range-exchange-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/currencyapi/refs/heads/main/openapi/currencyapi-openapi.yml
- filename: currencyapi-openapi.yml
  format: yaml
  label: CurrencyAPI Convert API
  slug: currencyapi-convert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/currencyapi/refs/heads/main/openapi/currencyapi-openapi.yml
- filename: currencyapi-openapi.yml
  format: yaml
  label: CurrencyAPI Currencies API
  slug: currencyapi-currencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/currencyapi/refs/heads/main/openapi/currencyapi-openapi.yml
- filename: currencyapi-openapi.yml
  format: yaml
  label: CurrencyAPI Status API
  slug: currencyapi-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/currencyapi/refs/heads/main/openapi/currencyapi-openapi.yml
consequence_counts:
  read: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Currencyapi Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'CurrencyAPI exposes 6 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CurrencyAPI
provider_slug: currencyapi
slug: currencyapi-agentic-access
source_filename: currencyapi-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/currencyapi-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 6\n  by_consequence:\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /latest\n  method: get\n  operationId: getLatestExchangeRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /historical\n  method: get\n  operationId: getHistoricalExchangeRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /range\n  method: get\n  operationId: getRangeExchangeRates\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /convert\n  method: get\n  operationId: convertCurrency\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /currencies\n  method: get\n  operationId: listCurrencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/currencyapi/refs/heads/main/agentic-access/currencyapi-agentic-access.yml
summary_line: 6 operations
tags:
- Foreign Exchange
- Currency
- Exchange Rates
- FX
- Currency Conversion
- Financial Data
---
