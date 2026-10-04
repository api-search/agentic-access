---
acting_count: 0
action_class_counts:
  connected: 3
api_specs:
- filename: windy-point-forecast-api-openapi.yml
  format: yaml
  label: Windy Point Forecast API
  slug: windy-point-forecast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windy/refs/heads/main/openapi/windy-point-forecast-api-openapi.yml
- filename: windy-webcams-api-openapi.yml
  format: yaml
  label: Windy Webcams API
  slug: windy-webcams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windy/refs/heads/main/openapi/windy-webcams-api-openapi.yml
consequence_counts:
  read: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Windy Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 3
overview: 'Windy exposes 3 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Windy
provider_slug: windy
slug: windy-agentic-access
source_filename: windy-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/windy-point-forecast-api-openapi.yml, openapi/windy-webcams-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 3\n  by_action_class:\n    connected: 3\n  by_consequence:\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /api/point-forecast/v2\n  method: post\n  operationId: getPointForecast\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webcams/api/v3/webcams\n  method: get\n  operationId: listWebcams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /webcams/api/v3/webcams/{webcamId}\n  method: get\n  operationId: getWebcam\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/windy/refs/heads/main/agentic-access/windy-agentic-access.yml
summary_line: 3 operations
tags:
- Weather
- Forecast
- Maps
- Webcams
- Visualization
---
