---
acting_count: 0
action_class_counts:
  connected: 6
api_specs:
- filename: damolive-com-health-api-openapi.yml
  format: yaml
  label: DAMO Health API
  slug: damolive-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/damolive-com/openapi/damolive-com-health-api-openapi.yml
- filename: damolive-com-market-state-api-openapi.yml
  format: yaml
  label: DAMO Market State API
  slug: damolive-com-market-state-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/damolive-com/openapi/damolive-com-market-state-api-openapi.yml
- filename: damolive-com-states-api-openapi.yml
  format: yaml
  label: DAMO States API
  slug: damolive-com-states-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/damolive-com/openapi/damolive-com-states-api-openapi.yml
- filename: damolive-com-symbols-api-openapi.yml
  format: yaml
  label: DAMO Symbols API
  slug: damolive-com-symbols-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/damolive-com/openapi/damolive-com-symbols-api-openapi.yml
- filename: damolive-com-well-known-api-openapi.yml
  format: yaml
  label: DAMO .well Known API
  slug: damolive-com-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/damolive-com/openapi/damolive-com-well-known-api-openapi.yml
consequence_counts:
  read: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Damolive Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'DAMO exposes 6 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: DAMO
provider_slug: damolive-com
slug: damolive-com-agentic-access
source_filename: damolive-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/damolive-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 6\n  by_consequence:\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/symbols\n  method: get\n  operationId: listSymbols\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/market-state/{symbol}\n  method: get\n  operationId: getMarketState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/market-state\n  method: get\n  operationId: getMarketStates\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/states\n  method: get\n  operationId: getStateDefinitions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/damo-keys.json\n  method: get\n  operationId: getSigningKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/damolive-com/agentic-access/damolive-com-agentic-access.yml
summary_line: 6 operations
tags:
- Finance
- Market Data
- Artificial Intelligence
- Analytics
- Trading
---
