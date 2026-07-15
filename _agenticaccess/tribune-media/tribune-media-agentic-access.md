---
acting_count: 0
action_class_counts:
  connected: 32
api_specs:
- filename: tms-onconnect-openapi.yml
  format: yaml
  label: TMS OnConnect API
  slug: tms-onconnect
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tribune-media/refs/heads/main/openapi/tms-onconnect-openapi.yml
consequence_counts:
  read: 32
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tribune Media Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 32
overview: 'Tribune Media exposes 32 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 32 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Tribune Media
provider_slug: tribune-media
slug: tribune-media-agentic-access
source_filename: tribune-media-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/tms-onconnect-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 32\n  by_action_class:\n    connected: 32\n  by_consequence:\n    read: 32\n  human_in_the_loop_required: 0\noperations:\n- path: /v1.1/lineups\n  method: get\n  operationId: getLineups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/lineups/{lineupId}\n  method: get\n  operationId: getLineupById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/lineups/{lineupId}/channels\n  method: get\n\
  \  operationId: getLineupChannels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/lineups/{lineupId}/grid\n  method: get\n  operationId: getLineupGrid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/stations/search\n  method: get\n  operationId: searchStations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/stations/{stationId}\n  method: get\n  operationId: getStationById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/stations/{stationId}/airings\n  method: get\n  operationId: getStationAirings\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/programs/search\n  method: get\n  operationId: searchPrograms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/programs/genres\n  method: get\n  operationId: getProgramGenres\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/programs/newShowAirings\n  method: get\n  operationId: getNewShowAirings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/programs/{tmsId}\n  method: get\n  operationId: getProgramById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1.1/programs/{tmsId}/airings\n  method: get\n  operationId: getProgramAirings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/series/{seriesId}\n  method: get\n  operationId: getSeriesById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/series/{seriesId}/airings\n  method: get\n  operationId: getSeriesAirings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/series/{seriesId}/episodes\n  method: get\n  operationId: getSeriesEpisodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/movies/airings\n  method: get\n  operationId: getMovieAirings\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/movies/showings\n  method: get\n  operationId: getMovieShowings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/theatres\n  method: get\n  operationId: getTheatres\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/theatres/{theatreId}/showings\n  method: get\n  operationId: getTheatreShowings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/movies/{movieId}/showings\n  method: get\n  operationId: getMovieShowtimes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/sports/{sportsId}\n  method: get\n  operationId: getSportById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/sports/{sportsId}/events/airings\n  method: get\n  operationId: getSportEventAirings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/sports/{sportsId}/non-events/airings\n  method: get\n  operationId: getSportNonEventAirings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/sports/organizations/{organizationId}/airings\n  method: get\n  operationId: getOrganizationAirings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1.1/sports/teams/{teamBrandId}/airings\n  method: get\n  operationId: getTeamAirings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/celebs/{personId}\n  method: get\n  operationId: getCelebrityById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/celebs/{personId}/airings\n  method: get\n  operationId: getCelebrityAirings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/celebs/talkShowAirings\n  method: get\n  operationId: getTalkShowCelebrityAirings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/series/{seriesId}\n\
  \  method: get\n  operationId: getOnlineVideoSeries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/episodes/{rootId_tmsId}\n  method: get\n  operationId: getOnlineVideoEpisode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/movies/{rootId_tmsId}\n  method: get\n  operationId: getOnlineVideoMovie\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /social/{rootId_seriesId}\n  method: get\n  operationId: getSocialData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tribune-media/refs/heads/main/agentic-access/tribune-media-agentic-access.yml
summary_line: 32 operations
tags:
- Media
- Entertainment
- Broadcasting
- Television
- Movies
- Sports
- Celebrity
- Fortune 1000
---
