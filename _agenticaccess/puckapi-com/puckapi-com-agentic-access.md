---
acting_count: 0
action_class_counts:
  connected: 22
api_specs:
- filename: puckapi-com-basic-lookup-api-openapi.yml
  format: yaml
  label: puckapi-com Basic lookup API
  slug: puckapi-com-basic-lookup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/puckapi-com/openapi/puckapi-com-basic-lookup-api-openapi.yml
- filename: puckapi-com-model-projections-api-openapi.yml
  format: yaml
  label: puckapi-com Model projections API
  slug: puckapi-com-model-projections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/puckapi-com/openapi/puckapi-com-model-projections-api-openapi.yml
- filename: puckapi-com-multi-table-api-openapi.yml
  format: yaml
  label: puckapi-com Multi Table API
  slug: puckapi-com-multi-table-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/puckapi-com/openapi/puckapi-com-multi-table-api-openapi.yml
- filename: puckapi-com-static-reference-api-openapi.yml
  format: yaml
  label: puckapi-com Static reference API
  slug: puckapi-com-static-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/puckapi-com/openapi/puckapi-com-static-reference-api-openapi.yml
- filename: puckapi-com-stats-aggregation-api-openapi.yml
  format: yaml
  label: puckapi-com Stats + aggregation API
  slug: puckapi-com-stats-aggregation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/puckapi-com/openapi/puckapi-com-stats-aggregation-api-openapi.yml
- filename: puckapi-com-time-series-api-openapi.yml
  format: yaml
  label: puckapi-com Time Series API
  slug: puckapi-com-time-series-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/puckapi-com/openapi/puckapi-com-time-series-api-openapi.yml
consequence_counts:
  read: 22
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Puckapi Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 22
overview: 'puckapi-com exposes 22 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: puckapi-com
provider_slug: puckapi-com
slug: puckapi-com-agentic-access
source_filename: puckapi-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/mcp-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 22\n  by_consequence:\n    read: 22\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/get_standings\n  method: post\n  operationId: get_standings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_team_stats\n  method: post\n  operationId: get_team_stats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/list_teams\n  method: post\n  operationId: list_teams\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_games\n  method: post\n  operationId: get_games\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_schedule\n  method: post\n  operationId: get_schedule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_game_detail\n  method: post\n  operationId: get_game_detail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_head_to_head\n  method: post\n  operationId: get_head_to_head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/search_players\n  method: post\n  operationId: search_players\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_player_stats\n  method: post\n  operationId: get_player_stats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_goalie_stats\n  method: post\n  operationId: get_goalie_stats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_skater_season_stats\n  method: post\n  operationId: get_skater_season_stats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_player_game_log\n  method: post\n  operationId: get_player_game_log\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_odds\n  method: post\n  operationId: get_odds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_line_movement\n  method: post\n  operationId: get_line_movement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_player_props\n  method: post\n  operationId: get_player_props\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_prop_history\n  method: post\n  operationId: get_prop_history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n    \
  \  max-ttl: 3600\n    audit: none\n- path: /v1/get_plays\n  method: post\n  operationId: get_plays\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_shot_map\n  method: post\n  operationId: get_shot_map\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_shifts\n  method: post\n  operationId: get_shifts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_situation_time\n  method: post\n  operationId: get_situation_time\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_predictions\n  method: post\n  operationId: get_predictions\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_prop_projections\n  method: post\n  operationId: get_prop_projections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/puckapi-com/agentic-access/puckapi-com-agentic-access.yml
summary_line: 22 operations
tags:
- Sports
- Hockey
- Data
- Statistics
---
