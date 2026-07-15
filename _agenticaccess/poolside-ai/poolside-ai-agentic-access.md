---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 1
api_specs:
- filename: poolside-ai-openapi.json
  format: json
  label: Poolside Chat Completions API
  slug: poolside-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/poolside-ai/refs/heads/main/openapi/poolside-ai-openapi.json
- filename: poolside-ai-openapi.json
  format: json
  label: Poolside Completions API (Legacy)
  slug: poolside-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/poolside-ai/refs/heads/main/openapi/poolside-ai-openapi.json
- filename: poolside-ai-openapi.json
  format: json
  label: Poolside Models API
  slug: poolside-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/poolside-ai/refs/heads/main/openapi/poolside-ai-openapi.json
consequence_counts:
  read: 1
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Poolside Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 3
overview: 'Poolside exposes 3 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Poolside
provider_slug: poolside-ai
slug: poolside-ai-agentic-access
source_filename: poolside-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/poolside-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 3\n  by_action_class:\n    acting: 2\n    connected: 1\n  by_consequence:\n    write: 2\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /openai/v1/chat/completions\n  method: post\n  operationId: create-chat-completion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openai/v1/completions\n  method: post\n  operationId: create-completion\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openai/v1/models\n  method: get\n  operationId: list-models\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/poolside-ai/refs/heads/main/agentic-access/poolside-ai-agentic-access.yml
summary_line: 3 operations · 2 acting
tags:
- AI
- LLM
- Foundation Models
- Agentic Coding
- Software Engineering
- Enterprise
- On-Prem
- Open Weights
---
