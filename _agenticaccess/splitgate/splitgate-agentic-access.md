---
acting_count: 0
action_class_counts:
  connected: 5
api_specs:
- filename: splitgate-matches-api-openapi.yml
  format: yaml
  label: Splitgate Matches API
  slug: splitgate-matches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splitgate/refs/heads/main/openapi/splitgate-matches-api-openapi.yml
- filename: splitgate-players-api-openapi.yml
  format: yaml
  label: Splitgate Players API
  slug: splitgate-players-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splitgate/refs/heads/main/openapi/splitgate-players-api-openapi.yml
consequence_counts:
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Splitgate Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Splitgate exposes 5 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Splitgate
provider_slug: splitgate
slug: splitgate-agentic-access
source_filename: splitgate-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: generated\nsource: openapi/splitgate-third-party-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 5\n  by_consequence:\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/search/players\n  method: get\n  operationId: searchPlayers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/game/splitgate2/players/{playerId}/stats\n  method: get\n  operationId: getPlayerStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/game/splitgate2/players/{playerId}/ranks\n\
  \  method: get\n  operationId: getPlayerRanks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/game/splitgate2/players/{playerId}/matches\n  method: get\n  operationId: getPlayerMatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/game/splitgate2/matches/{matchId}\n  method: get\n  operationId: getMatchDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/splitgate/refs/heads/main/agentic-access/splitgate-agentic-access.yml
summary_line: 5 operations
tags:
- Company
- Gaming
- Video Games
- Esports
- Player Statistics
- Leaderboards
- Match Data
- Entertainment
---
