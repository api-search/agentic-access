---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 10
api_specs:
- filename: accelbyte-openapi.yml
  format: yaml
  label: AccelByte IAM API
  slug: accelbyte-iam-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-openapi.yml
- filename: accelbyte-openapi.yml
  format: yaml
  label: AccelByte Basic (Player Profile) API
  slug: accelbyte-basic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-openapi.yml
- filename: accelbyte-openapi.yml
  format: yaml
  label: AccelByte Cloud Save API
  slug: accelbyte-cloudsave-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-openapi.yml
- filename: accelbyte-openapi.yml
  format: yaml
  label: AccelByte Statistics & Leaderboard API
  slug: accelbyte-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-openapi.yml
- filename: accelbyte-openapi.yml
  format: yaml
  label: AccelByte Matchmaking API
  slug: accelbyte-matchmaking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-openapi.yml
- filename: accelbyte-openapi.yml
  format: yaml
  label: AccelByte Lobby & Session API
  slug: accelbyte-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-openapi.yml
- filename: accelbyte-openapi.yml
  format: yaml
  label: AccelByte Commerce (Platform) API
  slug: accelbyte-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-openapi.yml
- filename: accelbyte-openapi.yml
  format: yaml
  label: AccelByte Seasons & Battle Pass API
  slug: accelbyte-seasonpass-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-openapi.yml
- filename: accelbyte-openapi.yml
  format: yaml
  label: AccelByte Achievement API
  slug: accelbyte-achievement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-openapi.yml
- filename: accelbyte-openapi.yml
  format: yaml
  label: AccelByte Dedicated Server (Armada/DSMC) API
  slug: accelbyte-dsmc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-openapi.yml
- filename: accelbyte-openapi.yml
  format: yaml
  label: AccelByte Analytics & Telemetry API
  slug: accelbyte-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-openapi.yml
- filename: accelbyte-openapi.yml
  format: yaml
  label: AccelByte UGC API
  slug: accelbyte-ugc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/openapi/accelbyte-openapi.yml
consequence_counts:
  physical: 1
  read: 10
  safety-critical: 1
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Accelbyte Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /dsmcontroller/namespaces/{namespace}/servers/claim
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /platform/public/namespaces/{namespace}/users/{userId}/orders
operation_count: 23
overview: 'AccelByte exposes 23 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read, 11 write, 1 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AccelByte
provider_slug: accelbyte
slug: accelbyte-agentic-access
source_filename: accelbyte-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/accelbyte-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    acting: 13\n    connected: 10\n  by_consequence:\n    write: 11\n    read: 10\n    physical: 1\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /iam/v3/oauth/token\n  method: post\n  operationId: iamGetToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/v3/public/namespaces/{namespace}/users\n  method: post\n  operationId:\
  \ iamCreateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iam/v3/public/namespaces/{namespace}/users/me\n  method: get\n  operationId: iamGetMyUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /basic/v1/public/namespaces/{namespace}/users/{userId}/profiles\n  method: get\n  operationId: basicGetUserProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /basic/v1/public/namespaces/{namespace}/users/{userId}/profiles\n  method: put\n  operationId: basicUpdateUserProfile\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cloudsave/v1/namespaces/{namespace}/users/{userId}/records/{key}\n  method: get\n  operationId: cloudSaveGetPlayerRecord\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cloudsave/v1/namespaces/{namespace}/users/{userId}/records/{key}\n  method: post\n  operationId: cloudSaveCreatePlayerRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /social/v1/namespaces/{namespace}/users/{userId}/statitems\n  method: get\n  operationId:\
  \ statisticsGetUserStatItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /social/v1/namespaces/{namespace}/users/{userId}/statitems/value/bulk\n  method: put\n  operationId: statisticsBulkUpdateStatItems\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /leaderboard/v1/public/namespaces/{namespace}/leaderboards/{leaderboardCode}/all\n  method: get\n  operationId: leaderboardGetAllTimeRanking\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /match2/v1/namespaces/{namespace}/match-tickets\n  method: post\n  operationId: matchmakingCreateTicket\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /match2/v1/namespaces/{namespace}/match-tickets/{ticketId}\n  method: delete\n  operationId: matchmakingDeleteTicket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /session/v1/public/namespaces/{namespace}/gamesession\n  method: post\n  operationId: sessionCreateGameSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /session/v1/public/namespaces/{namespace}/party\n  method: post\n  operationId: sessionCreateParty\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/public/namespaces/{namespace}/items/byCriteria\n  method: get\n  operationId: platformQueryItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/public/namespaces/{namespace}/users/{userId}/entitlements\n  method: get\n  operationId: platformGetUserEntitlements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /platform/public/namespaces/{namespace}/users/{userId}/orders\n  method: post\n  operationId: platformCreateOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/public/namespaces/{namespace}/users/{userId}/wallets/{currencyCode}\n  method: get\n  operationId: platformGetUserWallet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /seasonpass/v1/public/namespaces/{namespace}/seasons/current/progression\n  method: get\n  operationId: seasonPassGetCurrentProgression\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /achievement/v1/public/namespaces/{namespace}/users/{userId}/achievements\n  method: get\n  operationId: achievementListUserAchievements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dsmcontroller/namespaces/{namespace}/servers/claim\n  method: post\n  operationId: dsmcClaimServer\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /game-telemetry/v1/protected/events\n  method: post\n  operationId: telemetrySaveEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n  \
  \  escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ugc/v1/public/namespaces/{namespace}/channels/{channelId}/contents/s3\n  method: post\n  operationId: ugcCreateContent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accelbyte/refs/heads/main/agentic-access/accelbyte-agentic-access.yml
summary_line: 23 operations · 13 acting · 1 human-in-the-loop
tags:
- Gaming
- Backend
- BaaS
- Live Services
- Player Accounts
- Commerce
---
