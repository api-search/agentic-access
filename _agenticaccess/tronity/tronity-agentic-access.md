---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 14
api_specs:
- filename: tronity-openapi.yml
  format: yaml
  label: TRONITY Vehicles API
  slug: tronity-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tronity/refs/heads/main/openapi/tronity-openapi.yml
- filename: tronity-openapi.yml
  format: yaml
  label: TRONITY Vehicle Data API
  slug: tronity-vehicle-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tronity/refs/heads/main/openapi/tronity-openapi.yml
- filename: tronity-openapi.yml
  format: yaml
  label: TRONITY Charging & Battery API
  slug: tronity-charging-battery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tronity/refs/heads/main/openapi/tronity-openapi.yml
- filename: tronity-openapi.yml
  format: yaml
  label: TRONITY Commands API
  slug: tronity-commands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tronity/refs/heads/main/openapi/tronity-openapi.yml
- filename: tronity-openapi.yml
  format: yaml
  label: TRONITY Webhooks API
  slug: tronity-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tronity/refs/heads/main/openapi/tronity-openapi.yml
consequence_counts:
  read: 14
  safety-critical: 4
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 4
kind: agentic-access
layout: agentic-access
method: generated
name: Tronity Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /oauth/authentication
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/vehicles/{vehicleId}/charge_start
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/vehicles/{vehicleId}/charge_stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/vehicles/{vehicleId}/wake_up
operation_count: 21
overview: 'TRONITY exposes 21 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read, 3 write, and 4 safety-critical.


  4 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: TRONITY
provider_slug: tronity
slug: tronity-agentic-access
source_filename: tronity-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/tronity-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    acting: 7\n    connected: 14\n  by_consequence:\n    safety-critical: 4\n    read: 14\n    write: 3\n  human_in_the_loop_required: 4\noperations:\n- path: /oauth/authentication\n  method: post\n  operationId: authControllerAuthentication\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/vehicles\n  method: get\n  operationId:\
  \ getManyVehicles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vehicles/{id}\n  method: get\n  operationId: getOneVehicle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vehicles/{id}\n  method: delete\n  operationId: deleteOneVehicle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/vehicles/{vehicleId}/vin\n  method: get\n  operationId: vehicleControllerVin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vehicles/{vehicleId}/odometer\n\
  \  method: get\n  operationId: vehicleControllerOdometer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vehicles/{vehicleId}/location\n  method: get\n  operationId: vehicleControllerLocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vehicles/{vehicleId}/bulk\n  method: get\n  operationId: vehicleControllerBulk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vehicles/{vehicleId}/records\n  method: get\n  operationId: getManyRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vehicles/{vehicleId}/trips\n  method: get\n  operationId: getManyTrips\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vehicles/{vehicleId}/idles\n  method: get\n  operationId: getManyIdles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vehicles/{vehicleId}/sleeps\n  method: get\n  operationId: getManySleeps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vehicles/{vehicleId}/battery\n  method: get\n  operationId: vehicleControllerBattery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vehicles/{vehicleId}/charge\n  method: get\n  operationId: vehicleControllerCharge\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vehicles/{vehicleId}/charges\n  method: get\n  operationId: getManyCharges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vehicles/{vehicleId}/charge_start\n  method: post\n  operationId: vehicleControllerChargeStart\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/vehicles/{vehicleId}/charge_stop\n  method: post\n  operationId: vehicleControllerChargeStop\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n    \
  \  max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/vehicles/{vehicleId}/wake_up\n  method: post\n  operationId: vehicleControllerWakeUp\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/users/{userId}/apps/{appId}/webhooks\n  method: get\n  operationId: getManyWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/{userId}/apps/{appId}/webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n  \
  \  subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/{userId}/apps/{appId}/webhooks/{id}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tronity/refs/heads/main/agentic-access/tronity-agentic-access.yml
summary_line: 21 operations · 7 acting · 4 human-in-the-loop
tags:
- Connected Car
- EV
- Telematics
- Fleet
- Vehicle Data
---
