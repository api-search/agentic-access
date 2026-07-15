---
acting_count: 0
action_class_counts:
  connected: 7
api_specs:
- filename: granular-farm-management-openapi.yml
  format: yaml
  label: Granular Farm Management API
  slug: granular-farm-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/granular/refs/heads/main/openapi/granular-farm-management-openapi.yml
consequence_counts:
  read: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Granular Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Granular (Corteva Agriscience) exposes 7 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Granular (Corteva Agriscience)
provider_slug: granular
slug: granular-agentic-access
source_filename: granular-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/granular-farm-management-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 7\n  by_consequence:\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /farms\n  method: get\n  operationId: listFarms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n    - write\n- path: /farms/{farmId}\n  method: get\n  operationId: getFarm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n    - write\n\
  - path: /farms/{farmId}/fields\n  method: get\n  operationId: listFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n    - write\n- path: /fields/{fieldId}\n  method: get\n  operationId: getField\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n    - write\n- path: /fields/{fieldId}/activities\n  method: get\n  operationId: listFieldActivities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n    - write\n- path: /crop-plans\n  method: get\n  operationId: listCropPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n\
  \    - read\n    - write\n- path: /financials/summary\n  method: get\n  operationId: getFinancialSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n    - write\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/granular/refs/heads/main/agentic-access/granular-agentic-access.yml
summary_line: 7 operations
tags:
- Agriculture
- Farm Management
- Financial
- Crop Planning
- Agronomy
---
