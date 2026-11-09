---
acting_count: 0
action_class_counts:
  connected: 1
api_specs:
- filename: infoplaza-geo-api-openapi.yml
  format: yaml
  label: Infoplaza Geo API
  slug: infoplaza-geo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infoplaza/openapi/infoplaza-geo-api-openapi.yml
- filename: infoplaza-marine-api-openapi.yml
  format: yaml
  label: Infoplaza Marine API
  slug: infoplaza-marine-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infoplaza/openapi/infoplaza-marine-api-openapi.yml
- filename: infoplaza-observations-api-openapi.yml
  format: yaml
  label: Infoplaza Observations API
  slug: infoplaza-observations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infoplaza/openapi/infoplaza-observations-api-openapi.yml
- filename: infoplaza-port-api-openapi.yml
  format: yaml
  label: Infoplaza Port API
  slug: infoplaza-port-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infoplaza/openapi/infoplaza-port-api-openapi.yml
- filename: infoplaza-storms-api-openapi.yml
  format: yaml
  label: Infoplaza Storms API
  slug: infoplaza-storms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infoplaza/openapi/infoplaza-storms-api-openapi.yml
- filename: infoplaza-traffic-api-openapi.yml
  format: yaml
  label: Infoplaza Traffic API
  slug: infoplaza-traffic-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infoplaza/openapi/infoplaza-traffic-api-openapi.yml
- filename: infoplaza-transit-api-openapi.yml
  format: yaml
  label: Infoplaza Transit API
  slug: infoplaza-transit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infoplaza/openapi/infoplaza-transit-api-openapi.yml
- filename: infoplaza-weather-api-openapi.yml
  format: yaml
  label: Infoplaza Weather API
  slug: infoplaza-weather-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infoplaza/openapi/infoplaza-weather-api-openapi.yml
consequence_counts:
  read: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Infoplaza Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 1
overview: 'Infoplaza exposes 1 API operation that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Infoplaza
provider_slug: infoplaza
slug: infoplaza-agentic-access
source_filename: infoplaza-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: generated\nsource: openapi/infoplaza-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 1\n  by_action_class:\n    connected: 1\n  by_consequence:\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/marine/shipping/point\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/infoplaza/agentic-access/infoplaza-agentic-access.yml
summary_line: 1 operation
tags:
- Company
- Weather
- Mobility
- Forecasting
- Event Planning
- Data Analytics
- Weather Data
- Marine
- Meteorology
- Geospatial
---
