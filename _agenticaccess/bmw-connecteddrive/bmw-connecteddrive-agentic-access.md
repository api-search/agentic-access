---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 9
api_specs:
- filename: bmw-cardata-customer-api-openapi.json
  format: json
  label: BMW CarData Customer API
  slug: bmw-cardata-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bmw-connecteddrive/refs/heads/main/openapi/bmw-cardata-customer-api-openapi.json
consequence_counts:
  read: 9
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bmw Connecteddrive Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'BMW ConnectedDrive exposes 11 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BMW ConnectedDrive
provider_slug: bmw-connecteddrive
slug: bmw-connecteddrive-agentic-access
source_filename: bmw-connecteddrive-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/bmw-cardata-customer-api-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 9\n    acting: 2\n  by_consequence:\n    read: 9\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /customers/containers\n  method: get\n  operationId: listContainers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/containers\n  method: post\n  operationId: createContainer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/vehicles/{vin}/telematicData\n  method: get\n  operationId: getTelematicData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/vehicles/{vin}/smartMaintenanceTyreDiagnosis\n  method: get\n  operationId: getSmartMaintenanceTyreDiagnosis\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/vehicles/{vin}/locationBasedChargingSettings\n  method: get\n  operationId: getLocationBasedChargingSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/vehicles/{vin}/image\n  method: get\n  operationId: getImage\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/vehicles/{vin}/chargingHistory\n  method: get\n  operationId: getChargingHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/vehicles/{vin}/basicData\n  method: get\n  operationId: getBasicData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/vehicles/mappings\n  method: get\n  operationId: getMappings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/containers/{containerId}\n  method: get\n  operationId: getContainerDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/containers/{containerId}\n  method: delete\n  operationId: deleteContainer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bmw-connecteddrive/refs/heads/main/agentic-access/bmw-connecteddrive-agentic-access.yml
summary_line: 11 operations · 2 acting
tags:
- Automotive
- Connected Vehicle
- Telematics
- Vehicle Data
- CarData
- ConnectedDrive
- Electric Vehicles
- Charging
- MQTT
- Streaming
- OAuth
- Device Code Flow
- GDPR
- Right To Repair
- Mobility
---
