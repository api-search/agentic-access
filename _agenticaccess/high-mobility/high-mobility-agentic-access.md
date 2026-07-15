---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 4
api_specs:
- filename: high-mobility-openapi.yml
  format: yaml
  label: High Mobility Vehicle API
  slug: high-mobility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/high-mobility/refs/heads/main/openapi/high-mobility-openapi.yml
consequence_counts:
  read: 4
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: High Mobility Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'High Mobility exposes 7 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: High Mobility
provider_slug: high-mobility
slug: high-mobility-agentic-access
source_filename: high-mobility-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/high-mobility-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    acting: 3\n    connected: 4\n  by_consequence:\n    write: 3\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/access_token\n  method: post\n  operationId: createAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - vehicle:data\n- path: /v1/vehicle-data/autoapi-13/{vin}\n  method: get\n  operationId: getVehicleData\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - vehicle:data\n- path: /v1/eligibility/{vin}\n  method: get\n  operationId: getVehicleEligibility\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - vehicle:data\n- path: /v1/fleet/vehicles\n  method: get\n  operationId: listFleetVehicles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - vehicle:data\n- path: /v1/fleet/vehicles\n  method: post\n  operationId: addFleetVehicle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n    scope:\n    - vehicle:data\n- path: /v1/fleet/vehicles/{vin}\n  method: get\n  operationId: getFleetVehicle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - vehicle:data\n- path: /v1/fleet/vehicles/{vin}\n  method: delete\n  operationId: removeFleetVehicle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - vehicle:data\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/high-mobility/refs/heads/main/agentic-access/high-mobility-agentic-access.yml
summary_line: 7 operations · 3 acting
tags:
- Automotive
- Connected Cars
- IoT
- Vehicle Data
---
