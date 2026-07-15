---
acting_count: 0
action_class_counts:
  connected: 5
api_specs:
- filename: edmunds-openapi.yml
  format: yaml
  label: Edmunds Dealership API
  slug: edmunds
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edmunds/refs/heads/main/openapi/edmunds-openapi.yml
- filename: edmunds-openapi.yml
  format: yaml
  label: Edmunds API
  slug: edmunds
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edmunds/refs/heads/main/openapi/edmunds-openapi.yml
consequence_counts:
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Edmunds Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Edmunds exposes 5 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Edmunds
provider_slug: edmunds
slug: edmunds-agentic-access
source_filename: edmunds-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/edmunds-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 5\n  by_consequence:\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /api/vehicle/v3/makes\n  method: get\n  operationId: listMakes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/vehicle/v3/makes/count\n  method: get\n  operationId: countMakes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/vehicle/v3/models\n  method: get\n  operationId:\
  \ listModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/vehicle/v2/makes\n  method: get\n  operationId: listMakesV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/vehicle/v2/{makeNiceName}/models\n  method: get\n  operationId: listModelsForMake\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/edmunds/refs/heads/main/agentic-access/edmunds-agentic-access.yml
summary_line: 5 operations
tags:
- Automobiles
- Cars
- Vehicles
---
