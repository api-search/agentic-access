---
acting_count: 0
action_class_counts:
  connected: 4
api_specs:
- filename: national-interagency-fire-center-openapi.yml
  format: yaml
  label: NIFC ArcGIS REST Services API
  slug: nifc-arcgis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-interagency-fire-center/main/openapi/national-interagency-fire-center-openapi.yml
consequence_counts:
  read: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: National Interagency Fire Center Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 4
overview: 'National Interagency Fire Center exposes 4 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: National Interagency Fire Center
provider_slug: national-interagency-fire-center
slug: national-interagency-fire-center-agentic-access
source_filename: national-interagency-fire-center-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/national-interagency-fire-center-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    connected: 4\n  by_consequence:\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: listServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{service}/FeatureServer\n  method: get\n  operationId: getFeatureServer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{service}/FeatureServer/{layerId}\n  method:\
  \ get\n  operationId: getLayer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{service}/FeatureServer/{layerId}/query\n  method: get\n  operationId: queryLayer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-interagency-fire-center/refs/heads/main/agentic-access/national-interagency-fire-center-agentic-access.yml
summary_line: 4 operations
tags:
- Emergency Management
- Federal Government
- Geospatial
- Wildfire
---
