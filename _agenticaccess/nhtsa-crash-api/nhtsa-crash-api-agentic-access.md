---
acting_count: 0
action_class_counts:
  connected: 6
api_specs:
- filename: nhtsa-crash-api-nhtsa-crash-data-api-openapi.yml
  format: yaml
  label: NHTSA Crash Data API
  slug: nhtsa-crash-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhtsa-crash-api/refs/heads/main/openapi/nhtsa-crash-api-nhtsa-crash-data-api-openapi.yml
consequence_counts:
  read: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Nhtsa Crash Api Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'NHTSA Crash API exposes 6 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: NHTSA Crash API
provider_slug: nhtsa-crash-api
slug: nhtsa-crash-api-agentic-access
source_filename: nhtsa-crash-api-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/nhtsa-crash-api-nhtsa-crash-data-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 6\n  by_consequence:\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /FARSData/GetFARSData\n  method: get\n  operationId: getFARSData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crashes/GetCaseList\n  method: get\n  operationId: getCaseList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crashes/GetCaseDetails\n  method:\
  \ get\n  operationId: getCaseDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crashes/GetCrashesByLocation\n  method: get\n  operationId: getCrashesByLocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crashes/GetCrashesByVehicle\n  method: get\n  operationId: getCrashesByVehicle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crashes/GetCrashesByOccupant\n  method: get\n  operationId: getCrashesByOccupant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nhtsa-crash-api/refs/heads/main/agentic-access/nhtsa-crash-api-agentic-access.yml
summary_line: 6 operations
tags:
- Crash Data
- Government
- NHTSA
- Traffic Safety
- Transportation
---
