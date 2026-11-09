---
acting_count: 0
action_class_counts:
  connected: 7
api_specs:
- filename: lotsofsounds-com-samples-api-openapi.yml
  format: yaml
  label: lotsofsounds-com Samples API
  slug: lotsofsounds-com-samples-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lotsofsounds-com/openapi/lotsofsounds-com-samples-api-openapi.yml
- filename: lotsofsounds-com-sounds-api-openapi.yml
  format: yaml
  label: lotsofsounds-com Sounds API
  slug: lotsofsounds-com-sounds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lotsofsounds-com/openapi/lotsofsounds-com-sounds-api-openapi.yml
consequence_counts:
  read: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Lotsofsounds Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'lotsofsounds-com exposes 7 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: lotsofsounds-com
provider_slug: lotsofsounds-com
slug: lotsofsounds-com-agentic-access
source_filename: lotsofsounds-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/lotsofsounds-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 7\n  by_consequence:\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/sounds/sample\n  method: get\n  operationId: listSampleSounds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sounds/sample/{id}/stream\n  method: get\n  operationId: streamSampleSound\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sounds\n  method:\
  \ get\n  operationId: searchSounds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sounds/popular\n  method: get\n  operationId: listPopularSounds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sounds/{id}\n  method: get\n  operationId: getSound\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sounds/{id}/stream\n  method: get\n  operationId: streamSound\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sounds/{id}/download\n  method: get\n  operationId: downloadSound\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/lotsofsounds-com/agentic-access/lotsofsounds-com-agentic-access.yml
summary_line: 7 operations
tags:
- Company
- Audio
- Free
- CC0
---
