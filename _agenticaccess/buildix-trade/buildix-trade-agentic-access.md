---
acting_count: 0
action_class_counts:
  connected: 6
api_specs:
- filename: buildix-trade-deep-view-api-openapi.yml
  format: yaml
  label: Buildix Deep View API
  slug: buildix-trade-deep-view-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildix-trade/openapi/buildix-trade-deep-view-api-openapi.yml
- filename: buildix-trade-funding-arb-api-openapi.yml
  format: yaml
  label: Buildix Funding Arb API
  slug: buildix-trade-funding-arb-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildix-trade/openapi/buildix-trade-funding-arb-api-openapi.yml
- filename: buildix-trade-pair-api-openapi.yml
  format: yaml
  label: Buildix Pair API
  slug: buildix-trade-pair-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildix-trade/openapi/buildix-trade-pair-api-openapi.yml
- filename: buildix-trade-screener-api-openapi.yml
  format: yaml
  label: Buildix Screener API
  slug: buildix-trade-screener-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildix-trade/openapi/buildix-trade-screener-api-openapi.yml
- filename: buildix-trade-signals-api-openapi.yml
  format: yaml
  label: Buildix Signals API
  slug: buildix-trade-signals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildix-trade/openapi/buildix-trade-signals-api-openapi.yml
- filename: buildix-trade-smart-money-api-openapi.yml
  format: yaml
  label: Buildix Smart Money API
  slug: buildix-trade-smart-money-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildix-trade/openapi/buildix-trade-smart-money-api-openapi.yml
consequence_counts:
  read: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Buildix Trade Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Buildix exposes 6 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Buildix
provider_slug: buildix-trade
slug: buildix-trade-agentic-access
source_filename: buildix-trade-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/buildix-trade-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 6\n  by_consequence:\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /screener\n  method: get\n  operationId: getScreener\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /signals\n  method: get\n  operationId: getSignals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pair/{symbol}\n  method: get\n  operationId: getPair\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deep-view/{symbol}\n  method: get\n  operationId: getDeepView\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /smart-money\n  method: get\n  operationId: getSmartMoney\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /funding-arb\n  method: get\n  operationId: getFundingArb\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/buildix-trade/agentic-access/buildix-trade-agentic-access.yml
summary_line: 6 operations
tags:
- Company
- Cryptocurrency
- Analytics
- Orderflow
- Artificial Intelligence
---
