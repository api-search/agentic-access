---
acting_count: 0
action_class_counts:
  connected: 6
api_specs:
- filename: bright-sky-alerts-api-openapi.yml
  format: yaml
  label: Bright Sky Alerts API
  slug: bright-sky-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bright-sky/openapi/bright-sky-alerts-api-openapi.yml
- filename: bright-sky-current-weather-api-openapi.yml
  format: yaml
  label: Bright Sky Current Weather API
  slug: bright-sky-current-weather-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bright-sky/openapi/bright-sky-current-weather-api-openapi.yml
- filename: bright-sky-internals-api-openapi.yml
  format: yaml
  label: Bright Sky Internals API
  slug: bright-sky-internals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bright-sky/openapi/bright-sky-internals-api-openapi.yml
- filename: bright-sky-radar-api-openapi.yml
  format: yaml
  label: Bright Sky Radar API
  slug: bright-sky-radar-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bright-sky/openapi/bright-sky-radar-api-openapi.yml
- filename: bright-sky-weather-api-openapi.yml
  format: yaml
  label: Bright Sky Weather API
  slug: bright-sky-weather-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bright-sky/openapi/bright-sky-weather-api-openapi.yml
consequence_counts:
  read: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bright Sky Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Bright Sky exposes 6 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bright Sky
provider_slug: bright-sky
slug: bright-sky-agentic-access
source_filename: bright-sky-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: generated\nsource: openapi/full.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 6\n  by_consequence:\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /sources\n  method: get\n  operationId: getSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /current_weather\n  method: get\n  operationId: getCurrentWeather\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /weather\n  method: get\n  operationId: getWeather\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /synop\n  method: get\n  operationId: getSynop\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /radar\n  method: get\n  operationId: getRadar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /alerts\n  method: get\n  operationId: getAlerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/bright-sky/agentic-access/bright-sky-agentic-access.yml
summary_line: 6 operations
tags:
- Company
- Weather
- Open Data
- JSON
---
