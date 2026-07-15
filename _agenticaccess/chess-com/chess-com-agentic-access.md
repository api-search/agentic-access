---
acting_count: 0
action_class_counts:
  connected: 29
api_specs:
- filename: chess-com-published-data-api-openapi.yml
  format: yaml
  label: Chess.com Published Data API
  slug: chess-com-published-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chess-com/refs/heads/main/openapi/chess-com-published-data-api-openapi.yml
consequence_counts:
  read: 29
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Chess Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 29
overview: 'Chess.com exposes 29 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 29 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Chess.com
provider_slug: chess-com
slug: chess-com-agentic-access
source_filename: chess-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/chess-com-published-data-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 29\n  by_action_class:\n    connected: 29\n  by_consequence:\n    read: 29\n  human_in_the_loop_required: 0\noperations:\n- path: /player/{username}\n  method: get\n  operationId: getPlayerProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /player/{username}/stats\n  method: get\n  operationId: getPlayerStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /player/{username}/is-online\n\
  \  method: get\n  operationId: getPlayerOnline\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /player/{username}/games\n  method: get\n  operationId: getPlayerCurrentGames\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /player/{username}/games/to-move\n  method: get\n  operationId: getPlayerGamesToMove\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /player/{username}/games/archives\n  method: get\n  operationId: listPlayerArchives\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /player/{username}/games/{year}/{month}\n  method: get\n  operationId: getPlayerMonthlyArchive\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /player/{username}/games/{year}/{month}/pgn\n  method: get\n  operationId: getPlayerMonthlyArchivePgn\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /player/{username}/clubs\n  method: get\n  operationId: getPlayerClubs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /player/{username}/matches\n  method: get\n  operationId: getPlayerMatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /player/{username}/tournaments\n  method: get\n  operationId: getPlayerTournaments\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /titled/{title-abbrev}\n  method: get\n  operationId: listTitledPlayers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /club/{url-ID}\n  method: get\n  operationId: getClub\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /club/{url-ID}/members\n  method: get\n  operationId: getClubMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /club/{url-ID}/matches\n  method: get\n  operationId: getClubMatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tournament/{url-ID}\n\
  \  method: get\n  operationId: getTournament\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tournament/{url-ID}/{round}\n  method: get\n  operationId: getTournamentRound\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tournament/{url-ID}/{round}/{group}\n  method: get\n  operationId: getTournamentRoundGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /match/{ID}\n  method: get\n  operationId: getDailyMatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /match/{ID}/{board}\n  method: get\n  operationId: getDailyMatchBoard\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /match/live/{ID}\n  method: get\n  operationId: getLiveMatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /match/live/{ID}/{board}\n  method: get\n  operationId: getLiveMatchBoard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /country/{iso}\n  method: get\n  operationId: getCountry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /country/{iso}/players\n  method: get\n  operationId: listCountryPlayers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /country/{iso}/clubs\n  method: get\n  operationId: listCountryClubs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /puzzle\n  method: get\n  operationId: getDailyPuzzle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /puzzle/random\n  method: get\n  operationId: getRandomPuzzle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /streamers\n  method: get\n  operationId: listStreamers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leaderboards\n  method: get\n  operationId: getLeaderboards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n \
  \   subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chess-com/refs/heads/main/agentic-access/chess-com-agentic-access.yml
summary_line: 29 operations
tags:
- Chess
- Gaming
- Online Games
- Sports
- Community
- Education
---
