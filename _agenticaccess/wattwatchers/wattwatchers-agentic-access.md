---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 13
api_specs:
- filename: wattwatchers-rest-api-v3-openapi.json
  format: json
  label: Wattwatchers REST API v3 (Mercury)
  slug: wattwatchers-rest-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wattwatchers/refs/heads/main/openapi/wattwatchers-rest-api-v3-openapi.json
consequence_counts:
  physical: 1
  read: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Wattwatchers Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: required
  method: PATCH
  path: /devices/{device-id}
operation_count: 14
overview: 'Wattwatchers exposes 14 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read and 1 physical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Wattwatchers
provider_slug: wattwatchers
slug: wattwatchers-agentic-access
source_filename: wattwatchers-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: generated\nsource: openapi/wattwatchers-rest-api-v3-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI.\n  A governance starting point for exposing this API to AI agents — review and bind audience per deployment.\n  See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 13\n    acting: 1\n  by_consequence:\n    read: 13\n    physical: 1\n  human_in_the_loop_required: 1\n  curated_operations: 1\noperations:\n- path: /devices\n  method: get\n  operationId: listDevices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices/{device-id}\n  method: get\n  operationId: getDevice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /devices/{device-id}\n  method: patch\n  operationId: updateDevice\n  curated: true\n  curation_note: 'Raised from the heuristic default (consequence write / human-in-the-loop conditional)\n    to consequence PHYSICAL with human-in-the-loop REQUIRED. This single operation carries the API''s\n    entire actuation surface: the `switches` array in the PATCH body opens or closes a real relay on +3SW\n    hardware (6M+3SW, 6W+3SW, 3RM+3SW), energising or de-energising a live electrical circuit. Wattwatchers\n    document a dedicated switching guide for it. The keyword heuristic could not see this because the\n    path and method carry no control/dispatch token — the consequence lives in the request body. Evidence:\n    https://docs.wattwatchers.com.au/api/tips/switching-example.html and openapi #/components/schemas/DevicePatchBody.switches.'\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: required\n      purpose-required: true\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - switch-state-change\n      - abnormal\n      - high-value\n    audit: required\n- path: /devices/channel-categories\n  method: get\n  operationId: getChannelCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices/models\n  method: get\n  operationId: getDeviceModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /short-energy/{device-id}\n  method: get\n  operationId: getShortEnergyData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /short-energy/{device-id}/first\n  method: get\n  operationId: getFirstShortEnergyData\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /short-energy/{device-id}/latest\n  method: get\n  operationId: getLatestShortEnergyData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /long-energy/{device-id}\n  method: get\n  operationId: getLongEnergyData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /long-energy/{device-id}/first\n  method: get\n  operationId: getFirstLongEnergyData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /long-energy/{device-id}/latest\n  method: get\n  operationId: getLatestLongEnergyData\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /modbus/{device-id}\n  method: get\n  operationId: getModbusData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /modbus/{device-id}/first\n  method: get\n  operationId: getFirstModbusData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /modbus/{device-id}/latest\n  method: get\n  operationId: getLatestModbusData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\ncuration: updateDevice raised to consequence=physical / human-in-the-loop=required after review; see the\n  curation_note on that operation.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wattwatchers/refs/heads/main/agentic-access/wattwatchers-agentic-access.yml
summary_line: 14 operations · 1 acting · 1 human-in-the-loop
tags:
- Energy
- Australia
- Utilities
- Electricity
- Smart Metering
- Energy Data
- IoT
- Solar
- DER
- Demand Response
---
