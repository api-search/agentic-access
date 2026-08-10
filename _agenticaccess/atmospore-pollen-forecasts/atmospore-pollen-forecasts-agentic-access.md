---
acting_count: 0
action_class_counts:
  connected: 4
api_specs:
- filename: atmospore-pollen-forecasts-pollen-api-openapi.yml
  format: yaml
  label: Atmospore Pollen Forecasts Pollen API
  slug: atmospore-pollen-forecasts-pollen-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atmospore-pollen-forecasts/refs/heads/main/openapi/atmospore-pollen-forecasts-pollen-api-openapi.yml
- filename: atmospore-pollen-forecasts-pollen-area-api-openapi.yml
  format: yaml
  label: Atmospore Pollen Forecasts Pollen Area API
  slug: atmospore-pollen-forecasts-pollen-area-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atmospore-pollen-forecasts/refs/heads/main/openapi/atmospore-pollen-forecasts-pollen-area-api-openapi.yml
- filename: atmospore-pollen-forecasts-pollen-top-api-openapi.yml
  format: yaml
  label: Atmospore Pollen Forecasts Pollen Top API
  slug: atmospore-pollen-forecasts-pollen-top-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atmospore-pollen-forecasts/refs/heads/main/openapi/atmospore-pollen-forecasts-pollen-top-api-openapi.yml
- filename: atmospore-pollen-forecasts-species-api-openapi.yml
  format: yaml
  label: Atmospore Pollen Forecasts Species API
  slug: atmospore-pollen-forecasts-species-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atmospore-pollen-forecasts/refs/heads/main/openapi/atmospore-pollen-forecasts-species-api-openapi.yml
consequence_counts:
  read: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Atmospore Pollen Forecasts Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 4
overview: 'Atmospore Pollen Forecasts exposes 4 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Atmospore Pollen Forecasts
provider_slug: atmospore-pollen-forecasts
slug: atmospore-pollen-forecasts-agentic-access
source_filename: atmospore-pollen-forecasts-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: generated\nsource: openapi/atmospore-pollen-forecasts-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    connected: 4\n  by_consequence:\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/pollen\n  method: get\n  operationId: getPollenForecast\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/pollen-area\n  method: get\n  operationId: getPollenArea\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/pollen-top\n  method: get\n  operationId:\
  \ getPollenTop\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/species\n  method: get\n  operationId: getSpecies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atmospore-pollen-forecasts/refs/heads/main/agentic-access/atmospore-pollen-forecasts-agentic-access.yml
summary_line: 4 operations
tags:
- weather
- pollen
- allergy
- environmental-data
- health
- geospatial
- forecasting
- smart-home
- mcp
- openapi
- norway
- climate
---
