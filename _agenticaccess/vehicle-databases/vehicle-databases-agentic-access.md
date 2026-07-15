---
acting_count: 0
action_class_counts:
  connected: 6
api_specs:
- filename: vehicle-databases-openapi.yml
  format: yaml
  label: Vehicle Databases Maintenance API
  slug: vehicle-databases
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vehicle-databases/refs/heads/main/openapi/vehicle-databases-openapi.yml
consequence_counts:
  read: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Vehicle Databases Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Vehicle Databases exposes 6 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Vehicle Databases
provider_slug: vehicle-databases
slug: vehicle-databases-agentic-access
source_filename: vehicle-databases-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/vehicle-databases-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 6\n  by_consequence:\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /vehicle\n  method: get\n  operationId: lookupVehicle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vin/{vin}\n  method: get\n  operationId: decodeVin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /maintenance/{vehicleId}\n  method: get\n  operationId: getMaintenanceSchedule\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/{vehicleId}\n  method: get\n  operationId: listServiceItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recalls/{vehicleId}\n  method: get\n  operationId: getRecalls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tsb/{vehicleId}\n  method: get\n  operationId: getTSBs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vehicle-databases/refs/heads/main/agentic-access/vehicle-databases-agentic-access.yml
summary_line: 6 operations
tags:
- Automotive
- Fleet Management
- Maintenance
- Recalls
- Vehicles
---
