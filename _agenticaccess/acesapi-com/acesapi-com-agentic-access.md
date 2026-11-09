---
acting_count: 0
action_class_counts:
  connected: 13
api_specs:
- filename: acesapi-com-basic-lookup-api-openapi.yml
  format: yaml
  label: acesapi-com Basic lookup API
  slug: acesapi-com-basic-lookup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/acesapi-com/openapi/acesapi-com-basic-lookup-api-openapi.yml
- filename: acesapi-com-multi-table-api-openapi.yml
  format: yaml
  label: acesapi-com Multi Table API
  slug: acesapi-com-multi-table-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/acesapi-com/openapi/acesapi-com-multi-table-api-openapi.yml
- filename: acesapi-com-static-reference-api-openapi.yml
  format: yaml
  label: acesapi-com Static reference API
  slug: acesapi-com-static-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/acesapi-com/openapi/acesapi-com-static-reference-api-openapi.yml
- filename: acesapi-com-stats-aggregation-api-openapi.yml
  format: yaml
  label: acesapi-com Stats + aggregation API
  slug: acesapi-com-stats-aggregation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/acesapi-com/openapi/acesapi-com-stats-aggregation-api-openapi.yml
consequence_counts:
  read: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Acesapi Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'acesapi-com exposes 13 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: acesapi-com
provider_slug: acesapi-com
slug: acesapi-com-agentic-access
source_filename: acesapi-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/acesapi-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 13\n  by_consequence:\n    read: 13\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/list_tournaments\n  method: post\n  operationId: list_tournaments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_tournament\n  method: post\n  operationId: get_tournament\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_matches\n  method: post\n  operationId:\
  \ get_matches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_schedule\n  method: post\n  operationId: get_schedule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_match\n  method: post\n  operationId: get_match\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/search_players\n  method: post\n  operationId: search_players\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_player\n  method: post\n  operationId: get_player\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/get_player_matches\n  method: post\n  operationId: get_player_matches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_head_to_head\n  method: post\n  operationId: get_head_to_head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_surface_splits\n  method: post\n  operationId: get_surface_splits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_player_stats\n  method: post\n  operationId: get_player_stats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_rankings\n  method: post\n  operationId: get_rankings\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get_ratings\n  method: post\n  operationId: get_ratings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/acesapi-com/agentic-access/acesapi-com-agentic-access.yml
summary_line: 13 operations
tags:
- Tennis
- Sports
- Data
- MCP
- Rankings
---
