---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 3
api_specs:
- filename: vera-health-chat-api-openapi.yml
  format: yaml
  label: Vera Health Chat API
  slug: vera-health-chat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vera-health/openapi/vera-health-chat-api-openapi.yml
consequence_counts:
  physical: 1
  read: 3
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Vera Health Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/chat/v2
operation_count: 6
overview: 'Vera Health exposes 6 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read, 2 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Vera Health
provider_slug: vera-health
slug: vera-health-agentic-access
source_filename: vera-health-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/vera-health-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    acting: 3\n    connected: 3\n  by_consequence:\n    write: 2\n    physical: 1\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /api/chat/v1\n  method: post\n  operationId: chatV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chat/v2\n  method: post\n  operationId: chatV2\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chat/v2/stream/{runId}\n  method: get\n  operationId: resume-a-chat-stream\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/chat/v2/quotas\n  method: get\n  operationId: get-your-rate-limit-quotas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/chat/v3\n  method: post\n  operationId: chatV3\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chat/v3/threads/{threadId}/stream\n  method: get\n  operationId: reconnect-to-an-agentic-stream\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/vera-health/agentic-access/vera-health-agentic-access.yml
summary_line: 6 operations · 3 acting
tags:
- Health
- Artificial Intelligence
- Clinical Decision Support
- Medical Knowledge
- Healthcare
---
