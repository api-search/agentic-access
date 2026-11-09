---
acting_count: 0
action_class_counts:
  connected: 20
api_specs:
- filename: endzoneapi-com-basic-lookup-api-openapi.yml
  format: yaml
  label: endzoneapi-com Basic lookup API
  slug: endzoneapi-com-basic-lookup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/endzoneapi-com/openapi/endzoneapi-com-basic-lookup-api-openapi.yml
- filename: endzoneapi-com-multi-table-api-openapi.yml
  format: yaml
  label: endzoneapi-com Multi Table API
  slug: endzoneapi-com-multi-table-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/endzoneapi-com/openapi/endzoneapi-com-multi-table-api-openapi.yml
- filename: endzoneapi-com-static-reference-api-openapi.yml
  format: yaml
  label: endzoneapi-com Static reference API
  slug: endzoneapi-com-static-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/endzoneapi-com/openapi/endzoneapi-com-static-reference-api-openapi.yml
- filename: endzoneapi-com-stats-aggregation-api-openapi.yml
  format: yaml
  label: endzoneapi-com Stats + aggregation API
  slug: endzoneapi-com-stats-aggregation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/endzoneapi-com/openapi/endzoneapi-com-stats-aggregation-api-openapi.yml
- filename: endzoneapi-com-time-series-api-openapi.yml
  format: yaml
  label: endzoneapi-com Time Series API
  slug: endzoneapi-com-time-series-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/endzoneapi-com/openapi/endzoneapi-com-time-series-api-openapi.yml
consequence_counts:
  read: 20
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Endzoneapi Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 20
overview: 'endzoneapi-com exposes 20 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: endzoneapi-com
provider_slug: endzoneapi-com
slug: endzoneapi-com-agentic-access
source_filename: endzoneapi-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/endzoneapi-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    connected: 20\n  by_consequence:\n    read: 20\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/list_teams\n  method: post\n  operationId: list_teams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_standings\n  method: post\n  operationId: get_standings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_team_stats\n  method: post\n  operationId: get_team_stats\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_games\n  method: post\n  operationId: get_games\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_schedule\n  method: post\n  operationId: get_schedule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_game_detail\n  method: post\n  operationId: get_game_detail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_head_to_head\n  method: post\n  operationId: get_head_to_head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/search_players\n  method: post\n  operationId: search_players\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_player_stats\n  method: post\n  operationId: get_player_stats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_player_leaders\n  method: post\n  operationId: get_player_leaders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_injuries\n  method: post\n  operationId: get_injuries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_depth_chart\n  method: post\n  operationId: get_depth_chart\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_snap_counts\n  method: post\n  operationId: get_snap_counts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_plays\n  method: post\n  operationId: get_plays\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_advanced_stats\n  method: post\n  operationId: get_advanced_stats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_odds\n  method: post\n  operationId: get_odds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /v1/get_line_movement\n  method: post\n  operationId: get_line_movement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_player_props\n  method: post\n  operationId: get_player_props\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_prop_history\n  method: post\n  operationId: get_prop_history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_alt_lines\n  method: post\n  operationId: get_alt_lines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/endzoneapi-com/agentic-access/endzoneapi-com-agentic-access.yml
summary_line: 20 operations
tags:
- Sports
- Football
- NFL
- Data API
- Odds
- MCP
---
