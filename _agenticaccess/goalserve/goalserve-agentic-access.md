---
acting_count: 0
action_class_counts:
  connected: 7
api_specs:
- filename: goalserve-openapi.yml
  format: yaml
  label: GoalServe Live Scores API
  slug: goalserve-live-scores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goalserve/refs/heads/main/openapi/goalserve-openapi.yml
- filename: goalserve-openapi.yml
  format: yaml
  label: GoalServe Fixtures and Schedules API
  slug: goalserve-fixtures-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goalserve/refs/heads/main/openapi/goalserve-openapi.yml
- filename: goalserve-openapi.yml
  format: yaml
  label: GoalServe Standings API
  slug: goalserve-standings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goalserve/refs/heads/main/openapi/goalserve-openapi.yml
- filename: goalserve-openapi.yml
  format: yaml
  label: GoalServe Odds API
  slug: goalserve-odds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goalserve/refs/heads/main/openapi/goalserve-openapi.yml
- filename: goalserve-openapi.yml
  format: yaml
  label: GoalServe Commentaries API
  slug: goalserve-commentaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goalserve/refs/heads/main/openapi/goalserve-openapi.yml
- filename: goalserve-openapi.yml
  format: yaml
  label: GoalServe Team and Player Data API
  slug: goalserve-team-player-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goalserve/refs/heads/main/openapi/goalserve-openapi.yml
consequence_counts:
  read: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Goalserve Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'GoalServe exposes 7 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: GoalServe
provider_slug: goalserve
slug: goalserve-agentic-access
source_filename: goalserve-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/goalserve-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 7\n  by_consequence:\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /{key}/soccernew/home\n  method: get\n  operationId: getLiveScores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{key}/soccernew/{country}\n  method: get\n  operationId: getCountryLiveScores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{key}/soccerfixtures/{country}/{cat}\n\
  \  method: get\n  operationId: getFixtures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{key}/standings/{competition}\n  method: get\n  operationId: getStandings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{key}/commentaries/{matchid}\n  method: get\n  operationId: getCommentaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{key}/soccerstats/team/{team_id}\n  method: get\n  operationId: getTeamData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{key}/soccerstats/player/{player_id}\n  method: get\n  operationId: getPlayerData\n  x-agentic-access:\n  \
  \  action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goalserve/refs/heads/main/agentic-access/goalserve-agentic-access.yml
summary_line: 7 operations
tags:
- Sports Data
- Live Scores
- Odds
- Fixtures
- Soccer
---
