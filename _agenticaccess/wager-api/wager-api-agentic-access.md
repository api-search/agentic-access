---
acting_count: 0
action_class_counts:
  connected: 9
api_specs:
- filename: wager-api-openapi.yml
  format: yaml
  label: Wager API - Sports Odds
  slug: wager-api-odds
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wager-api/refs/heads/main/openapi/wager-api-openapi.yml
- filename: wager-api-openapi.yml
  format: yaml
  label: Wager API - Fantasy Sports Data
  slug: wager-api-fantasy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wager-api/refs/heads/main/openapi/wager-api-openapi.yml
consequence_counts:
  read: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Wager Api Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'Wager API exposes 9 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Wager API
provider_slug: wager-api
slug: wager-api-agentic-access
source_filename: wager-api-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/wager-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 9\n  by_consequence:\n    read: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/odds\n  method: get\n  operationId: getGameOdds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/props\n  method: get\n  operationId: getPlayerProps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/futures\n  method: get\n  operationId: getFuturesOdds\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/players\n  method: get\n  operationId: getPlayers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/players/{playerId}/stats\n  method: get\n  operationId: getPlayerStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/players/{playerId}/projections\n  method: get\n  operationId: getPlayerProjections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/injuries\n  method: get\n  operationId: getInjuryReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/games\n  method: get\n  operationId: getGames\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/depth-charts\n  method: get\n  operationId: getDepthCharts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wager-api/refs/heads/main/agentic-access/wager-api-agentic-access.yml
summary_line: 9 operations
tags:
- Sports Betting
- Sports Odds
- Fantasy Sports
- Sports Data
- NFL
- NBA
- MLB
- NHL
- NCAA
---
