---
acting_count: 0
action_class_counts:
  connected: 16
api_specs:
- filename: carstat-app-recalls-api-openapi.yml
  format: yaml
  label: carstat-app Recalls API
  slug: carstat-app-recalls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carstat-app/openapi/carstat-app-recalls-api-openapi.yml
- filename: carstat-app-safety-ratings-api-openapi.yml
  format: yaml
  label: carstat-app Safety Ratings API
  slug: carstat-app-safety-ratings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carstat-app/openapi/carstat-app-safety-ratings-api-openapi.yml
- filename: carstat-app-vehicle-specifications-api-openapi.yml
  format: yaml
  label: carstat-app Vehicle Specifications API
  slug: carstat-app-vehicle-specifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carstat-app/openapi/carstat-app-vehicle-specifications-api-openapi.yml
- filename: carstat-app-vin-decoding-api-openapi.yml
  format: yaml
  label: carstat-app VIN Decoding API
  slug: carstat-app-vin-decoding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carstat-app/openapi/carstat-app-vin-decoding-api-openapi.yml
consequence_counts:
  read: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Carstat App Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'carstat-app exposes 16 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: carstat-app
provider_slug: carstat-app
slug: carstat-app-agentic-access
source_filename: carstat-app-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/carstat-app-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 16\n  by_consequence:\n    read: 16\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/specs/makes/{year}\n  method: get\n  operationId: getMakesByYear\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/specs/models/{year}/{make}\n  method: get\n  operationId: getModelsByYearMake\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/specs/modifications/{year}/{make}/{model}\n\
  \  method: get\n  operationId: getModificationsByYearMakeModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/specs/{modification_id}\n  method: get\n  operationId: getVehicleSpecs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/specs/vin/{vin}\n  method: get\n  operationId: getVehicleSpecsByVin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/recalls/years\n  method: get\n  operationId: getRecallYears\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/recalls/makes/{year}\n  method: get\n  operationId: getRecallMakesByYear\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/recalls/models/{year}/{make}\n  method: get\n  operationId: getRecallModelsByYearMake\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/recalls/{year}/{make}/{model}\n  method: get\n  operationId: getRecallsByVehicle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/safety-ratings/years\n  method: get\n  operationId: getSafetyRatingYears\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/safety-ratings/makes/{year}\n  method: get\n  operationId: getSafetyRatingMakesByYear\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n \
  \   subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/safety-ratings/models/{year}/{make}\n  method: get\n  operationId: getSafetyRatingModelsByYearMake\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/safety-ratings/{year}/{make}/{model}\n  method: get\n  operationId: getSafetyRatingsByVehicle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/specs/search\n  method: get\n  operationId: searchVehicles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vin-decode/{vin}\n  method: get\n  operationId: decodeVin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/specs/years\n  method: get\n  operationId: getYears\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/carstat-app/agentic-access/carstat-app-agentic-access.yml
summary_line: 16 operations
tags:
- Company
- Automotive
- Data
- Vehicles
---
