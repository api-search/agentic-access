---
acting_count: 0
action_class_counts:
  connected: 11
api_specs:
- filename: crosbynews-com-air-api-openapi.yml
  format: yaml
  label: Crosby News Air API
  slug: crosbynews-com-air-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosbynews-com/openapi/crosbynews-com-air-api-openapi.yml
- filename: crosbynews-com-burn-ban-api-openapi.yml
  format: yaml
  label: Crosby News Burn Ban API
  slug: crosbynews-com-burn-ban-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosbynews-com/openapi/crosbynews-com-burn-ban-api-openapi.yml
- filename: crosbynews-com-calendar-api-openapi.yml
  format: yaml
  label: Crosby News Calendar API
  slug: crosbynews-com-calendar-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosbynews-com/openapi/crosbynews-com-calendar-api-openapi.yml
- filename: crosbynews-com-fishing-api-openapi.yml
  format: yaml
  label: Crosby News Fishing API
  slug: crosbynews-com-fishing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosbynews-com/openapi/crosbynews-com-fishing-api-openapi.yml
- filename: crosbynews-com-health-api-openapi.yml
  format: yaml
  label: Crosby News Health API
  slug: crosbynews-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosbynews-com/openapi/crosbynews-com-health-api-openapi.yml
- filename: crosbynews-com-news-api-openapi.yml
  format: yaml
  label: Crosby News News API
  slug: crosbynews-com-news-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosbynews-com/openapi/crosbynews-com-news-api-openapi.yml
- filename: crosbynews-com-pollen-api-openapi.yml
  format: yaml
  label: Crosby News Pollen API
  slug: crosbynews-com-pollen-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosbynews-com/openapi/crosbynews-com-pollen-api-openapi.yml
- filename: crosbynews-com-traffic-api-openapi.yml
  format: yaml
  label: Crosby News Traffic API
  slug: crosbynews-com-traffic-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosbynews-com/openapi/crosbynews-com-traffic-api-openapi.yml
- filename: crosbynews-com-tropics-api-openapi.yml
  format: yaml
  label: Crosby News Tropics API
  slug: crosbynews-com-tropics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosbynews-com/openapi/crosbynews-com-tropics-api-openapi.yml
- filename: crosbynews-com-water-api-openapi.yml
  format: yaml
  label: Crosby News Water API
  slug: crosbynews-com-water-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosbynews-com/openapi/crosbynews-com-water-api-openapi.yml
- filename: crosbynews-com-weather-api-openapi.yml
  format: yaml
  label: Crosby News Weather API
  slug: crosbynews-com-weather-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosbynews-com/openapi/crosbynews-com-weather-api-openapi.yml
consequence_counts:
  read: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Crosbynews Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'Crosby News exposes 11 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Crosby News
provider_slug: crosbynews-com
slug: crosbynews-com-agentic-access
source_filename: crosbynews-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/crosbynews-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 11\n  by_consequence:\n    read: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /api/weather\n  method: get\n  operationId: getWeather\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/news\n  method: get\n  operationId: getNews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/calendar\n  method: get\n  operationId: getCalendar\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/water\n  method: get\n  operationId: getWater\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/fishing\n  method: get\n  operationId: getFishing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tropics\n  method: get\n  operationId: getTropics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/pollen\n  method: get\n  operationId: getPollen\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/burn-ban\n  method: get\n \
  \ operationId: getBurnBan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/air\n  method: get\n  operationId: getAir\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/traffic\n  method: get\n  operationId: getTraffic\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/crosbynews-com/agentic-access/crosbynews-com-agentic-access.yml
summary_line: 11 operations
tags:
- Company
---
