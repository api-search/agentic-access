---
acting_count: 0
action_class_counts:
  connected: 5
api_specs:
- filename: openweather-openapi.yml
  format: yaml
  label: OpenWeather One Call API
  slug: openweather-one-call-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweather/refs/heads/main/openapi/openweather-openapi.yml
consequence_counts:
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Openweather Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'OpenWeather exposes 5 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: OpenWeather
provider_slug: openweather
slug: openweather-agentic-access
source_filename: openweather-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openweather-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 5\n  by_consequence:\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /onecall\n  method: get\n  operationId: getOneCall\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /onecall/timemachine\n  method: get\n  operationId: getOneCallTimemachine\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /air_pollution\n  method: get\n  operationId: getCurrentAirPollution\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /air_pollution/forecast\n  method: get\n  operationId: getAirPollutionForecast\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /air_pollution/history\n  method: get\n  operationId: getAirPollutionHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openweather/refs/heads/main/agentic-access/openweather-agentic-access.yml
summary_line: 5 operations
tags:
- Air Pollution
- Air Quality
- Climate
- Forecasting
- Weather
---
