---
acting_count: 0
action_class_counts:
  connected: 7
api_specs:
- filename: k-agentpay-com-airport-api-openapi.yml
  format: yaml
  label: k-agentpay-com Airport API
  slug: k-agentpay-com-airport-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/k-agentpay-com/openapi/k-agentpay-com-airport-api-openapi.yml
- filename: k-agentpay-com-kpop-api-openapi.yml
  format: yaml
  label: k-agentpay-com Kpop API
  slug: k-agentpay-com-kpop-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/k-agentpay-com/openapi/k-agentpay-com-kpop-api-openapi.yml
- filename: k-agentpay-com-seoul-api-openapi.yml
  format: yaml
  label: k-agentpay-com Seoul API
  slug: k-agentpay-com-seoul-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/k-agentpay-com/openapi/k-agentpay-com-seoul-api-openapi.yml
consequence_counts:
  read: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: K Agentpay Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'k-agentpay-com exposes 7 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: k-agentpay-com
provider_slug: k-agentpay-com
slug: k-agentpay-com-agentic-access
source_filename: k-agentpay-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/k-agentpay-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 7\n  by_consequence:\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/kpop/search\n  method: get\n  operationId: kpopSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/seoul/trip-pack\n  method: get\n  operationId: seoulTripPack\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/kpop/new\n  method: get\n  operationId: kpopNew\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/seoul/now\n  method: get\n  operationId: seoulNow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/seoul/subway\n  method: get\n  operationId: seoulSubway\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/airport/icn\n  method: get\n  operationId: airportIcn\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/seoul/places\n  method: get\n  operationId: seoulPlaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/k-agentpay-com/agentic-access/k-agentpay-com-agentic-access.yml
summary_line: 7 operations
tags:
- Company
- Travel
- K-Pop
- Data
- South Korea
---
