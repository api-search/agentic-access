---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 7
api_specs:
- filename: end-game-threads-api-openapi.yml
  format: yaml
  label: Endgame Threads API
  slug: end-game-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/end-game/refs/heads/main/openapi/end-game-threads-api-openapi.yml
- filename: end-game-internal-api-openapi.yml
  format: yaml
  label: Endgame Internal API
  slug: end-game-internal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/end-game/refs/heads/main/openapi/end-game-internal-api-openapi.yml
- filename: end-game-protected-static-api-openapi.yml
  format: yaml
  label: Endgame Protected Static API
  slug: end-game-protected-static-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/end-game/refs/heads/main/openapi/end-game-protected-static-api-openapi.yml
consequence_counts:
  read: 7
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: End Game Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'Endgame exposes 17 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 10 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Endgame
provider_slug: end-game
slug: end-game-agentic-access
source_filename: end-game-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: generated\nsource: openapi/end-game-internal-api-openapi.yml, openapi/end-game-protected-static-api-openapi.yml,\n  openapi/end-game-threads-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    connected: 7\n    acting: 10\n  by_consequence:\n    read: 7\n    write: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /internal/feedback\n  method: get\n  operationId: internal.feedback.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /internal/feedback/promote\n  method: post\n  operationId: internal.feedback.promote\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /internal/feedback/dismiss\n  method: post\n  operationId: internal.feedback.dismiss\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /protected-static/objects\n  method: get\n  operationId: protectedStatic.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /protected-static/objects\n  method: put\n  operationId: protectedStatic.put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /protected-static/objects\n  method: delete\n  operationId: protectedStatic.delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /protected-static/objects/content\n  method: get\n  operationId: protectedStatic.getContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/threads\n  method: post\n  operationId: createThread\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/threads\n  method: get\n  operationId: listThreads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/threads/{id}\n  method: get\n  operationId: getThread\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/threads/{id}\n  method: patch\n  operationId: updateThread\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/threads/{id}\n  method: delete\n  operationId: deleteThread\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /threads\n  method: post\n  operationId: threads.create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /threads\n  method: get\n  operationId: threads.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /threads/{id}\n  method: get\n  operationId: threads.get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /threads/{id}\n  method: patch\n  operationId: threads.update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /threads/{id}\n  method: delete\n  operationId: threads.delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/end-game/refs/heads/main/agentic-access/end-game-agentic-access.yml
summary_line: 17 operations · 10 acting
tags:
- Company
- Sales
- Revenue Intelligence
- Go-To-Market
- Artificial Intelligence
- Agents
- MCP
- Knowledge Graph
- CRM
- Conversation Intelligence
---
