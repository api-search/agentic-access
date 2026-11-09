---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 3
api_specs:
- filename: centeringlab-com-grade-api-openapi.yml
  format: yaml
  label: Centering Lab Grade API
  slug: centeringlab-com-grade-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/centeringlab-com/openapi/centeringlab-com-grade-api-openapi.yml
- filename: centeringlab-com-health-api-openapi.yml
  format: yaml
  label: Centering Lab Health API
  slug: centeringlab-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/centeringlab-com/openapi/centeringlab-com-health-api-openapi.yml
- filename: centeringlab-com-measure-api-openapi.yml
  format: yaml
  label: Centering Lab Measure API
  slug: centeringlab-com-measure-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/centeringlab-com/openapi/centeringlab-com-measure-api-openapi.yml
- filename: centeringlab-com-openapi-json-api-openapi.yml
  format: yaml
  label: Centering Lab Openapi.json API
  slug: centeringlab-com-openapi-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/centeringlab-com/openapi/centeringlab-com-openapi-json-api-openapi.yml
- filename: centeringlab-com-standards-api-openapi.yml
  format: yaml
  label: Centering Lab Standards API
  slug: centeringlab-com-standards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/centeringlab-com/openapi/centeringlab-com-standards-api-openapi.yml
consequence_counts:
  read: 3
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Centeringlab Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Centering Lab exposes 6 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Centering Lab
provider_slug: centeringlab-com
slug: centeringlab-com-agentic-access
source_filename: centeringlab-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/centeringlab-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    acting: 3\n    connected: 3\n  by_consequence:\n    write: 3\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/grade\n  method: post\n  operationId: grade_centering\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/standards\n  method: get\n  operationId: get_centering_standards\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/measure\n  method: post\n  operationId: measure_card_centering\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/measure/confirm\n  method: post\n  operationId: confirm_card_centering\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/health\n  method: get\n  operationId: get_api_health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/openapi.json\n  method: get\n  operationId: get_openapi_schema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/centeringlab-com/agentic-access/centeringlab-com-agentic-access.yml
summary_line: 6 operations · 3 acting
tags:
- Cards
- Centering
- Collectors
- Web App
---
