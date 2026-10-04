---
acting_count: 0
action_class_counts:
  connected: 3
api_specs:
- filename: agrio-balance-api-openapi.yml
  format: yaml
  label: agrio Balance API
  slug: agrio-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrio/refs/heads/main/openapi/agrio-balance-api-openapi.yml
- filename: agrio-crops-api-openapi.yml
  format: yaml
  label: agrio Crops API
  slug: agrio-crops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrio/refs/heads/main/openapi/agrio-crops-api-openapi.yml
- filename: agrio-diagnose-api-openapi.yml
  format: yaml
  label: agrio Diagnose API
  slug: agrio-diagnose-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrio/refs/heads/main/openapi/agrio-diagnose-api-openapi.yml
consequence_counts:
  read: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Agrio Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 3
overview: 'Agrio exposes 3 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Agrio
provider_slug: agrio
slug: agrio-agentic-access
source_filename: agrio-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/agrio-balance-api-openapi.yml, openapi/agrio-crops-api-openapi.yml, openapi/agrio-diagnose-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 3\n  by_action_class:\n    connected: 3\n  by_consequence:\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/get-credit\n  method: get\n  operationId: getCredit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get-supported-crops\n  method: get\n  operationId: getSupportedCrops\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/diagnose\n  method: post\n  operationId: getDiagnosis\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agrio/refs/heads/main/agentic-access/agrio-agentic-access.yml
summary_line: 3 operations
tags:
- Agriculture
- Plant Disease
- Pest Detection
- Artificial Intelligence
- Crop Advisory
---
