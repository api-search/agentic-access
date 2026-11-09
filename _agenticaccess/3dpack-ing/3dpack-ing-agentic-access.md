---
acting_count: 6
action_class_counts:
  acting: 6
api_specs:
- filename: 3dpack-ing-packing-api-openapi.yml
  format: yaml
  label: 3dpack-ing Packing API
  slug: 3dpack-ing-packing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/3dpack-ing/openapi/3dpack-ing-packing-api-openapi.yml
- filename: 3dpack-ing-typed-api-openapi.yml
  format: yaml
  label: 3dpack-ing Typed API
  slug: 3dpack-ing-typed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/3dpack-ing/openapi/3dpack-ing-typed-api-openapi.yml
consequence_counts:
  physical: 2
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: 3Dpack Ing Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/ai/calculate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/ai/calculate
operation_count: 6
overview: '3dpack-ing exposes 6 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 write and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: 3dpack-ing
provider_slug: 3dpack-ing
slug: 3dpack-ing-agentic-access
source_filename: 3dpack-ing-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/3dpack-ing-openapi.json, openapi/3dpack-ing-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    acting: 6\n  by_consequence:\n    physical: 2\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /api/ai/calculate\n  method: post\n  operationId: packShipment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calculate\n  method: post\n  operationId:\
  \ typedCalculate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/best-boxes\n  method: post\n  operationId: typedBestBoxes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/ai/calculate\n  method: post\n  operationId: packShipment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calculate\n  method: post\n  operationId: typedCalculate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/best-boxes\n  method: post\n  operationId: typedBestBoxes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/3dpack-ing/agentic-access/3dpack-ing-agentic-access.yml
summary_line: 6 operations · 6 acting
tags:
- Company
- Logistics
- 3D
- Software-as-a-Service
---
