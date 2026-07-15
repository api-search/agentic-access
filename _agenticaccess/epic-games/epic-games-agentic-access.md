---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 12
consequence_counts:
  physical: 3
  read: 12
  safety-critical: 1
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Epic Games Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /auth/v1/oauth/revoke
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /player-data-storage/v1/{deploymentId}/file/{filename}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /player-data-storage/v1/{deploymentId}/file/{filename}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /stats/v1/{deploymentId}/users/{productUserId}/stats
operation_count: 17
overview: 'Epic Games exposes 17 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read, 1 write, 3 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Epic Games
provider_slug: epic-games
slug: epic-games-agentic-access
source_filename: epic-games-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/epic-games-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    acting: 5\n    connected: 12\n  by_consequence:\n    write: 1\n    read: 12\n    safety-critical: 1\n    physical: 3\n  human_in_the_loop_required: 1\noperations:\n- path: /auth/v1/oauth/token\n  method: post\n  operationId: getOAuthToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/v1/oauth/verify\n  method: get\n  operationId: verifyOAuthToken\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/v1/oauth/revoke\n  method: post\n  operationId: revokeOAuthToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /auth/v1/accounts/{accountId}\n  method: get\n  operationId: getEpicAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connect/v1/{deploymentId}/users\n  method: get\n  operationId: queryConnectUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /player-data-storage/v1/{deploymentId}/file/{filename}\n  method: get\n  operationId: getPlayerDataFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /player-data-storage/v1/{deploymentId}/file/{filename}\n  method: put\n  operationId: putPlayerDataFile\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /player-data-storage/v1/{deploymentId}/file/{filename}\n  method: delete\n  operationId: deletePlayerDataFile\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n\
  \      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /title-storage/v1/{deploymentId}/file/{filename}\n  method: get\n  operationId: getTitleStorageFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats/v1/{deploymentId}/users/{productUserId}/stats\n  method: get\n  operationId: listUserStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats/v1/{deploymentId}/users/{productUserId}/stats\n  method: post\n  operationId: ingestUserStats\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n \
  \     human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /achievements/v2/{deploymentId}/definitions\n  method: get\n  operationId: listAchievementDefinitions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /achievements/v2/{deploymentId}/users/{productUserId}/achievements\n  method: get\n  operationId: listPlayerAchievements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leaderboards/v1/{deploymentId}/definitions\n  method: get\n  operationId: listLeaderboardDefinitions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leaderboards/v1/{deploymentId}/leaderboard/{leaderboardId}/ranks\n  method: get\n  operationId:\
  \ getLeaderboardRanks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sanctions/v1/{deploymentId}/sanctions\n  method: get\n  operationId: listSanctions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ecom/v1/identities/{accountId}/entitlements\n  method: get\n  operationId: listEntitlements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/epic-games/refs/heads/main/agentic-access/epic-games-agentic-access.yml
summary_line: 17 operations · 5 acting · 1 human-in-the-loop
tags:
- Achievements
- Anti-Cheat
- Cross-Platform
- EOS
- Epic Online Services
- Game Backend
- Game Development
- Games
- Identity
- Lobby
- Matchmaking
- Multiplayer
- Sessions
- Unreal Engine
- Voice
---
