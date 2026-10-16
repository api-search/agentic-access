---
acting_count: 0
action_class_counts:
  connected: 15
api_specs:
- filename: 5dollarfootballapi-bookmakers-api-openapi.yml
  format: yaml
  label: 5DollarFootballAPI Bookmakers API
  slug: 5dollarfootballapi-bookmakers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/5dollarfootballapi/refs/heads/main/openapi/5dollarfootballapi-bookmakers-api-openapi.yml
- filename: 5dollarfootballapi-countries-api-openapi.yml
  format: yaml
  label: 5DollarFootballAPI Countries API
  slug: 5dollarfootballapi-countries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/5dollarfootballapi/refs/heads/main/openapi/5dollarfootballapi-countries-api-openapi.yml
- filename: 5dollarfootballapi-fixtures-api-openapi.yml
  format: yaml
  label: 5DollarFootballAPI Fixtures API
  slug: 5dollarfootballapi-fixtures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/5dollarfootballapi/refs/heads/main/openapi/5dollarfootballapi-fixtures-api-openapi.yml
- filename: 5dollarfootballapi-leagues-api-openapi.yml
  format: yaml
  label: 5DollarFootballAPI Leagues API
  slug: 5dollarfootballapi-leagues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/5dollarfootballapi/refs/heads/main/openapi/5dollarfootballapi-leagues-api-openapi.yml
- filename: 5dollarfootballapi-standings-api-openapi.yml
  format: yaml
  label: 5DollarFootballAPI Standings API
  slug: 5dollarfootballapi-standings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/5dollarfootballapi/refs/heads/main/openapi/5dollarfootballapi-standings-api-openapi.yml
- filename: 5dollarfootballapi-status-api-openapi.yml
  format: yaml
  label: 5DollarFootballAPI Status API
  slug: 5dollarfootballapi-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/5dollarfootballapi/refs/heads/main/openapi/5dollarfootballapi-status-api-openapi.yml
- filename: 5dollarfootballapi-teams-api-openapi.yml
  format: yaml
  label: 5DollarFootballAPI Teams API
  slug: 5dollarfootballapi-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/5dollarfootballapi/refs/heads/main/openapi/5dollarfootballapi-teams-api-openapi.yml
- filename: 5dollarfootballapi-bookmakers-api-openapi.yml
  format: yaml
  label: 5DollarFootballAPI Bookmakers API
  slug: 5dollarfootballapi-bookmakers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/5dollarfootballapi/refs/heads/main/openapi/5dollarfootballapi-bookmakers-api-openapi.yml
consequence_counts:
  read: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: 5Dollarfootballapi Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: '5DollarFootballAPI exposes 15 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: 5DollarFootballAPI
provider_slug: 5dollarfootballapi
slug: 5dollarfootballapi-agentic-access
source_filename: 5dollarfootballapi-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: generated\nsource: openapi/5dollarfootballapi-bookmakers-api-openapi.yml, openapi/5dollarfootballapi-countries-api-openapi.yml,\n  openapi/5dollarfootballapi-fixtures-api-openapi.yml, openapi/5dollarfootballapi-leagues-api-openapi.yml,\n  openapi/5dollarfootballapi-standings-api-openapi.yml, openapi/5dollarfootballapi-status-api-openapi.yml,\n  openapi/5dollarfootballapi-teams-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 15\n  by_consequence:\n    read: 15\n  human_in_the_loop_required: 0\noperations:\n- path: /bookmakers\n  method: get\n  operationId: bookmakers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /countries\n  method: get\n  operationId: countries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fixtures\n  method: get\n  operationId: fixtures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fixtures/{id}\n  method: get\n  operationId: fixture\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fixtures/{id}/odds\n  method: get\n  operationId: odds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fixtures/{id}/odds/history\n  method: get\n  operationId: oddsHistory\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fixtures/{id}/events\n  method: get\n  operationId: events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fixtures/{id}/statistics\n  method: get\n  operationId: statistics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leagues\n  method: get\n  operationId: leagues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leagues/{id}\n  method: get\n  operationId: league\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leagues/{id}/fixtures\n  method: get\n\
  \  operationId: leagueFixtures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /standings\n  method: get\n  operationId: standings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status\n  method: get\n  operationId: status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /teams/{id}\n  method: get\n  operationId: team\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /teams/{id}/fixtures\n  method: get\n  operationId: teamFixtures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/5dollarfootballapi/refs/heads/main/agentic-access/5dollarfootballapi-agentic-access.yml
summary_line: 15 operations
tags:
- Football
- Soccer
- Sports
- Sports Data
- Live Scores
- Fixtures
- Standings
- Statistics
- Odds
- Bookmakers
---
