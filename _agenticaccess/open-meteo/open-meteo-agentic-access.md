---
acting_count: 0
action_class_counts:
  connected: 9
api_specs:
- filename: open-meteo-air-quality-apis-api-openapi.yml
  format: yaml
  label: Open-Meteo Air Quality APIs API
  slug: open-meteo-air-quality-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-meteo/refs/heads/main/openapi/open-meteo-air-quality-apis-api-openapi.yml
- filename: open-meteo-climate-change-apis-api-openapi.yml
  format: yaml
  label: Open-Meteo Climate Change APIs API
  slug: open-meteo-climate-change-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-meteo/refs/heads/main/openapi/open-meteo-climate-change-apis-api-openapi.yml
- filename: open-meteo-elevation-api-api-openapi.yml
  format: yaml
  label: Open-Meteo Elevation API API
  slug: open-meteo-elevation-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-meteo/refs/heads/main/openapi/open-meteo-elevation-api-api-openapi.yml
- filename: open-meteo-ensemble-forecast-apis-api-openapi.yml
  format: yaml
  label: Open-Meteo Ensemble Forecast APIs API
  slug: open-meteo-ensemble-forecast-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-meteo/refs/heads/main/openapi/open-meteo-ensemble-forecast-apis-api-openapi.yml
- filename: open-meteo-flood-apis-api-openapi.yml
  format: yaml
  label: Open-Meteo Flood APIs API
  slug: open-meteo-flood-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-meteo/refs/heads/main/openapi/open-meteo-flood-apis-api-openapi.yml
- filename: open-meteo-historical-weather-apis-api-openapi.yml
  format: yaml
  label: Open-Meteo Historical Weather APIs API
  slug: open-meteo-historical-weather-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-meteo/refs/heads/main/openapi/open-meteo-historical-weather-apis-api-openapi.yml
- filename: open-meteo-marine-weather-apis-api-openapi.yml
  format: yaml
  label: Open-Meteo Marine Weather APIs API
  slug: open-meteo-marine-weather-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-meteo/refs/heads/main/openapi/open-meteo-marine-weather-apis-api-openapi.yml
- filename: open-meteo-seasonal-forecast-apis-api-openapi.yml
  format: yaml
  label: Open-Meteo Seasonal Forecast APIs API
  slug: open-meteo-seasonal-forecast-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-meteo/refs/heads/main/openapi/open-meteo-seasonal-forecast-apis-api-openapi.yml
- filename: open-meteo-weather-forecast-apis-api-openapi.yml
  format: yaml
  label: Open-Meteo Weather Forecast APIs API
  slug: open-meteo-weather-forecast-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-meteo/refs/heads/main/openapi/open-meteo-weather-forecast-apis-api-openapi.yml
consequence_counts:
  read: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Open Meteo Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'Open-Meteo exposes 9 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Open-Meteo
provider_slug: open-meteo
slug: open-meteo-agentic-access
source_filename: open-meteo-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/open-meteo-air-quality-openapi.yml, openapi/open-meteo-climate-openapi.yml,\n  openapi/open-meteo-elevation-openapi.yml, openapi/open-meteo-ensemble-openapi.yml, openapi/open-meteo-flood-openapi.yml,\n  openapi/open-meteo-forecast-openapi.yml, openapi/open-meteo-historical-weather-openapi.yml,\n  openapi/open-meteo-marine-openapi.yml, openapi/open-meteo-seasonal-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 9\n  by_consequence:\n    read: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/air-quality\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/climate\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/elevation\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ensemble\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/flood\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/forecast\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/archive\n  method: get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/marine\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/seasonal\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-meteo/refs/heads/main/agentic-access/open-meteo-agentic-access.yml
summary_line: 9 operations
tags:
- Weather
- Forecast
- Historical Weather
- Air Quality
- Marine
- Climate
- Open-Source
- Free
---
