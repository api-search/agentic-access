---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 6
api_specs:
- filename: gameye-session-openapi.yml
  format: yaml
  label: Gameye Session API
  slug: gameye-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gameye/refs/heads/main/openapi/gameye-session-openapi.yml
consequence_counts:
  read: 6
  safety-critical: 1
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Gameye Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /session/{id}
operation_count: 10
overview: 'Gameye exposes 10 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 3 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Gameye
provider_slug: gameye
slug: gameye-agentic-access
source_filename: gameye-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/gameye-session-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    acting: 4\n    connected: 6\n  by_consequence:\n    write: 3\n    read: 6\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /session\n  method: post\n  operationId: session-run\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - session:start\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /session\n  method: get\n  operationId: session-list\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - session:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /session/{id}\n  method: get\n  operationId: describe-session\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - session:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /session/{id}\n  method: delete\n  operationId: session-stop\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - session:stop\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /session/player/join\n  method: put\n  operationId: join-session\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /session/player/leave\n  method: delete\n  operationId: leave-session\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /artifacts\n  method: get\n  operationId: artifacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - artifact:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /available-location/{image}\n  method: get\n  operationId: get-available-locations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - regions:read\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /tag/{region}/{image}/{version}\n  method: get\n  operationId: tag-exists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - regions:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /logs\n  method: get\n  operationId: stream-logs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - logs:read\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gameye/refs/heads/main/agentic-access/gameye-agentic-access.yml
summary_line: 10 operations · 4 acting · 1 human-in-the-loop
tags:
- Company
- Game Server Hosting
- Game Server Orchestration
- Multiplayer
- Containers
- Infrastructure
- Gaming
- Edge Computing
- DevOps
---
