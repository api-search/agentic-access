---
acting_count: 0
action_class_counts:
  connected: 9
api_specs:
- filename: exchangerate-api-openapi.yml
  format: yaml
  label: ExchangeRate-API Latest Rates API
  slug: latest-rates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exchangerate-api/refs/heads/main/openapi/exchangerate-api-openapi.yml
- filename: exchangerate-api-openapi.yml
  format: yaml
  label: ExchangeRate-API Pair Conversion API
  slug: pair-conversion
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exchangerate-api/refs/heads/main/openapi/exchangerate-api-openapi.yml
- filename: exchangerate-api-openapi.yml
  format: yaml
  label: ExchangeRate-API Enriched Data API
  slug: enriched-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exchangerate-api/refs/heads/main/openapi/exchangerate-api-openapi.yml
- filename: exchangerate-api-openapi.yml
  format: yaml
  label: ExchangeRate-API Historical Rates API
  slug: historical-rates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exchangerate-api/refs/heads/main/openapi/exchangerate-api-openapi.yml
- filename: exchangerate-api-openapi.yml
  format: yaml
  label: ExchangeRate-API Supported Codes API
  slug: supported-codes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exchangerate-api/refs/heads/main/openapi/exchangerate-api-openapi.yml
- filename: exchangerate-api-openapi.yml
  format: yaml
  label: ExchangeRate-API Quota API
  slug: quota
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exchangerate-api/refs/heads/main/openapi/exchangerate-api-openapi.yml
- filename: exchangerate-api-openapi.yml
  format: yaml
  label: ExchangeRate-API Open Access API
  slug: open-access
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exchangerate-api/refs/heads/main/openapi/exchangerate-api-openapi.yml
consequence_counts:
  read: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Exchangerate Api Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'ExchangeRate-API exposes 9 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ExchangeRate-API
provider_slug: exchangerate-api
slug: exchangerate-api-agentic-access
source_filename: exchangerate-api-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/exchangerate-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 9\n  by_consequence:\n    read: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /{api_key}/latest/{base_code}\n  method: get\n  operationId: getLatestRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{api_key}/pair/{base_code}/{target_code}\n  method: get\n  operationId: getPairConversion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{api_key}/pair/{base_code}/{target_code}/{amount}\n\
  \  method: get\n  operationId: getPairConversionWithAmount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{api_key}/enriched/{base_code}/{target_code}\n  method: get\n  operationId: getEnrichedPair\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{api_key}/history/{base_code}/{year}/{month}/{day}\n  method: get\n  operationId: getHistoricalRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{api_key}/history/{base_code}/{year}/{month}/{day}/{amount}\n  method: get\n  operationId: getHistoricalRatesWithAmount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{api_key}/codes\n\
  \  method: get\n  operationId: getSupportedCodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{api_key}/quota\n  method: get\n  operationId: getQuota\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /latest/{base_code}\n  method: get\n  operationId: getOpenAccessLatest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exchangerate-api/refs/heads/main/agentic-access/exchangerate-api-agentic-access.yml
summary_line: 9 operations
tags:
- Currency Exchange
- Foreign Exchange
- Financial Data
- Forex
- Currency Conversion
- Public APIs
---
