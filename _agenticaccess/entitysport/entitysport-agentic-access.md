---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 14
api_specs:
- filename: entitysport-openapi.yml
  format: yaml
  label: Entity Sport Competitions API
  slug: competitions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entitysport/refs/heads/main/openapi/entitysport-openapi.yml
- filename: entitysport-openapi.yml
  format: yaml
  label: Entity Sport Matches & Live Scoring API
  slug: matches-live-scoring
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entitysport/refs/heads/main/openapi/entitysport-openapi.yml
- filename: entitysport-openapi.yml
  format: yaml
  label: Entity Sport Scorecards API
  slug: scorecards
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entitysport/refs/heads/main/openapi/entitysport-openapi.yml
- filename: entitysport-openapi.yml
  format: yaml
  label: Entity Sport Fantasy Points API
  slug: fantasy-points
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entitysport/refs/heads/main/openapi/entitysport-openapi.yml
- filename: entitysport-openapi.yml
  format: yaml
  label: Entity Sport Players & Teams API
  slug: players-teams
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entitysport/refs/heads/main/openapi/entitysport-openapi.yml
- filename: entitysport-openapi.yml
  format: yaml
  label: Entity Sport Odds API
  slug: odds
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entitysport/refs/heads/main/openapi/entitysport-openapi.yml
consequence_counts:
  read: 14
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Entitysport Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'Entity Sport exposes 15 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Entity Sport
provider_slug: entitysport
slug: entitysport-agentic-access
source_filename: entitysport-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/entitysport-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    acting: 1\n    connected: 14\n  by_consequence:\n    write: 1\n    read: 14\n  human_in_the_loop_required: 0\noperations:\n- path: /auth\n  method: post\n  operationId: createAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /seasons\n  method: get\n  operationId: listSeasons\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /competitions\n  method: get\n  operationId: listCompetitions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /competitions/{cid}\n  method: get\n  operationId: getCompetition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /competitions/{cid}/matches\n  method: get\n  operationId: listCompetitionMatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /competitions/{cid}/standings\n  method: get\n  operationId: getCompetitionStandings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /matches\n  method: get\n  operationId: listMatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /matches/{mid}/info\n  method: get\n  operationId: getMatchInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /matches/{mid}/live\n  method: get\n  operationId: getMatchLive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /matches/{mid}/scorecard\n  method: get\n  operationId: getMatchScorecard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /matches/{mid}/squads\n  method: get\n  operationId: getMatchSquads\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /matches/{mid}/point\n  method: get\n  operationId: getMatchFantasyPoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /matches/{mid}/odds\n  method: get\n  operationId: getMatchOdds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /players/{pid}\n  method: get\n  operationId: getPlayer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /teams/{tid}\n  method: get\n  operationId: getTeam\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/entitysport/refs/heads/main/agentic-access/entitysport-agentic-access.yml
summary_line: 15 operations · 1 acting
tags:
- Sports Data
- Cricket
- Live Scores
- Fantasy
- Odds
---
