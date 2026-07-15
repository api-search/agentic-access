---
acting_count: 0
action_class_counts:
  connected: 24
api_specs:
- filename: highlightly-openapi.yml
  format: yaml
  label: Highlightly Matches & Fixtures API
  slug: matches-fixtures
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highlightly/refs/heads/main/openapi/highlightly-openapi.yml
- filename: highlightly-openapi.yml
  format: yaml
  label: Highlightly Live Scores API
  slug: live-scores
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highlightly/refs/heads/main/openapi/highlightly-openapi.yml
- filename: highlightly-openapi.yml
  format: yaml
  label: Highlightly Standings API
  slug: standings
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highlightly/refs/heads/main/openapi/highlightly-openapi.yml
- filename: highlightly-openapi.yml
  format: yaml
  label: Highlightly Statistics API
  slug: statistics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highlightly/refs/heads/main/openapi/highlightly-openapi.yml
- filename: highlightly-openapi.yml
  format: yaml
  label: Highlightly Odds API
  slug: odds
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highlightly/refs/heads/main/openapi/highlightly-openapi.yml
- filename: highlightly-openapi.yml
  format: yaml
  label: Highlightly Highlights API
  slug: highlights
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highlightly/refs/heads/main/openapi/highlightly-openapi.yml
consequence_counts:
  read: 24
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Highlightly Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 24
overview: 'Highlightly exposes 24 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 24 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Highlightly
provider_slug: highlightly
slug: highlightly-agentic-access
source_filename: highlightly-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/highlightly-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 24\n  by_action_class:\n    connected: 24\n  by_consequence:\n    read: 24\n  human_in_the_loop_required: 0\noperations:\n- path: /football/countries\n  method: get\n  operationId: listFootballCountries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /football/countries/{countryCode}\n  method: get\n  operationId: getFootballCountry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /football/leagues\n  method:\
  \ get\n  operationId: listFootballLeagues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /football/leagues/{id}\n  method: get\n  operationId: getFootballLeague\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /football/teams\n  method: get\n  operationId: listFootballTeams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /football/teams/{id}\n  method: get\n  operationId: getFootballTeam\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /football/teams/statistics/{id}\n  method: get\n  operationId: getFootballTeamStatistics\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /football/matches\n  method: get\n  operationId: listFootballMatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /football/matches/{id}\n  method: get\n  operationId: getFootballMatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /football/highlights\n  method: get\n  operationId: listFootballHighlights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /football/highlights/{id}\n  method: get\n  operationId: getFootballHighlight\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /football/highlights/geo-restrictions/{id}\n  method: get\n  operationId: getFootballHighlightGeoRestrictions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /football/bookmakers\n  method: get\n  operationId: listFootballBookmakers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /football/bookmakers/{id}\n  method: get\n  operationId: getFootballBookmaker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /football/odds\n  method: get\n  operationId: listFootballOdds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /football/standings\n  method: get\n \
  \ operationId: getFootballStandings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /football/last-five-games\n  method: get\n  operationId: getFootballLastFiveGames\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /football/head-2-head\n  method: get\n  operationId: getFootballHeadToHead\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /football/lineups/{matchId}\n  method: get\n  operationId: getFootballLineups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /football/statistics/{matchId}\n  method: get\n  operationId: getFootballMatchStatistics\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /football/events/{id}\n  method: get\n  operationId: getFootballEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /football/players\n  method: get\n  operationId: listFootballPlayers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /football/players/{id}\n  method: get\n  operationId: getFootballPlayer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /football/players/{id}/statistics\n  method: get\n  operationId: getFootballPlayerStatistics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/highlightly/refs/heads/main/agentic-access/highlightly-agentic-access.yml
summary_line: 24 operations
tags:
- Sports
- Sports Data
- Live Scores
- Odds
- Highlights
---
