---
acting_count: 0
action_class_counts:
  connected: 19
api_specs:
- filename: ambee-openapi.yml
  format: yaml
  label: Ambee Air Quality API
  slug: air-quality
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambee/refs/heads/main/openapi/ambee-openapi.yml
- filename: ambee-openapi.yml
  format: yaml
  label: Ambee Pollen API
  slug: pollen
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambee/refs/heads/main/openapi/ambee-openapi.yml
- filename: ambee-openapi.yml
  format: yaml
  label: Ambee Weather API
  slug: weather
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambee/refs/heads/main/openapi/ambee-openapi.yml
- filename: ambee-openapi.yml
  format: yaml
  label: Ambee Fire API
  slug: fire
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambee/refs/heads/main/openapi/ambee-openapi.yml
- filename: ambee-openapi.yml
  format: yaml
  label: Ambee Soil API
  slug: soil
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambee/refs/heads/main/openapi/ambee-openapi.yml
- filename: ambee-openapi.yml
  format: yaml
  label: Ambee NDVI / Vegetation API
  slug: ndvi-vegetation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambee/refs/heads/main/openapi/ambee-openapi.yml
consequence_counts:
  read: 19
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ambee Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 19
overview: 'Ambee exposes 19 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Ambee
provider_slug: ambee
slug: ambee-agentic-access
source_filename: ambee-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/ambee-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    connected: 19\n  by_consequence:\n    read: 19\n  human_in_the_loop_required: 0\noperations:\n- path: /latest/by-lat-lng\n  method: get\n  operationId: getAirQualityLatestByLatLng\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /latest/by-city\n  method: get\n  operationId: getAirQualityLatestByCity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /latest/by-postal-code\n  method:\
  \ get\n  operationId: getAirQualityLatestByPostalCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /history/by-lat-lng\n  method: get\n  operationId: getAirQualityHistoryByLatLng\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /forecast/aq/by-lat-lng\n  method: get\n  operationId: getAirQualityForecastByLatLng\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /latest/pollen/by-lat-lng\n  method: get\n  operationId: getPollenLatestByLatLng\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /latest/pollen/by-place\n  method: get\n  operationId: getPollenLatestByPlace\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /history/pollen/by-lat-lng\n  method: get\n  operationId: getPollenHistoryByLatLng\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /forecast/pollen/by-lat-lng\n  method: get\n  operationId: getPollenForecastByLatLng\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /forecast/v2/pollen/120hr/by-lat-lng\n  method: get\n  operationId: getPollen120hrForecastByLatLng\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /weather/latest/by-lat-lng\n  method: get\n  operationId: getWeatherLatestByLatLng\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /weather/history/by-lat-lng\n  method: get\n  operationId: getWeatherHistoryByLatLng\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /weather/forecast/by-lat-lng\n  method: get\n  operationId: getWeatherForecastByLatLng\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fire/latest/by-lat-lng\n  method: get\n  operationId: getFireLatestByLatLng\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fire/risk/by-lat-lng\n  method: get\n  operationId: getFireRiskByLatLng\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /soil/latest/by-lat-lng\n  method: get\n  operationId: getSoilLatestByLatLng\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /soil/history/by-lat-lng\n  method: get\n  operationId: getSoilHistoryByLatLng\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ndvi/latest/by-lat-lng\n  method: get\n  operationId: getNdviLatestByLatLng\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ndvi/history/by-lat-lng\n  method: get\n  operationId: getNdviHistoryByLatLng\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ambee/refs/heads/main/agentic-access/ambee-agentic-access.yml
summary_line: 19 operations
tags:
- Environmental Intelligence
- Air Quality
- Weather
- Pollen
- Geospatial
---
