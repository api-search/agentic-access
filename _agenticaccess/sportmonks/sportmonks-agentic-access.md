---
acting_count: 0
action_class_counts:
  connected: 17
api_specs:
- filename: postman.yaml
  format: yaml
  label: Sportmonks Cricket API
  slug: cricket-api
  spec_type: Postman
  url: https://cricket-postman.sportmonks.com/
- filename: sportmonks-fixtures-api-openapi.yml
  format: yaml
  label: Sportmonks Fixtures API
  slug: sportmonks-fixtures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportmonks/refs/heads/main/openapi/sportmonks-fixtures-api-openapi.yml
- filename: sportmonks-leagues-api-openapi.yml
  format: yaml
  label: Sportmonks Leagues API
  slug: sportmonks-leagues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportmonks/refs/heads/main/openapi/sportmonks-leagues-api-openapi.yml
- filename: sportmonks-livescores-api-openapi.yml
  format: yaml
  label: Sportmonks Livescores API
  slug: sportmonks-livescores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportmonks/refs/heads/main/openapi/sportmonks-livescores-api-openapi.yml
- filename: sportmonks-odds-api-openapi.yml
  format: yaml
  label: Sportmonks Odds API
  slug: sportmonks-odds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportmonks/refs/heads/main/openapi/sportmonks-odds-api-openapi.yml
- filename: sportmonks-players-api-openapi.yml
  format: yaml
  label: Sportmonks Players API
  slug: sportmonks-players-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportmonks/refs/heads/main/openapi/sportmonks-players-api-openapi.yml
- filename: sportmonks-predictions-api-openapi.yml
  format: yaml
  label: Sportmonks Predictions API
  slug: sportmonks-predictions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportmonks/refs/heads/main/openapi/sportmonks-predictions-api-openapi.yml
- filename: sportmonks-schedules-api-openapi.yml
  format: yaml
  label: Sportmonks Schedules API
  slug: sportmonks-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportmonks/refs/heads/main/openapi/sportmonks-schedules-api-openapi.yml
- filename: sportmonks-seasons-api-openapi.yml
  format: yaml
  label: Sportmonks Seasons API
  slug: sportmonks-seasons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportmonks/refs/heads/main/openapi/sportmonks-seasons-api-openapi.yml
- filename: sportmonks-standings-api-openapi.yml
  format: yaml
  label: Sportmonks Standings API
  slug: sportmonks-standings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportmonks/refs/heads/main/openapi/sportmonks-standings-api-openapi.yml
- filename: sportmonks-teams-api-openapi.yml
  format: yaml
  label: Sportmonks Teams API
  slug: sportmonks-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportmonks/refs/heads/main/openapi/sportmonks-teams-api-openapi.yml
consequence_counts:
  read: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sportmonks Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'Sportmonks exposes 17 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Sportmonks
provider_slug: sportmonks
slug: sportmonks-agentic-access
source_filename: sportmonks-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/sportmonks-football-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    connected: 17\n  by_consequence:\n    read: 17\n  human_in_the_loop_required: 0\noperations:\n- path: /livescores\n  method: get\n  operationId: listLivescores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /livescores/inplay\n  method: get\n  operationId: listInplayLivescores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fixtures\n  method: get\n  operationId: listFixtures\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fixtures/{id}\n  method: get\n  operationId: getFixture\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fixtures/date/{date}\n  method: get\n  operationId: listFixturesByDate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leagues\n  method: get\n  operationId: listLeagues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leagues/{id}\n  method: get\n  operationId: getLeague\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /seasons\n  method: get\n  operationId: listSeasons\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /standings/seasons/{seasonId}\n  method: get\n  operationId: getStandingsBySeason\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /teams\n  method: get\n  operationId: listTeams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /teams/{id}\n  method: get\n  operationId: getTeam\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /players\n  method: get\n  operationId: listPlayers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /players/{id}\n  method: get\n  operationId: getPlayer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /predictions/probabilities/fixtures/{fixtureId}\n  method: get\n  operationId: getPredictionByFixture\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /odds/pre-match/fixtures/{fixtureId}\n  method: get\n  operationId: getPreMatchOddsByFixture\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /odds/inplay/fixtures/{fixtureId}\n  method: get\n  operationId: getInplayOddsByFixture\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /schedules/seasons/{seasonId}\n  method: get\n  operationId: getScheduleBySeason\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sportmonks/refs/heads/main/agentic-access/sportmonks-agentic-access.yml
summary_line: 17 operations
tags:
- Cricket
- Data
- Developer-Friendly
- Football
- Formula 1
- Live Scores
- Motorsport
- Real-Time
- Soccer
- Sports
- Sports Data
- Statistics
---
