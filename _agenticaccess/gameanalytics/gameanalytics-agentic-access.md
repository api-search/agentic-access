---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 5
api_specs:
- filename: gameanalytics-openapi.yml
  format: yaml
  label: GameAnalytics Collection API
  slug: gameanalytics-collection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gameanalytics/refs/heads/main/openapi/gameanalytics-openapi.yml
- filename: gameanalytics-openapi.yml
  format: yaml
  label: GameAnalytics Metrics API
  slug: gameanalytics-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gameanalytics/refs/heads/main/openapi/gameanalytics-openapi.yml
- filename: gameanalytics-openapi.yml
  format: yaml
  label: GameAnalytics Organization API
  slug: gameanalytics-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gameanalytics/refs/heads/main/openapi/gameanalytics-openapi.yml
consequence_counts:
  read: 5
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Gameanalytics Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'GameAnalytics exposes 12 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: GameAnalytics
provider_slug: gameanalytics
slug: gameanalytics-agentic-access
source_filename: gameanalytics-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/gameanalytics-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    acting: 7\n    connected: 5\n  by_consequence:\n    write: 7\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/{game_key}/init\n  method: post\n  operationId: collectionInit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/{game_key}/events\n  method: post\n  operationId: collectionEvents\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /metrics/v1/metrics/{metric}\n  method: post\n  operationId: queryMetric\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/games\n  method: get\n  operationId: listGames\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/games\n  method: post\n  operationId: createGame\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/games/{game_id}\n  method: get\n  operationId: getGame\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/studios\n  method: get\n  operationId: listStudios\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/studios\n  method: post\n  operationId: createStudio\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/studios/{studio_id}\n  method: get\n  operationId: getStudio\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/users\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/users/invite\n  method: post\n  operationId: inviteUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/users/{user_id}/replace_acl\n  method: post\n  operationId: replaceUserAcl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gameanalytics/refs/heads/main/agentic-access/gameanalytics-agentic-access.yml
summary_line: 12 operations · 7 acting
tags:
- Analytics
- Games
- Gaming
- Player Behavior
- Retention
- Monetization
- Ad Analytics
- Telemetry
---
