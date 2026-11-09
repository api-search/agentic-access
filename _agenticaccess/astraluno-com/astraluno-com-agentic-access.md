---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 8
api_specs:
- filename: astraluno-com-chart-api-openapi.yml
  format: yaml
  label: Astraluno Chart API
  slug: astraluno-com-chart-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astraluno-com/openapi/astraluno-com-chart-api-openapi.yml
- filename: astraluno-com-ingresses-api-openapi.yml
  format: yaml
  label: Astraluno Ingresses API
  slug: astraluno-com-ingresses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astraluno-com/openapi/astraluno-com-ingresses-api-openapi.yml
- filename: astraluno-com-lunations-api-openapi.yml
  format: yaml
  label: Astraluno Lunations API
  slug: astraluno-com-lunations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astraluno-com/openapi/astraluno-com-lunations-api-openapi.yml
- filename: astraluno-com-openapi-json-api-openapi.yml
  format: yaml
  label: Astraluno Openapi.json API
  slug: astraluno-com-openapi-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astraluno-com/openapi/astraluno-com-openapi-json-api-openapi.yml
- filename: astraluno-com-places-api-openapi.yml
  format: yaml
  label: Astraluno Places API
  slug: astraluno-com-places-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astraluno-com/openapi/astraluno-com-places-api-openapi.yml
- filename: astraluno-com-readings-api-openapi.yml
  format: yaml
  label: Astraluno Readings API
  slug: astraluno-com-readings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astraluno-com/openapi/astraluno-com-readings-api-openapi.yml
- filename: astraluno-com-retrogrades-api-openapi.yml
  format: yaml
  label: Astraluno Retrogrades API
  slug: astraluno-com-retrogrades-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astraluno-com/openapi/astraluno-com-retrogrades-api-openapi.yml
- filename: astraluno-com-sky-api-openapi.yml
  format: yaml
  label: Astraluno Sky API
  slug: astraluno-com-sky-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astraluno-com/openapi/astraluno-com-sky-api-openapi.yml
- filename: astraluno-com-sun-sign-api-openapi.yml
  format: yaml
  label: Astraluno Sun Sign API
  slug: astraluno-com-sun-sign-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astraluno-com/openapi/astraluno-com-sun-sign-api-openapi.yml
consequence_counts:
  read: 8
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Astraluno Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'Astraluno exposes 9 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Astraluno
provider_slug: astraluno-com
slug: astraluno-com-agentic-access
source_filename: astraluno-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/astraluno-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    acting: 1\n    connected: 8\n  by_consequence:\n    write: 1\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/chart\n  method: post\n  operationId: chart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sun-sign\n  method: get\n  operationId: sun_sign\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sky\n  method: get\n  operationId: sky\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/retrogrades\n  method: get\n  operationId: retrogrades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/ingresses\n  method: get\n  operationId: ingresses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/lunations\n  method: get\n  operationId: lunations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/places\n  method: get\n  operationId: places\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/readings/{kind}/{key}\n  method: get\n  operationId: readings__kind___key_\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/openapi.json\n  method: get\n  operationId: openapi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/astraluno-com/agentic-access/astraluno-com-agentic-access.yml
summary_line: 9 operations · 1 acting
tags:
- Astrology
- BirthChart
- Horoscope
---
