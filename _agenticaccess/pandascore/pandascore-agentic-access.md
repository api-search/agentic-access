---
acting_count: 0
action_class_counts:
  connected: 19
api_specs:
- filename: pandascore-changes-api-openapi.yml
  format: yaml
  label: PandaScore Changes API
  slug: pandascore-changes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandascore/refs/heads/main/openapi/pandascore-changes-api-openapi.yml
- filename: pandascore-game-cs-go-api-openapi.yml
  format: yaml
  label: PandaScore Game - CS:GO API
  slug: pandascore-game-cs-go-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandascore/refs/heads/main/openapi/pandascore-game-cs-go-api-openapi.yml
- filename: pandascore-game-dota-2-api-openapi.yml
  format: yaml
  label: PandaScore Game - Dota 2 API
  slug: pandascore-game-dota-2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandascore/refs/heads/main/openapi/pandascore-game-dota-2-api-openapi.yml
- filename: pandascore-game-league-of-legends-api-openapi.yml
  format: yaml
  label: PandaScore Game - League of Legends API
  slug: pandascore-game-league-of-legends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandascore/refs/heads/main/openapi/pandascore-game-league-of-legends-api-openapi.yml
- filename: pandascore-game-valorant-api-openapi.yml
  format: yaml
  label: PandaScore Game - Valorant API
  slug: pandascore-game-valorant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandascore/refs/heads/main/openapi/pandascore-game-valorant-api-openapi.yml
- filename: pandascore-leagues-api-openapi.yml
  format: yaml
  label: PandaScore Leagues API
  slug: pandascore-leagues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandascore/refs/heads/main/openapi/pandascore-leagues-api-openapi.yml
- filename: pandascore-matches-api-openapi.yml
  format: yaml
  label: PandaScore Matches API
  slug: pandascore-matches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandascore/refs/heads/main/openapi/pandascore-matches-api-openapi.yml
- filename: pandascore-players-api-openapi.yml
  format: yaml
  label: PandaScore Players API
  slug: pandascore-players-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandascore/refs/heads/main/openapi/pandascore-players-api-openapi.yml
- filename: pandascore-series-api-openapi.yml
  format: yaml
  label: PandaScore Series API
  slug: pandascore-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandascore/refs/heads/main/openapi/pandascore-series-api-openapi.yml
- filename: pandascore-teams-api-openapi.yml
  format: yaml
  label: PandaScore Teams API
  slug: pandascore-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandascore/refs/heads/main/openapi/pandascore-teams-api-openapi.yml
- filename: pandascore-tournaments-api-openapi.yml
  format: yaml
  label: PandaScore Tournaments API
  slug: pandascore-tournaments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandascore/refs/heads/main/openapi/pandascore-tournaments-api-openapi.yml
consequence_counts:
  read: 19
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Pandascore Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 19
overview: 'PandaScore exposes 19 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: PandaScore
provider_slug: pandascore
slug: pandascore-agentic-access
source_filename: pandascore-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/pandascore-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    connected: 19\n  by_consequence:\n    read: 19\n  human_in_the_loop_required: 0\noperations:\n- path: /matches\n  method: get\n  operationId: listMatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /matches/past\n  method: get\n  operationId: listPastMatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /matches/running\n  method: get\n  operationId: listRunningMatches\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /matches/upcoming\n  method: get\n  operationId: listUpcomingMatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /matches/{matchIdOrSlug}\n  method: get\n  operationId: getMatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leagues\n  method: get\n  operationId: listLeagues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leagues/{leagueIdOrSlug}\n  method: get\n  operationId: getLeague\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /tournaments\n  method: get\n  operationId: listTournaments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tournaments/{tournamentIdOrSlug}\n  method: get\n  operationId: getTournament\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /teams\n  method: get\n  operationId: listTeams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /players\n  method: get\n  operationId: listPlayers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /series\n  method: get\n  operationId: listSeries\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /additions\n  method: get\n  operationId: getAdditions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /changes\n  method: get\n  operationId: getChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /incidents\n  method: get\n  operationId: getIncidents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lol/matches\n  method: get\n  operationId: listLolMatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /csgo/matches\n  method: get\n  operationId: listCsgoMatches\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /valorant/matches\n  method: get\n  operationId: listValorantMatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dota2/matches\n  method: get\n  operationId: listDota2Matches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pandascore/refs/heads/main/agentic-access/pandascore-agentic-access.yml
summary_line: 19 operations
tags:
- Esports
- Odds
- Betting
- Live Data
- Stats
- Fantasy
- WebSocket
- REST
---
