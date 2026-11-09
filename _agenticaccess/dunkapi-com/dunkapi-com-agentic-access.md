---
acting_count: 0
action_class_counts:
  connected: 18
api_specs:
- filename: dunkapi-com-basic-lookup-api-openapi.yml
  format: yaml
  label: dunkapi-com Basic lookup API
  slug: dunkapi-com-basic-lookup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dunkapi-com/openapi/dunkapi-com-basic-lookup-api-openapi.yml
- filename: dunkapi-com-multi-table-api-openapi.yml
  format: yaml
  label: dunkapi-com Multi Table API
  slug: dunkapi-com-multi-table-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dunkapi-com/openapi/dunkapi-com-multi-table-api-openapi.yml
- filename: dunkapi-com-static-reference-api-openapi.yml
  format: yaml
  label: dunkapi-com Static reference API
  slug: dunkapi-com-static-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dunkapi-com/openapi/dunkapi-com-static-reference-api-openapi.yml
- filename: dunkapi-com-stats-aggregation-api-openapi.yml
  format: yaml
  label: dunkapi-com Stats + aggregation API
  slug: dunkapi-com-stats-aggregation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dunkapi-com/openapi/dunkapi-com-stats-aggregation-api-openapi.yml
- filename: dunkapi-com-time-series-api-openapi.yml
  format: yaml
  label: dunkapi-com Time Series API
  slug: dunkapi-com-time-series-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dunkapi-com/openapi/dunkapi-com-time-series-api-openapi.yml
consequence_counts:
  read: 18
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Dunkapi Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 18
overview: 'dunkapi-com exposes 18 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: dunkapi-com
provider_slug: dunkapi-com
slug: dunkapi-com-agentic-access
source_filename: dunkapi-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/mcp-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    connected: 18\n  by_consequence:\n    read: 18\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/list_teams\n  method: post\n  operationId: list_teams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/list_games\n  method: post\n  operationId: list_games\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_schedule\n  method: post\n  operationId: get_schedule\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_game\n  method: post\n  operationId: get_game\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_standings\n  method: post\n  operationId: get_standings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_injuries\n  method: post\n  operationId: get_injuries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/search_players\n  method: post\n  operationId: search_players\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/get_player\n  method: post\n  operationId: get_player\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_player_games\n  method: post\n  operationId: get_player_games\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_leaders\n  method: post\n  operationId: get_leaders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_team_stats\n  method: post\n  operationId: get_team_stats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_plays\n  method: post\n  operationId: get_plays\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_shot_chart\n  method: post\n  operationId: get_shot_chart\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_odds\n  method: post\n  operationId: get_odds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_line_movement\n  method: post\n  operationId: get_line_movement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_ratings\n  method: post\n  operationId: get_ratings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_player_props\n  method: post\n\
  \  operationId: get_player_props\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_prop_history\n  method: post\n  operationId: get_prop_history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/dunkapi-com/agentic-access/dunkapi-com-agentic-access.yml
summary_line: 18 operations
tags:
- Company
- Sports
- Basketball
- NBA
- Data
---
