---
acting_count: 0
action_class_counts:
  connected: 6
api_specs:
- filename: pennsylvania-state-university-fis.yaml
  format: yaml
  label: LionSpaceFIS REST API
  slug: fis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennsylvania-state-university/refs/heads/main/openapi/pennsylvania-state-university-fis.yaml
consequence_counts:
  read: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Pennsylvania State University Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Pennsylvania State University exposes 6 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Pennsylvania State University
provider_slug: pennsylvania-state-university
slug: pennsylvania-state-university-agentic-access
source_filename: pennsylvania-state-university-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/pennsylvania-state-university-fis.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 6\n  by_consequence:\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /campuses\n  method: get\n  operationId: listCampuses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /buildings\n  method: get\n  operationId: listBuildings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rooms\n  method: get\n  operationId: listRooms\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /buildingEvents\n  method: get\n  operationId: listBuildingEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /roomEvents\n  method: get\n  operationId: listRoomEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pennsylvania-state-university/refs/heads/main/agentic-access/pennsylvania-state-university-agentic-access.yml
summary_line: 6 operations
tags:
- Education
- Higher Education
- University
- Research
- Library
- Facilities
- United States
---
