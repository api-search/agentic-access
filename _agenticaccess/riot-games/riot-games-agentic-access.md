---
acting_count: 0
action_class_counts:
  connected: 17
api_specs:
- filename: riot-games-league-of-legends-openapi.yml
  format: yaml
  label: League of Legends API
  slug: league-of-legends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riot-games/refs/heads/main/openapi/riot-games-league-of-legends-openapi.yml
consequence_counts:
  read: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Riot Games Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'Riot Games exposes 17 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Riot Games
provider_slug: riot-games
slug: riot-games-agentic-access
source_filename: riot-games-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/riot-games-league-of-legends-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    connected: 17\n  by_consequence:\n    read: 17\n  human_in_the_loop_required: 0\noperations:\n- path: /lol/summoner/v4/summoners/by-name/{summonerName}\n  method: get\n  operationId: getSummonerByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lol/summoner/v4/summoners/by-puuid/{encryptedPUUID}\n  method: get\n  operationId: getSummonerByPUUID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n- path: /lol/summoner/v4/summoners/{encryptedSummonerId}\n  method: get\n  operationId: getSummonerById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lol/champion-mastery/v4/champion-masteries/by-puuid/{encryptedPUUID}\n  method: get\n  operationId: getChampionMasteryByPUUID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lol/champion-mastery/v4/champion-masteries/by-puuid/{encryptedPUUID}/by-champion/{championId}\n  method: get\n  operationId: getChampionMasteryByPUUIDAndChampion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lol/league/v4/entries/by-summoner/{encryptedSummonerId}\n  method: get\n  operationId: getLeagueEntriesBySummoner\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lol/league/v4/entries/{queue}/{tier}/{division}\n  method: get\n  operationId: getLeagueEntries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lol/league/v4/challengerleagues/by-queue/{queue}\n  method: get\n  operationId: getChallengerLeague\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lol/match/v5/matches/by-puuid/{puuid}/ids\n  method: get\n  operationId: getMatchIdsByPUUID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lol/match/v5/matches/{matchId}\n  method: get\n  operationId: getMatch\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lol/match/v5/matches/{matchId}/timeline\n  method: get\n  operationId: getMatchTimeline\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lol/spectator/v5/active-games/by-summoner/{encryptedSummonerId}\n  method: get\n  operationId: getLiveGame\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lol/spectator/v5/featured-games\n  method: get\n  operationId: getFeaturedGames\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lol/clash/v1/players/by-puuid/{puuid}\n  method: get\n  operationId: getClashPlayersByPUUID\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lol/champion/v3/champion-rotations\n  method: get\n  operationId: getChampionRotations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lol/status/v4/platform-data\n  method: get\n  operationId: getPlatformStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /riot/account/v1/accounts/by-riot-id/{gameName}/{tagLine}\n  method: get\n  operationId: getAccountByRiotId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/riot-games/refs/heads/main/agentic-access/riot-games-agentic-access.yml
summary_line: 17 operations
tags:
- Esports
- Gaming
- League of Legends
- Legends of Runeterra
- Teamfight Tactics
- VALORANT
---
