---
acting_count: 0
action_class_counts:
  connected: 11
api_specs:
- filename: fighterapi-com-basic-lookup-api-openapi.yml
  format: yaml
  label: fighterapi-com Basic lookup API
  slug: fighterapi-com-basic-lookup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fighterapi-com/openapi/fighterapi-com-basic-lookup-api-openapi.yml
- filename: fighterapi-com-static-reference-api-openapi.yml
  format: yaml
  label: fighterapi-com Static reference API
  slug: fighterapi-com-static-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fighterapi-com/openapi/fighterapi-com-static-reference-api-openapi.yml
- filename: fighterapi-com-stats-aggregation-api-openapi.yml
  format: yaml
  label: fighterapi-com Stats + aggregation API
  slug: fighterapi-com-stats-aggregation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fighterapi-com/openapi/fighterapi-com-stats-aggregation-api-openapi.yml
- filename: fighterapi-com-time-series-api-openapi.yml
  format: yaml
  label: fighterapi-com Time Series API
  slug: fighterapi-com-time-series-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fighterapi-com/openapi/fighterapi-com-time-series-api-openapi.yml
consequence_counts:
  read: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Fighterapi Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'fighterapi-com exposes 11 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: fighterapi-com
provider_slug: fighterapi-com
slug: fighterapi-com-agentic-access
source_filename: fighterapi-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/fighterapi-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 11\n  by_consequence:\n    read: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/list_events\n  method: post\n  operationId: list_events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_event\n  method: post\n  operationId: get_event\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_schedule\n  method: post\n  operationId: get_schedule\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_fight\n  method: post\n  operationId: get_fight\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/search_fighters\n  method: post\n  operationId: search_fighters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_fighter\n  method: post\n  operationId: get_fighter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_fighter_fights\n  method: post\n  operationId: get_fighter_fights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/get_leaders\n  method: post\n  operationId: get_leaders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_ratings\n  method: post\n  operationId: get_ratings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_odds\n  method: post\n  operationId: get_odds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_line_movement\n  method: post\n  operationId: get_line_movement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/fighterapi-com/agentic-access/fighterapi-com-agentic-access.yml
summary_line: 11 operations
tags:
- Sports
- MMA
- Data
- Odds
---
