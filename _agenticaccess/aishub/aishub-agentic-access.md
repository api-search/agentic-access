---
acting_count: 0
action_class_counts:
  connected: 2
api_specs:
- filename: aishub-openapi.yml
  format: yaml
  label: AISHub Vessel Positions API
  slug: aishub-vessel-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aishub/refs/heads/main/openapi/aishub-openapi.yml
- filename: aishub-openapi.yml
  format: yaml
  label: AISHub Stations API
  slug: aishub-stations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aishub/refs/heads/main/openapi/aishub-openapi.yml
consequence_counts:
  read: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Aishub Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 2
overview: 'AISHub exposes 2 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AISHub
provider_slug: aishub
slug: aishub-agentic-access
source_filename: aishub-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/aishub-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 2\n  by_action_class:\n    connected: 2\n  by_consequence:\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /ws.php\n  method: get\n  operationId: getVesselPositions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stations.php\n  method: get\n  operationId: getStations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aishub/refs/heads/main/agentic-access/aishub-agentic-access.yml
summary_line: 2 operations
tags:
- Vessel Tracking
- Maritime
- AIS
- Shipping
- Geospatial
- Data Sharing
---
