---
acting_count: 0
action_class_counts:
  connected: 8
api_specs:
- filename: colorfulclouds-caiyun-weather-openapi.yml
  format: yaml
  label: Caiyun Weather API
  slug: caiyun-weather-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colorfulclouds/refs/heads/main/openapi/colorfulclouds-caiyun-weather-openapi.yml
consequence_counts:
  read: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Colorfulclouds Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'ColorfulClouds exposes 8 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ColorfulClouds
provider_slug: colorfulclouds
slug: colorfulclouds-agentic-access
source_filename: colorfulclouds-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/colorfulclouds-caiyun-weather-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 8\n  by_consequence:\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /{token}/{lnglat}/realtime\n  method: get\n  operationId: getRealtimeWeather\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{token}/{lnglat}/minutely\n  method: get\n  operationId: getMinutelyPrecipitation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{token}/{lnglat}/hourly\n\
  \  method: get\n  operationId: getHourlyForecast\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{token}/{lnglat}/daily\n  method: get\n  operationId: getDailyForecast\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{token}/{lnglat}/weather\n  method: get\n  operationId: getWeatherCombined\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{token}/{lnglat}/air-quality\n  method: get\n  operationId: getRealtimeAirQuality\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{token}/{lnglat}/alert\n  method: get\n  operationId: getWeatherAlerts\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /precipitation/{z}/{x}/{y}.png\n  method: get\n  operationId: getPrecipitationMapTile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/colorfulclouds/refs/heads/main/agentic-access/colorfulclouds-agentic-access.yml
summary_line: 8 operations
tags:
- Weather
- Forecasting
- Air Quality
- Precipitation
- Hyperlocal
- Geospatial
- China
---
