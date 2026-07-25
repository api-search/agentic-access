---
acting_count: 0
action_class_counts:
  connected: 11
api_specs:
- filename: sportsgameodds-account-api-openapi.yml
  format: yaml
  label: SportsGameOdds Account API
  slug: sportsgameodds-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsgameodds/refs/heads/main/openapi/sportsgameodds-account-api-openapi.yml
- filename: sportsgameodds-events-api-openapi.yml
  format: yaml
  label: SportsGameOdds Events API
  slug: sportsgameodds-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsgameodds/refs/heads/main/openapi/sportsgameodds-events-api-openapi.yml
- filename: sportsgameodds-leagues-api-openapi.yml
  format: yaml
  label: SportsGameOdds Leagues API
  slug: sportsgameodds-leagues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsgameodds/refs/heads/main/openapi/sportsgameodds-leagues-api-openapi.yml
- filename: sportsgameodds-markets-api-openapi.yml
  format: yaml
  label: SportsGameOdds Markets API
  slug: sportsgameodds-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsgameodds/refs/heads/main/openapi/sportsgameodds-markets-api-openapi.yml
- filename: sportsgameodds-players-api-openapi.yml
  format: yaml
  label: SportsGameOdds Players API
  slug: sportsgameodds-players-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsgameodds/refs/heads/main/openapi/sportsgameodds-players-api-openapi.yml
- filename: sportsgameodds-sports-api-openapi.yml
  format: yaml
  label: SportsGameOdds Sports API
  slug: sportsgameodds-sports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsgameodds/refs/heads/main/openapi/sportsgameodds-sports-api-openapi.yml
- filename: sportsgameodds-stats-api-openapi.yml
  format: yaml
  label: SportsGameOdds Stats API
  slug: sportsgameodds-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsgameodds/refs/heads/main/openapi/sportsgameodds-stats-api-openapi.yml
- filename: sportsgameodds-teams-api-openapi.yml
  format: yaml
  label: SportsGameOdds Teams API
  slug: sportsgameodds-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsgameodds/refs/heads/main/openapi/sportsgameodds-teams-api-openapi.yml
consequence_counts:
  read: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sportsgameodds Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'SportsGameOdds exposes 11 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SportsGameOdds
provider_slug: sportsgameodds
slug: sportsgameodds-agentic-access
source_filename: sportsgameodds-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/sportsgameodds-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 11\n  by_consequence:\n    read: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /events/\n  method: get\n  operationId: listEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{eventId}\n  method: get\n  operationId: getEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /teams/\n  method: get\n  operationId: listTeams\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /teams/{teamId}\n  method: get\n  operationId: getTeam\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /players/\n  method: get\n  operationId: listPlayers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /players/{playerId}\n  method: get\n  operationId: getPlayer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sports/\n  method: get\n  operationId: listSports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leagues/\n  method: get\n\
  \  operationId: listLeagues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats/\n  method: get\n  operationId: listStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/\n  method: get\n  operationId: listMarkets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/usage/\n  method: get\n  operationId: getAccountUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sportsgameodds/refs/heads/main/agentic-access/sportsgameodds-agentic-access.yml
summary_line: 11 operations
tags:
- Sports Betting
- Odds
- Sports Data
- Fantasy Sports
- Gambling
---
