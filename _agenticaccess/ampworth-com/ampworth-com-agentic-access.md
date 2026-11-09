---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 20
api_specs:
- filename: ampworth-com-calculators-api-openapi.yml
  format: yaml
  label: ampworth-com Calculators API
  slug: ampworth-com-calculators-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ampworth-com/openapi/ampworth-com-calculators-api-openapi.yml
- filename: ampworth-com-discovery-api-openapi.yml
  format: yaml
  label: ampworth-com Discovery API
  slug: ampworth-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ampworth-com/openapi/ampworth-com-discovery-api-openapi.yml
- filename: ampworth-com-documents-api-openapi.yml
  format: yaml
  label: ampworth-com Documents API
  slug: ampworth-com-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ampworth-com/openapi/ampworth-com-documents-api-openapi.yml
consequence_counts:
  read: 20
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ampworth Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 31
overview: 'ampworth-com exposes 31 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 read and 11 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ampworth-com
provider_slug: ampworth-com
slug: ampworth-com-agentic-access
source_filename: ampworth-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/ampworth-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 31\n  by_action_class:\n    connected: 20\n    acting: 11\n  by_consequence:\n    read: 20\n    write: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1\n  method: get\n  operationId: discovery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/calculators\n  method: get\n  operationId: listCalculators\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/calculators/connection-route\n\
  \  method: get\n  operationId: getConnectionRoute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/calculators/connection-route\n  method: post\n  operationId: runConnectionRoute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calculators/heat-pump-noise\n  method: get\n  operationId: getHeatPumpNoise\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/calculators/heat-pump-noise\n  method: post\n  operationId: runHeatPumpNoise\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n \
  \   audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calculators/heat-pump-running-cost\n  method: get\n  operationId: getHeatPumpRunningCost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/calculators/heat-pump-running-cost\n  method: post\n  operationId: runHeatPumpRunningCost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calculators/heat-pump-size\n  method: get\n  operationId: getHeatPumpSize\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/calculators/heat-pump-size\n  method: post\n  operationId: runHeatPumpSize\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calculators/hot-water-cylinder\n  method: get\n  operationId: getHotWaterCylinder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/calculators/hot-water-cylinder\n  method: post\n  operationId: runHotWaterCylinder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/v1/calculators/radiator-flow-temperature\n  method: get\n  operationId: getRadiatorFlowTemperature\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/calculators/radiator-flow-temperature\n  method: post\n  operationId: runRadiatorFlowTemperature\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calculators/room-heat-loss\n  method: get\n  operationId: getRoomHeatLoss\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/calculators/room-heat-loss\n  method: post\n  operationId:\
  \ runRoomHeatLoss\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calculators/solar-pv-output\n  method: get\n  operationId: getSolarPvOutput\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/calculators/solar-pv-output\n  method: post\n  operationId: runSolarPvOutput\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calculators/solar-pv-self-consumption\n  method: get\n  operationId: getSolarPvSelfConsumption\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/calculators/solar-pv-self-consumption\n  method: post\n  operationId: runSolarPvSelfConsumption\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calculators/solar-pv-shading\n  method: get\n  operationId: getSolarPvShading\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/calculators/solar-pv-shading\n  method: post\n  operationId: runSolarPvShading\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calculators/solar-pv-system-size\n  method: get\n  operationId: getSolarPvSystemSize\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/calculators/solar-pv-system-size\n  method: post\n  operationId: runSolarPvSystemSize\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calculators/{id}\n  method: get\n  operationId: describeCalculator\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/v1/documents\n  method: get\n  operationId: listDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/documents/categories\n  method: get\n  operationId: listCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/documents/perspectives\n  method: get\n  operationId: listPerspectives\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/documents/search\n  method: get\n  operationId: searchDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/documents/{kind}/{slug}\n  method: get\n  operationId: getDocument\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/openapi.json\n  method: get\n  operationId: openapi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/ampworth-com/agentic-access/ampworth-com-agentic-access.yml
summary_line: 31 operations · 11 acting
tags:
- Company
- Energy
- Heat Pumps
- Solar
- Batteries
- United Kingdom
---
