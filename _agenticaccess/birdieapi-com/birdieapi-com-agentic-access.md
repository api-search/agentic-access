---
acting_count: 0
action_class_counts:
  connected: 14
api_specs:
- filename: birdieapi-com-basic-lookup-api-openapi.yml
  format: yaml
  label: birdieapi-com Basic lookup API
  slug: birdieapi-com-basic-lookup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/birdieapi-com/openapi/birdieapi-com-basic-lookup-api-openapi.yml
- filename: birdieapi-com-static-reference-api-openapi.yml
  format: yaml
  label: birdieapi-com Static reference API
  slug: birdieapi-com-static-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/birdieapi-com/openapi/birdieapi-com-static-reference-api-openapi.yml
- filename: birdieapi-com-stats-aggregation-api-openapi.yml
  format: yaml
  label: birdieapi-com Stats + aggregation API
  slug: birdieapi-com-stats-aggregation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/birdieapi-com/openapi/birdieapi-com-stats-aggregation-api-openapi.yml
- filename: birdieapi-com-time-series-api-openapi.yml
  format: yaml
  label: birdieapi-com Time Series API
  slug: birdieapi-com-time-series-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/birdieapi-com/openapi/birdieapi-com-time-series-api-openapi.yml
consequence_counts:
  read: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Birdieapi Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'birdieapi-com exposes 14 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: birdieapi-com
provider_slug: birdieapi-com
slug: birdieapi-com-agentic-access
source_filename: birdieapi-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/birdieapi-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 14\n  by_consequence:\n    read: 14\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/list_tournaments\n  method: post\n  operationId: list_tournaments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_schedule\n  method: post\n  operationId: get_schedule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_leaderboard\n  method: post\n  operationId:\
  \ get_leaderboard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_course\n  method: post\n  operationId: get_course\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/search_players\n  method: post\n  operationId: search_players\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_player\n  method: post\n  operationId: get_player\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_player_results\n  method: post\n  operationId: get_player_results\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/get_player_stats\n  method: post\n  operationId: get_player_stats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_scorecard\n  method: post\n  operationId: get_scorecard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_course_history\n  method: post\n  operationId: get_course_history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_head_to_head\n  method: post\n  operationId: get_head_to_head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_ratings\n  method: post\n  operationId: get_ratings\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_leaders\n  method: post\n  operationId: get_leaders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_winner_odds\n  method: post\n  operationId: get_winner_odds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/birdieapi-com/agentic-access/birdieapi-com-agentic-access.yml
summary_line: 14 operations
tags:
- Company
- Bird Tracking
- Migration Analytics
- Open Data
- Conservation
---
