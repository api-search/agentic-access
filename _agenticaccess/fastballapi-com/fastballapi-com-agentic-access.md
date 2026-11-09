---
acting_count: 0
action_class_counts:
  connected: 20
api_specs:
- filename: fastballapi-com-basic-lookup-api-openapi.yml
  format: yaml
  label: fastballapi-com Basic lookup API
  slug: fastballapi-com-basic-lookup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fastballapi-com/openapi/fastballapi-com-basic-lookup-api-openapi.yml
- filename: fastballapi-com-multi-table-api-openapi.yml
  format: yaml
  label: fastballapi-com Multi Table API
  slug: fastballapi-com-multi-table-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fastballapi-com/openapi/fastballapi-com-multi-table-api-openapi.yml
- filename: fastballapi-com-static-reference-api-openapi.yml
  format: yaml
  label: fastballapi-com Static reference API
  slug: fastballapi-com-static-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fastballapi-com/openapi/fastballapi-com-static-reference-api-openapi.yml
- filename: fastballapi-com-stats-aggregation-api-openapi.yml
  format: yaml
  label: fastballapi-com Stats + aggregation API
  slug: fastballapi-com-stats-aggregation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fastballapi-com/openapi/fastballapi-com-stats-aggregation-api-openapi.yml
- filename: fastballapi-com-time-series-api-openapi.yml
  format: yaml
  label: fastballapi-com Time Series API
  slug: fastballapi-com-time-series-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fastballapi-com/openapi/fastballapi-com-time-series-api-openapi.yml
consequence_counts:
  read: 20
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Fastballapi Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 20
overview: 'fastballapi-com exposes 20 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: fastballapi-com
provider_slug: fastballapi-com
slug: fastballapi-com-agentic-access
source_filename: fastballapi-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/fastballapi-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    connected: 20\n  by_consequence:\n    read: 20\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/list_teams\n  method: post\n  operationId: list_teams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_games\n  method: post\n  operationId: get_games\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_schedule\n  method: post\n  operationId: get_schedule\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_game\n  method: post\n  operationId: get_game\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_standings\n  method: post\n  operationId: get_standings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_injuries\n  method: post\n  operationId: get_injuries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/search_players\n  method: post\n  operationId: search_players\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n- path: /v1/get_player\n  method: post\n  operationId: get_player\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_player_games\n  method: post\n  operationId: get_player_games\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_leaders\n  method: post\n  operationId: get_leaders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_team_stats\n  method: post\n  operationId: get_team_stats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_plate_appearances\n  method: post\n  operationId: get_plate_appearances\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_pitches\n  method: post\n  operationId: get_pitches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_pitch_mix\n  method: post\n  operationId: get_pitch_mix\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_spray_chart\n  method: post\n  operationId: get_spray_chart\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_odds\n  method: post\n  operationId: get_odds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/get_line_movement\n  method: post\n  operationId: get_line_movement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_ratings\n  method: post\n  operationId: get_ratings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_player_props\n  method: post\n  operationId: get_player_props\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_prop_history\n  method: post\n  operationId: get_prop_history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/fastballapi-com/agentic-access/fastballapi-com-agentic-access.yml
summary_line: 20 operations
tags:
- Baseball
- Sports
- Data
- MLB
---
