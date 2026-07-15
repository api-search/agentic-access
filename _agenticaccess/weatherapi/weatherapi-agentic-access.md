---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 11
api_specs:
- filename: weatherapi-openapi-original.yml
  format: yaml
  label: WeatherAPI
  slug: weatherapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weatherapi/refs/heads/main/openapi/weatherapi-openapi-original.yml
consequence_counts:
  read: 11
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Weatherapi Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'WeatherAPI exposes 12 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: WeatherAPI
provider_slug: weatherapi
slug: weatherapi-agentic-access
source_filename: weatherapi-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/weatherapi-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 11\n    acting: 1\n  by_consequence:\n    read: 11\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /current.json\n  method: get\n  operationId: getCurrentWeather\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /forecast.json\n  method: get\n  operationId: getForecast\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /history.json\n  method:\
  \ get\n  operationId: getHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /alerts.json\n  method: get\n  operationId: getAlerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /marine.json\n  method: get\n  operationId: getMarine\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /future.json\n  method: get\n  operationId: getFutureWeather\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search.json\n  method: get\n  operationId: searchLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /ip.json\n  method: get\n  operationId: ipLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /timezone.json\n  method: get\n  operationId: getTimezone\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /astronomy.json\n  method: get\n  operationId: getAstronomy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sports.json\n  method: get\n  operationId: getSports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /current.json#bulk\n  method: post\n  operationId: getBulkCurrentWeather\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weatherapi/refs/heads/main/agentic-access/weatherapi-agentic-access.yml
summary_line: 12 operations · 1 acting
tags:
- Weather
- Forecast
- History
- Marine
- Astronomy
- Geolocation
- Sports
- Alerts
- Public APIs
---
