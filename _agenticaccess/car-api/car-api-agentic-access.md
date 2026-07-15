---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 16
api_specs:
- filename: car-api-openapi-original.yml
  format: yaml
  label: CarAPI Vehicle API
  slug: vehicle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/car-api/refs/heads/main/openapi/car-api-openapi-original.yml
consequence_counts:
  read: 16
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Car Api Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'Car API (carapi.app) exposes 17 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Car API (carapi.app)
provider_slug: car-api
slug: car-api-agentic-access
source_filename: car-api-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/car-api-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    connected: 16\n    acting: 1\n  by_consequence:\n    read: 16\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/account/requests\n  method: get\n  operationId: account:requests:get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/account/requests-today\n  method: get\n  operationId: account:requeststoday:get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/auth/login\n  method: post\n  operationId: auth:api:post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/bodies\n  method: get\n  operationId: makemodeltrimbodies:index:get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data-feeds/download\n  method: get\n  operationId: datafeeds:download:get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data-feeds/last-updated\n  method: get\n  operationId: datafeeds:lastupdated:get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/engines\n  method: get\n  operationId: makemodeltrimengines:index:get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/exterior-colors\n  method: get\n  operationId: makemodeltrimexteriorcolors:index:get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/interior-colors\n  method: get\n  operationId: makemodeltriminteriorcolors:index:get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/makes\n  method: get\n  operationId: makes:index:get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mileages\n\
  \  method: get\n  operationId: makemodeltrimmileages:index:get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/models\n  method: get\n  operationId: makemodels:index:get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/trims\n  method: get\n  operationId: makemodeltrims:index:get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/trims/{id}\n  method: get\n  operationId: makemodeltrims:view:get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/vehicle-attributes\n  method: get\n  operationId: vehicleattributes:display:get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/vin/{vin}\n  method: get\n  operationId: vindecoder:index:get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/years\n  method: get\n  operationId: years:index:get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/car-api/refs/heads/main/agentic-access/car-api-agentic-access.yml
summary_line: 17 operations · 1 acting
tags:
- Automobiles
- Automotive Data
- Cars
- License Plate Decoder
- OBD-II
- Power Sports
- Vehicle API
- Vehicle Specifications
- Vehicles
- VIN Decoder
---
