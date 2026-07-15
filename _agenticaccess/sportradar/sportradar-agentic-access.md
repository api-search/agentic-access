---
acting_count: 0
action_class_counts:
  connected: 25
api_specs:
- filename: sportradar-sports-data-openapi.yml
  format: yaml
  label: Sportradar Sports Data API
  slug: sports-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportradar/refs/heads/main/openapi/sportradar-sports-data-openapi.yml
- filename: sportradar-push-feeds-openapi.yml
  format: yaml
  label: Sportradar Push Feeds API
  slug: push-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportradar/refs/heads/main/openapi/sportradar-push-feeds-openapi.yml
consequence_counts:
  read: 25
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sportradar Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 25
overview: 'Sportradar exposes 25 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 25 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Sportradar
provider_slug: sportradar
slug: sportradar-agentic-access
source_filename: sportradar-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/sportradar-push-feeds-openapi.yml, openapi/sportradar-sports-data-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 25\n  by_action_class:\n    connected: 25\n  by_consequence:\n    read: 25\n  human_in_the_loop_required: 0\noperations:\n- path: /nfl/official/{access_level}/stream/{language_code}/events/subscribe\n  method: get\n  operationId: subscribeNflPushEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nfl/official/{access_level}/stream/{language_code}/statistics/subscribe\n  method: get\n  operationId: subscribeNflPushStatistics\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nfl/official/{access_level}/stream/{language_code}/pulse/subscribe\n  method: get\n  operationId: subscribeNflPushPulse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nfl/official/{access_level}/stream/{language_code}/draft-picks/subscribe\n  method: get\n  operationId: subscribeNflPushDraftPicks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nfl/official/{access_level}/stream/{language_code}/draft-trades/subscribe\n  method: get\n  operationId: subscribeNflPushDraftTrades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nba/{access_level}/stream/{language_code}/events/subscribe\n\
  \  method: get\n  operationId: subscribeNbaPushEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nba/{access_level}/stream/{language_code}/statistics/subscribe\n  method: get\n  operationId: subscribeNbaPushStatistics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nba/{access_level}/stream/{language_code}/clock/subscribe\n  method: get\n  operationId: subscribeNbaPushClock\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nba/{access_level}/stream/{language_code}/draft_picks/subscribe\n  method: get\n  operationId: subscribeNbaPushDraftPicks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /nba/{access_level}/stream/{language_code}/draft_trades/subscribe\n  method: get\n  operationId: subscribeNbaPushDraftTrades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nhl/{access_level}/stream/{language_code}/events/subscribe\n  method: get\n  operationId: subscribeNhlPushEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nhl/{access_level}/stream/{language_code}/statistics/subscribe\n  method: get\n  operationId: subscribeNhlPushStatistics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nhl/{access_level}/stream/{language_code}/push-clock/subscribe\n  method: get\n  operationId: subscribeNhlPushClock\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wnba/{access_level}/stream/events/subscribe\n  method: get\n  operationId: subscribeWnbaPushEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wnba/{access_level}/stream/statistics/subscribe\n  method: get\n  operationId: subscribeWnbaPushStatistics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wnba/{access_level}/stream/clock/subscribe\n  method: get\n  operationId: subscribeWnbaPushClock\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /soccer/{access_level}/{version}/stream/events/subscribe\n  method: get\n  operationId: subscribeSoccerPushEvents\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /soccer/{access_level}/{version}/stream/statistics/subscribe\n  method: get\n  operationId: subscribeSoccerPushStatistics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nba/trial/v8/en/games/{game_id}/summary.json\n  method: get\n  operationId: getNbaGameSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nba/trial/v8/en/games/{date}/schedule.json\n  method: get\n  operationId: getNbaDailySchedule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nba/trial/v8/en/seasons/{season_year}/REG/standings.json\n  method:\
  \ get\n  operationId: getNbaStandings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /soccer-t3/trial/v4/en/competitions/{competition_id}/info.json\n  method: get\n  operationId: getSoccerCompetitionInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /soccer-t3/trial/v4/en/sport_events/{sport_event_id}/summary.json\n  method: get\n  operationId: getSoccerMatchSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nfl/trial/v7/en/games/{game_id}/summary.json\n  method: get\n  operationId: getNflGameSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nba/trial/v8/en/players/{player_id}/profile.json\n\
  \  method: get\n  operationId: getNbaPlayerProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sportradar/refs/heads/main/agentic-access/sportradar-agentic-access.yml
summary_line: 25 operations
tags:
- Data
- Esports
- Fantasy Sports
- HTTP Chunked
- Media
- Push
- Real-Time
- Sports
- Sports Data
- Statistics
- Streaming
---
