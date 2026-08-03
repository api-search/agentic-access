---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 3
api_specs:
- filename: taalas-inference-api-openapi.yml
  format: yaml
  label: Taalas API
  slug: taalas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taalas/refs/heads/main/openapi/taalas-inference-api-openapi.yml
- filename: taalas-inference-v1-api-openapi.yml
  format: yaml
  label: Taalas API v1 (OpenAI-compatible)
  slug: taalas-api-v1-openai-compatible
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taalas/refs/heads/main/openapi/taalas-inference-v1-api-openapi.yml
consequence_counts:
  read: 3
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Taalas Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Taalas exposes 6 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Taalas
provider_slug: taalas
slug: taalas-agentic-access
source_filename: taalas-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: generated\nsource: openapi/taalas-inference-api-openapi.yml, openapi/taalas-inference-v1-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 3\n    acting: 3\n  by_consequence:\n    read: 3\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /health\n  method: get\n  operationId: health_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /models\n  method: get\n  operationId: models_models_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /generate\n  method: post\n  operationId: generate_generate_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /models\n  method: get\n  operationId: models_models_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /completions\n  method: post\n  operationId: completions_completions_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chat/completions\n  method: post\n  operationId: chat_completions_chat_completions_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taalas/refs/heads/main/agentic-access/taalas-agentic-access.yml
summary_line: 6 operations · 3 acting
tags:
- Company
- artificial-intelligence
- ai-inference
- semiconductors
- ai-accelerator
- large-language-models
- llama
- inference-api
- openai-compatible
- hardware
- deep-tech
---
