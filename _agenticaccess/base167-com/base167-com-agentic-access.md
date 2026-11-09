---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 5
api_specs:
- filename: base167-com-check-api-openapi.yml
  format: yaml
  label: BASE167 Check API
  slug: base167-com-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/base167-com/openapi/base167-com-check-api-openapi.yml
- filename: base167-com-games-api-openapi.yml
  format: yaml
  label: BASE167 Games API
  slug: base167-com-games-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/base167-com/openapi/base167-com-games-api-openapi.yml
consequence_counts:
  read: 5
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Base167 Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'BASE167 exposes 9 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BASE167
provider_slug: base167-com
slug: base167-com-agentic-access
source_filename: base167-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/base167-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    acting: 4\n    connected: 5\n  by_consequence:\n    write: 4\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /api/check\n  method: post\n  operationId: checkEligibility\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/games/claim-entry\n  method: post\n  operationId: claimEntry\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/games/enroll\n  method: post\n  operationId: enroll\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/games/claim-winner\n  method: post\n  operationId: claimWinner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/games/set-name\n  method: post\n  operationId: setName\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/games/set-handle\n  method: post\n  operationId: setHandle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/games/leaderboard\n  method: get\n  operationId: getLeaderboard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/games/results\n  method: get\n  operationId: getResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/games/state\n  method: get\n  operationId: getState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/base167-com/agentic-access/base167-com-agentic-access.yml
summary_line: 9 operations · 4 acting
tags:
- Blockchain
- Gaming
- Cryptocurrency
- Tokens
- DegenGames
---
