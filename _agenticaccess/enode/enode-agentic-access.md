---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 18
api_specs:
- filename: enode-batteries-api-openapi.yml
  format: yaml
  label: Enode Batteries API
  slug: enode-batteries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enode/refs/heads/main/openapi/enode-batteries-api-openapi.yml
- filename: enode-chargers-api-openapi.yml
  format: yaml
  label: Enode Chargers API
  slug: enode-chargers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enode/refs/heads/main/openapi/enode-chargers-api-openapi.yml
- filename: enode-hvac-api-openapi.yml
  format: yaml
  label: Enode HVAC API
  slug: enode-hvac-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enode/refs/heads/main/openapi/enode-hvac-api-openapi.yml
- filename: enode-inverters-api-openapi.yml
  format: yaml
  label: Enode Inverters API
  slug: enode-inverters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enode/refs/heads/main/openapi/enode-inverters-api-openapi.yml
- filename: enode-meters-api-openapi.yml
  format: yaml
  label: Enode Meters API
  slug: enode-meters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enode/refs/heads/main/openapi/enode-meters-api-openapi.yml
- filename: enode-smart-charging-api-openapi.yml
  format: yaml
  label: Enode Smart Charging API
  slug: enode-smart-charging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enode/refs/heads/main/openapi/enode-smart-charging-api-openapi.yml
- filename: enode-users-api-openapi.yml
  format: yaml
  label: Enode Users API
  slug: enode-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enode/refs/heads/main/openapi/enode-users-api-openapi.yml
- filename: enode-vehicles-api-openapi.yml
  format: yaml
  label: Enode Vehicles API
  slug: enode-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enode/refs/heads/main/openapi/enode-vehicles-api-openapi.yml
- filename: enode-webhooks-api-openapi.yml
  format: yaml
  label: Enode Webhooks API
  slug: enode-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enode/refs/heads/main/openapi/enode-webhooks-api-openapi.yml
consequence_counts:
  physical: 1
  read: 18
  safety-critical: 2
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Enode Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /chargers/{chargerId}/charging
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /vehicles/{vehicleId}/charging
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /webhooks/{webhookId}/test
operation_count: 27
overview: 'Enode exposes 27 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read, 6 write, 1 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Enode
provider_slug: enode
slug: enode-agentic-access
source_filename: enode-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/enode-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 27\n  by_action_class:\n    acting: 9\n    connected: 18\n  by_consequence:\n    write: 6\n    read: 18\n    safety-critical: 2\n    physical: 1\n  human_in_the_loop_required: 2\noperations:\n- path: /users/{userId}/link\n  method: post\n  operationId: linkUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{userId}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{userId}\n  method: delete\n  operationId: deleteUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vehicles\n  method: get\n  operationId: listVehicles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vehicles/{vehicleId}\n  method: get\n  operationId: getVehicle\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vehicles/{vehicleId}/charging\n  method: post\n  operationId: controlVehicleCharging\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /vehicles/{vehicleId}/smart-charging-policy\n  method: get\n  operationId: getVehicleSmartChargingPolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vehicles/{vehicleId}/smart-charging-policy\n  method: post\n  operationId: setVehicleSmartChargingPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vehicles/{vehicleId}/smart-charging-plans\n  method: get\n  operationId: getVehicleSmartChargingPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chargers\n  method: get\n  operationId: listChargers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chargers/{chargerId}\n  method: get\n  operationId: getCharger\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chargers/{chargerId}/charging\n  method: post\n  operationId: controlChargerCharging\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /hvacs\n  method: get\n  operationId: listHvacs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hvacs/{hvacId}\n  method: get\n  operationId: getHvac\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /batteries\n  method: get\n  operationId: listBatteries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /batteries/{batteryId}\n  method: get\n  operationId: getBattery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /batteries/{batteryId}/operation-mode\n  method: post\n  operationId: setBatteryOperationMode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inverters\n  method: get\n  operationId: listInverters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inverters/{inverterId}\n  method: get\n  operationId: getInverter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /meters\n  method: get\n  operationId: listMeters\n  x-agentic-access:\n    action-class: connected\n   \
  \ consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /meters/{meterId}\n  method: get\n  operationId: getMeter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{webhookId}\n  method: get\n  operationId: getWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/{webhookId}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{webhookId}/test\n  method: post\n  operationId: testWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enode/refs/heads/main/agentic-access/enode-agentic-access.yml
summary_line: 27 operations · 9 acting · 2 human-in-the-loop
tags:
- Energy
- Electric Vehicles
- EV Charging
- Smart Charging
- Energy Transition
---
