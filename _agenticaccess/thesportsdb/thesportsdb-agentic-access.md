---
acting_count: 0
action_class_counts:
  connected: 17
api_specs:
- filename: thesportsdb-openapi.yml
  format: yaml
  label: TheSportsDB API
  slug: thesportsdb
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thesportsdb/refs/heads/main/openapi/thesportsdb-openapi.yml
consequence_counts:
  read: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Thesportsdb Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'TheSportsDB exposes 17 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: TheSportsDB
provider_slug: thesportsdb
slug: thesportsdb-agentic-access
source_filename: thesportsdb-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/thesportsdb-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    connected: 17\n  by_consequence:\n    read: 17\n  human_in_the_loop_required: 0\noperations:\n- path: /searchteams.php\n  method: get\n  operationId: searchTeams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /searchplayers.php\n  method: get\n  operationId: searchPlayers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /searchevents.php\n  method: get\n  operationId: searchEvents\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /searchvenues.php\n  method: get\n  operationId: searchVenues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /all_leagues.php\n  method: get\n  operationId: listAllLeagues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /all_sports.php\n  method: get\n  operationId: listAllSports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search_all_teams.php\n  method: get\n  operationId: listAllTeams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /search_all_leagues.php\n  method: get\n  operationId: searchAllLeagues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lookupleague.php\n  method: get\n  operationId: lookupLeague\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lookupteam.php\n  method: get\n  operationId: lookupTeam\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lookupplayer.php\n  method: get\n  operationId: lookupPlayer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lookupevent.php\n  method: get\n  operationId: lookupEvent\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /eventsnext.php\n  method: get\n  operationId: getNextTeamEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /eventslast.php\n  method: get\n  operationId: getLastTeamEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /eventsseason.php\n  method: get\n  operationId: getSeasonEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lookuptable.php\n  method: get\n  operationId: lookupTable\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search_all_seasons.php\n\
  \  method: get\n  operationId: listAllSeasons\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thesportsdb/refs/heads/main/agentic-access/thesportsdb-agentic-access.yml
summary_line: 17 operations
tags:
- Sports
- Database
- Free
- Open Data
- Teams
- Players
- Events
---
