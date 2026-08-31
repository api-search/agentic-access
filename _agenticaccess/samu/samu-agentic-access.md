---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 8
api_specs:
- filename: samu-meetings-api-openapi.yml
  format: yaml
  label: Samu Meetings API
  slug: samu-meetings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/samu/refs/heads/main/openapi/samu-meetings-api-openapi.yml
- filename: samu-threads-api-openapi.yml
  format: yaml
  label: Samu Threads API
  slug: samu-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/samu/refs/heads/main/openapi/samu-threads-api-openapi.yml
- filename: samu-usuarios-api-openapi.yml
  format: yaml
  label: Samu Usuarios API
  slug: samu-usuarios-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/samu/refs/heads/main/openapi/samu-usuarios-api-openapi.yml
consequence_counts:
  read: 8
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Samu Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'Samu exposes 10 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Samu
provider_slug: samu
slug: samu-agentic-access
source_filename: samu-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: generated\nsource: openapi/samu-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 8\n    acting: 2\n  by_consequence:\n    read: 8\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/users\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/meeting\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n \
  \   audit: required\n- path: /api/meeting/{id}\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/meeting/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/meeting/{id}/transcription\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/chat/threads\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/chat/threads/{threadId}\n  method: get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/chat/threads/{threadId}/messages\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/chat/threads/{threadId}/interactions\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/meetings\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/samu/refs/heads/main/agentic-access/samu-agentic-access.yml
summary_line: 10 operations · 2 acting
tags:
- Company
- Artificial Intelligence
- Sales
- Sales Intelligence
- Conversation Intelligence
- CRM
- Call Recording
- Analytics
- Latin America
- Transcription
- WhatsApp
- MCP
- Agent Native
---
