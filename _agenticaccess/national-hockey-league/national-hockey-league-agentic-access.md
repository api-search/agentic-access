---
acting_count: 0
action_class_counts:
  connected: 15
api_specs:
- filename: national-hockey-league-openapi.yml
  format: yaml
  label: NHL Web API
  slug: nhl-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-hockey-league/refs/heads/main/openapi/national-hockey-league-openapi.yml
consequence_counts:
  read: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: National Hockey League Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'National Hockey League exposes 15 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: National Hockey League
provider_slug: national-hockey-league
slug: national-hockey-league-agentic-access
source_filename: national-hockey-league-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/national-hockey-league-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 15\n  by_consequence:\n    read: 15\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/schedule/now\n  method: get\n  operationId: getScheduleNow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/score/now\n  method: get\n  operationId: getScoreNow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/score/{date}\n  method: get\n  operationId:\
  \ getScoreByDate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/standings/now\n  method: get\n  operationId: getStandingsNow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/standings/{date}\n  method: get\n  operationId: getStandingsByDate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/roster/{team}/current\n  method: get\n  operationId: getRosterCurrent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/roster/{team}/{season}\n  method: get\n  operationId: getRosterBySeason\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/club-stats/{team}/now\n  method: get\n  operationId: getClubStatsNow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/club-schedule-season/{team}/now\n  method: get\n  operationId: getClubScheduleSeasonNow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/player/{player}/landing\n  method: get\n  operationId: getPlayerLanding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/player/{player}/game-log/{season}/{game-type}\n  method: get\n  operationId: getPlayerGameLog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/skater-stats-leaders/current\n  method: get\n  operationId: getSkaterStatsLeadersCurrent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/goalie-stats-leaders/current\n  method: get\n  operationId: getGoalieStatsLeadersCurrent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/gamecenter/{game-id}/boxscore\n  method: get\n  operationId: getBoxscore\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/gamecenter/{game-id}/play-by-play\n  method: get\n  operationId: getPlayByPlay\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-hockey-league/refs/heads/main/agentic-access/national-hockey-league-agentic-access.yml
summary_line: 15 operations
tags:
- Sports
- Hockey
- Entertainment
- Professional League
---
