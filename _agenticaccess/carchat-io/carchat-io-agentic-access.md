---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 4
api_specs:
- filename: carchat-io-dealers-api-openapi.yml
  format: yaml
  label: CarChat Dealers API
  slug: carchat-io-dealers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carchat-io/openapi/carchat-io-dealers-api-openapi.yml
- filename: carchat-io-inventory-api-openapi.yml
  format: yaml
  label: CarChat Inventory API
  slug: carchat-io-inventory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carchat-io/openapi/carchat-io-inventory-api-openapi.yml
- filename: carchat-io-lead-api-openapi.yml
  format: yaml
  label: CarChat Lead API
  slug: carchat-io-lead-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carchat-io/openapi/carchat-io-lead-api-openapi.yml
- filename: carchat-io-segments-api-openapi.yml
  format: yaml
  label: CarChat Segments API
  slug: carchat-io-segments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carchat-io/openapi/carchat-io-segments-api-openapi.yml
- filename: carchat-io-vehicles-api-openapi.yml
  format: yaml
  label: CarChat Vehicles API
  slug: carchat-io-vehicles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carchat-io/openapi/carchat-io-vehicles-api-openapi.yml
consequence_counts:
  physical: 1
  read: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Carchat Io Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/lead
operation_count: 5
overview: 'CarChat exposes 5 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CarChat
provider_slug: carchat-io
slug: carchat-io-agentic-access
source_filename: carchat-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/carchat-io-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 4\n    acting: 1\n  by_consequence:\n    read: 4\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/inventory\n  method: get\n  operationId: searchInventory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/vehicles/{id}\n  method: get\n  operationId: getVehicle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/dealers\n  method:\
  \ get\n  operationId: listDealers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/segments\n  method: get\n  operationId: listSegments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/lead\n  method: post\n  operationId: submitInquiry\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/carchat-io/agentic-access/carchat-io-agentic-access.yml
summary_line: 5 operations · 1 acting
tags:
- Company
- Marketplace
- Automotive
- Artificial Intelligence
- OpenAPI
---
