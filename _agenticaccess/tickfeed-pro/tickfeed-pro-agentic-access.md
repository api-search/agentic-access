---
acting_count: 0
action_class_counts:
  connected: 22
api_specs:
- filename: tickfeed-pro-account-api-openapi.yml
  format: yaml
  label: tickfeed-pro Account API
  slug: tickfeed-pro-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickfeed-pro/openapi/tickfeed-pro-account-api-openapi.yml
- filename: tickfeed-pro-market-data-api-openapi.yml
  format: yaml
  label: tickfeed-pro market data API
  slug: tickfeed-pro-market-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickfeed-pro/openapi/tickfeed-pro-market-data-api-openapi.yml
- filename: tickfeed-pro-system-api-openapi.yml
  format: yaml
  label: tickfeed-pro System API
  slug: tickfeed-pro-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickfeed-pro/openapi/tickfeed-pro-system-api-openapi.yml
consequence_counts:
  read: 22
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tickfeed Pro Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 22
overview: 'tickfeed-pro exposes 22 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: tickfeed-pro
provider_slug: tickfeed-pro
slug: tickfeed-pro-agentic-access
source_filename: tickfeed-pro-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/api.tickfeed.pro-openapi.json, openapi/tickfeed-pro-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 22\n  by_consequence:\n    read: 22\n  human_in_the_loop_required: 0\noperations:\n- path: /health\n  method: get\n  operationId: health_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status\n  method: get\n  operationId: status_status_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status.json\n  method:\
  \ get\n  operationId: status_json_status_json_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pricing\n  method: get\n  operationId: public_pricing_pricing_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/usage\n  method: get\n  operationId: usage_v1_usage_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/symbols\n  method: get\n  operationId: list_symbols_v1_symbols_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/price/{symbol}\n  method: get\n  operationId: get_price_v1_price__symbol__get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/prices\n  method: get\n  operationId: get_prices_v1_prices_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/candles/{symbol}\n  method: get\n  operationId: get_candles_v1_candles__symbol__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ticks/{symbol}\n  method: get\n  operationId: get_ticks_v1_ticks__symbol__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/candles/{symbol}/gaps\n  method: get\n  operationId: get_gaps_v1_candles__symbol__gaps_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: health_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status\n  method: get\n  operationId: status_status_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status.json\n  method: get\n  operationId: status_json_status_json_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pricing\n  method: get\n  operationId: public_pricing_pricing_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/usage\n  method: get\n  operationId: usage_v1_usage_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/symbols\n  method: get\n  operationId: list_symbols_v1_symbols_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/price/{symbol}\n  method: get\n  operationId: get_price_v1_price__symbol__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/prices\n  method: get\n  operationId: get_prices_v1_prices_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/candles/{symbol}\n  method: get\n  operationId: get_candles_v1_candles__symbol__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ticks/{symbol}\n  method: get\n  operationId: get_ticks_v1_ticks__symbol__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/candles/{symbol}/gaps\n  method: get\n  operationId: get_gaps_v1_candles__symbol__gaps_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/tickfeed-pro/agentic-access/tickfeed-pro-agentic-access.yml
summary_line: 22 operations
tags:
- Company
- Finance
- Market Data
- Foreign Exchange
- Gold
- MCP
---
