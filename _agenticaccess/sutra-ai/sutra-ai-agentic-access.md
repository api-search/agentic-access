---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 1
api_specs:
- filename: sutra-ai-openapi.yml
  format: yaml
  label: SUTRA Chat Completions (Multilingual) API
  slug: chat-completions-multilingual-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sutra-ai/refs/heads/main/openapi/sutra-ai-openapi.yml
- filename: sutra-ai-openapi.yml
  format: yaml
  label: SUTRA Reasoning API
  slug: reasoning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sutra-ai/refs/heads/main/openapi/sutra-ai-openapi.yml
- filename: sutra-ai-openapi.yml
  format: yaml
  label: SUTRA Models API
  slug: models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sutra-ai/refs/heads/main/openapi/sutra-ai-openapi.yml
consequence_counts:
  read: 1
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sutra Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 2
overview: 'SUTRA (Two AI) exposes 2 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SUTRA (Two AI)
provider_slug: sutra-ai
slug: sutra-ai-agentic-access
source_filename: sutra-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/sutra-ai-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 2\n  by_action_class:\n    acting: 1\n    connected: 1\n  by_consequence:\n    write: 1\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /chat/completions\n  method: post\n  operationId: createChatCompletion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /models\n  method: get\n  operationId: listModels\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sutra-ai/refs/heads/main/agentic-access/sutra-ai-agentic-access.yml
summary_line: 2 operations · 1 acting
tags:
- AI
- LLM
- Multilingual
- Inference
- Reasoning
---
