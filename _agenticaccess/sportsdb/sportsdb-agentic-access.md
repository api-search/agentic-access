---
acting_count: 0
action_class_counts:
  connected: 22
api_specs:
- filename: sportsdb-openapi.yml
  format: yaml
  label: TheSportsDB Search API
  slug: sportsdb-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsdb/refs/heads/main/openapi/sportsdb-openapi.yml
- filename: sportsdb-openapi.yml
  format: yaml
  label: TheSportsDB Lookups API
  slug: sportsdb-lookups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsdb/refs/heads/main/openapi/sportsdb-openapi.yml
- filename: sportsdb-openapi.yml
  format: yaml
  label: TheSportsDB Leagues API
  slug: sportsdb-leagues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsdb/refs/heads/main/openapi/sportsdb-openapi.yml
- filename: sportsdb-openapi.yml
  format: yaml
  label: TheSportsDB Events & Schedules API
  slug: sportsdb-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsdb/refs/heads/main/openapi/sportsdb-openapi.yml
- filename: sportsdb-openapi.yml
  format: yaml
  label: TheSportsDB Livescores API
  slug: sportsdb-livescores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsdb/refs/heads/main/openapi/sportsdb-openapi.yml
- filename: sportsdb-openapi.yml
  format: yaml
  label: TheSportsDB Players & Teams API
  slug: sportsdb-players-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsdb/refs/heads/main/openapi/sportsdb-openapi.yml
consequence_counts:
  read: 22
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sportsdb Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 22
overview: 'TheSportsDB exposes 22 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: TheSportsDB
provider_slug: sportsdb
slug: sportsdb-agentic-access
source_filename: sportsdb-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/sportsdb-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 22\n  by_consequence:\n    read: 22\n  human_in_the_loop_required: 0\noperations:\n- path: /{apiKey}/searchteams.php\n  method: get\n  operationId: searchTeams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apiKey}/searchplayers.php\n  method: get\n  operationId: searchPlayers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apiKey}/searchevents.php\n  method: get\n\
  \  operationId: searchEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apiKey}/searchvenues.php\n  method: get\n  operationId: searchVenues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apiKey}/lookupleague.php\n  method: get\n  operationId: lookupLeague\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apiKey}/lookupteam.php\n  method: get\n  operationId: lookupTeam\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apiKey}/lookupplayer.php\n  method: get\n  operationId: lookupPlayer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apiKey}/lookupevent.php\n  method: get\n  operationId: lookupEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apiKey}/lookupvenue.php\n  method: get\n  operationId: lookupVenue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apiKey}/lookuptable.php\n  method: get\n  operationId: lookupTable\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apiKey}/all_sports.php\n  method: get\n  operationId: allSports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apiKey}/all_countries.php\n\
  \  method: get\n  operationId: allCountries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apiKey}/all_leagues.php\n  method: get\n  operationId: allLeagues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apiKey}/search_all_seasons.php\n  method: get\n  operationId: searchAllSeasons\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apiKey}/search_all_teams.php\n  method: get\n  operationId: searchAllTeams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apiKey}/lookup_all_players.php\n  method: get\n  operationId: lookupAllPlayers\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apiKey}/eventsnext.php\n  method: get\n  operationId: eventsNext\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apiKey}/eventslast.php\n  method: get\n  operationId: eventsLast\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apiKey}/eventsday.php\n  method: get\n  operationId: eventsDay\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apiKey}/eventsseason.php\n  method: get\n  operationId: eventsSeason\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /{apiKey}/eventshighlights.php\n  method: get\n  operationId: eventsHighlights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /livescore/{strSport}\n  method: get\n  operationId: livescoreBySport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sportsdb/refs/heads/main/agentic-access/sportsdb-agentic-access.yml
summary_line: 22 operations
tags:
- Sports
- Sports Data
- Teams
- Players
- Events
---
