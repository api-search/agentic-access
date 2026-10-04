---
acting_count: 0
action_class_counts:
  connected: 18
api_specs:
- filename: pinnacle-asyncapi.yml
  format: yaml
  label: Pinnacle Lines API
  slug: pinnacle-lines-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinnacle/refs/heads/main/openapi/pinnacle-asyncapi.yml
- filename: pinnacle-cancellationreasons-api-openapi.yml
  format: yaml
  label: ' Pinnacle Sports Betting Cancellationreasons API'
  slug: pinnacle-cancellationreasons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinnacle/refs/heads/main/openapi/pinnacle-cancellationreasons-api-openapi.yml
- filename: pinnacle-currencies-api-openapi.yml
  format: yaml
  label: ' Pinnacle Sports Betting Currencies API'
  slug: pinnacle-currencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinnacle/refs/heads/main/openapi/pinnacle-currencies-api-openapi.yml
- filename: pinnacle-fixtures-api-openapi.yml
  format: yaml
  label: ' Pinnacle Sports Betting Fixtures API'
  slug: pinnacle-fixtures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinnacle/refs/heads/main/openapi/pinnacle-fixtures-api-openapi.yml
- filename: pinnacle-inrunning-api-openapi.yml
  format: yaml
  label: ' Pinnacle Sports Betting Inrunning API'
  slug: pinnacle-inrunning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinnacle/refs/heads/main/openapi/pinnacle-inrunning-api-openapi.yml
- filename: pinnacle-leagues-api-openapi.yml
  format: yaml
  label: ' Pinnacle Sports Betting Leagues API'
  slug: pinnacle-leagues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinnacle/refs/heads/main/openapi/pinnacle-leagues-api-openapi.yml
- filename: pinnacle-line-api-openapi.yml
  format: yaml
  label: ' Pinnacle Sports Betting Line API'
  slug: pinnacle-line-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinnacle/refs/heads/main/openapi/pinnacle-line-api-openapi.yml
- filename: pinnacle-odds-api-openapi.yml
  format: yaml
  label: ' Pinnacle Sports Betting Odds API'
  slug: pinnacle-odds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinnacle/refs/heads/main/openapi/pinnacle-odds-api-openapi.yml
- filename: pinnacle-periods-api-openapi.yml
  format: yaml
  label: ' Pinnacle Sports Betting Periods API'
  slug: pinnacle-periods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinnacle/refs/heads/main/openapi/pinnacle-periods-api-openapi.yml
- filename: pinnacle-sports-api-openapi.yml
  format: yaml
  label: ' Pinnacle Sports Betting Sports API'
  slug: pinnacle-sports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinnacle/refs/heads/main/openapi/pinnacle-sports-api-openapi.yml
- filename: pinnacle-teaser-api-openapi.yml
  format: yaml
  label: ' Pinnacle Sports Betting Teaser API'
  slug: pinnacle-teaser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinnacle/refs/heads/main/openapi/pinnacle-teaser-api-openapi.yml
consequence_counts:
  read: 18
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Pinnacle Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 18
overview: 'Pinnacle Sports Betting exposes 18 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Pinnacle Sports Betting
provider_slug: pinnacle
slug: pinnacle-agentic-access
source_filename: pinnacle-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/pinnacle-cancellationreasons-api-openapi.yml, openapi/pinnacle-currencies-api-openapi.yml,\n  openapi/pinnacle-fixtures-api-openapi.yml, openapi/pinnacle-inrunning-api-openapi.yml, openapi/pinnacle-leagues-api-openapi.yml,\n  openapi/pinnacle-line-api-openapi.yml, openapi/pinnacle-odds-api-openapi.yml, openapi/pinnacle-periods-api-openapi.yml,\n  openapi/pinnacle-sports-api-openapi.yml, openapi/pinnacle-teaser-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    connected: 18\n  by_consequence:\n    read: 18\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/cancellationreasons\n  method: get\n  operationId: getCancellationReasons\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/currencies\n  method: get\n  operationId: getCurrencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fixtures\n  method: get\n  operationId: getFixtures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fixtures/special\n  method: get\n  operationId: getSpecialFixtures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fixtures/settled\n  method: get\n  operationId: getSettledFixtures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/fixtures/special/settled\n  method: get\n  operationId: getSettledSpecialFixtures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/inrunning\n  method: get\n  operationId: getInRunning\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/leagues\n  method: get\n  operationId: getLeagues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/line\n  method: get\n  operationId: getStraightLine\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/line/parlay\n  method: post\n  operationId: getParlayLine\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/line/teaser\n  method: post\n  operationId: getTeaserLine\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/line/special\n  method: get\n  operationId: getSpecialLine\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/odds\n  method: get\n  operationId: getStraightOdds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/odds/teaser\n  method: get\n  operationId: getTeaserOdds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/odds/special\n  method: get\n  operationId: getSpecialOdds\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/periods\n  method: get\n  operationId: getPeriods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/sports\n  method: get\n  operationId: getSports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/teaser/groups\n  method: get\n  operationId: getTeaserGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pinnacle/refs/heads/main/agentic-access/pinnacle-agentic-access.yml
summary_line: 18 operations
tags:
- Gambling
- Sports Betting
---
