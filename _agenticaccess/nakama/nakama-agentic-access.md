---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 9
api_specs:
- filename: nakama-asyncapi.yml
  format: yaml
  label: Nakama Realtime Socket API
  slug: nakama-realtime-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/nakama/refs/heads/main/asyncapi/nakama-asyncapi.yml
- filename: nakama-account-api-openapi.yml
  format: yaml
  label: Nakama Account API
  slug: nakama-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nakama/refs/heads/main/openapi/nakama-account-api-openapi.yml
- filename: nakama-authentication-api-openapi.yml
  format: yaml
  label: Nakama Authentication API
  slug: nakama-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nakama/refs/heads/main/openapi/nakama-authentication-api-openapi.yml
- filename: nakama-friends-api-openapi.yml
  format: yaml
  label: Nakama Friends API
  slug: nakama-friends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nakama/refs/heads/main/openapi/nakama-friends-api-openapi.yml
- filename: nakama-groups-api-openapi.yml
  format: yaml
  label: Nakama Groups API
  slug: nakama-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nakama/refs/heads/main/openapi/nakama-groups-api-openapi.yml
- filename: nakama-leaderboards-api-openapi.yml
  format: yaml
  label: Nakama Leaderboards API
  slug: nakama-leaderboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nakama/refs/heads/main/openapi/nakama-leaderboards-api-openapi.yml
- filename: nakama-notifications-api-openapi.yml
  format: yaml
  label: Nakama Notifications API
  slug: nakama-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nakama/refs/heads/main/openapi/nakama-notifications-api-openapi.yml
- filename: nakama-rpc-api-openapi.yml
  format: yaml
  label: Nakama RPC API
  slug: nakama-rpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nakama/refs/heads/main/openapi/nakama-rpc-api-openapi.yml
- filename: nakama-storage-api-openapi.yml
  format: yaml
  label: Nakama Storage API
  slug: nakama-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nakama/refs/heads/main/openapi/nakama-storage-api-openapi.yml
- filename: nakama-tournaments-api-openapi.yml
  format: yaml
  label: Nakama Tournaments API
  slug: nakama-tournaments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nakama/refs/heads/main/openapi/nakama-tournaments-api-openapi.yml
consequence_counts:
  read: 9
  write: 18
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Nakama Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 27
overview: 'Nakama exposes 27 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 18 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Nakama
provider_slug: nakama
slug: nakama-agentic-access
source_filename: nakama-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/nakama-account-api-openapi.yml, openapi/nakama-authentication-api-openapi.yml,\n  openapi/nakama-friends-api-openapi.yml, openapi/nakama-groups-api-openapi.yml, openapi/nakama-leaderboards-api-openapi.yml,\n  openapi/nakama-notifications-api-openapi.yml, openapi/nakama-rpc-api-openapi.yml, openapi/nakama-storage-api-openapi.yml,\n  openapi/nakama-tournaments-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 27\n  by_action_class:\n    connected: 9\n    acting: 18\n  by_consequence:\n    read: 9\n    write: 18\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/account\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n \
  \   consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/account\n  method: put\n  operationId: updateAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account\n  method: delete\n  operationId: deleteAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/link/device\n  method: post\n  operationId: linkDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/unlink/device\n  method: post\n  operationId: unlinkDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/user\n  method: get\n  operationId: getUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/account/authenticate/device\n  method: post\n  operationId: authenticateDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/authenticate/email\n  method: post\n  operationId: authenticateEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/authenticate/custom\n  method: post\n  operationId: authenticateCustom\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/session/refresh\n  method: post\n  operationId: sessionRefresh\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/friend\n  method: get\n  operationId: listFriends\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/friend\n  method: post\n  operationId: addFriends\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/friend\n  method: delete\n  operationId: deleteFriends\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v2/group\n  method: post\n  operationId: createGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/group/{group_id}/join\n  method: post\n  operationId: joinGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/leaderboard/{leaderboard_id}\n  method: get\n  operationId: listLeaderboardRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/leaderboard/{leaderboard_id}\n\
  \  method: post\n  operationId: writeLeaderboardRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/notification\n  method: get\n  operationId: listNotifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/notification\n  method: delete\n  operationId: deleteNotifications\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/rpc/{id}\n  method: post\n  operationId: rpcFunc\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/rpc/{id}\n  method: get\n  operationId: rpcFunc2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/storage\n  method: put\n  operationId: writeStorageObjects\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/storage\n  method: post\n  operationId: readStorageObjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n \
  \   audit: none\n- path: /v2/storage/{collection}\n  method: get\n  operationId: listStorageObjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/storage/delete\n  method: put\n  operationId: deleteStorageObjects\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tournament\n  method: get\n  operationId: listTournaments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/tournament/{tournament_id}/join\n  method: post\n  operationId: joinTournament\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nakama/refs/heads/main/agentic-access/nakama-agentic-access.yml
summary_line: 27 operations · 18 acting
tags:
- Gaming
- Game Backend
- Backend
- Real-Time
- Multiplayer
- Matchmaking
- Leaderboards
- Social
- Open Source
---
