---
acting_count: 0
action_class_counts:
  connected: 8
api_specs:
- filename: wunderground-pws-api.yml
  format: yaml
  label: Weather Underground PWS API
  slug: weather-underground-pws-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wunderground/refs/heads/main/openapi/wunderground-pws-api.yml
consequence_counts:
  read: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Wunderground Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Weather Underground exposes 8 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Weather Underground
provider_slug: wunderground
slug: wunderground-agentic-access
source_filename: wunderground-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/wunderground-pws-api.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 8\n  by_consequence:\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/pws/observations/current\n  method: get\n  operationId: getCurrentObservations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/pws/observations/all/1day\n  method: get\n  operationId: getAllObservations1Day\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/pws/observations/hourly/7day\n\
  \  method: get\n  operationId: getHourlyObservations7Day\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/pws/dailysummary/7day\n  method: get\n  operationId: getDailySummary7Day\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/pws/history/all\n  method: get\n  operationId: getHistoryAllForDate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/pws/history/daily\n  method: get\n  operationId: getHistoryDaily\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/wx/forecast/daily/5day\n  method: get\n  operationId: get5DayForecast\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/location/near\n  method: get\n  operationId: getNearbyPWSLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wunderground/refs/heads/main/agentic-access/wunderground-agentic-access.yml
summary_line: 8 operations
tags:
- Weather
- Personal Weather Stations
- Hyperlocal
- Observations
- Forecasts
- Historical Data
- REST API
---
