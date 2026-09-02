---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 1
api_specs:
- filename: doubao-batch-api-openapi.yml
  format: yaml
  label: ByteDance Doubao Batch API
  slug: doubao-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doubao/refs/heads/main/openapi/doubao-batch-api-openapi.yml
- filename: doubao-chat-api-openapi.yml
  format: yaml
  label: ByteDance Doubao Chat API
  slug: doubao-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doubao/refs/heads/main/openapi/doubao-chat-api-openapi.yml
- filename: doubao-embeddings-api-openapi.yml
  format: yaml
  label: ByteDance Doubao Embeddings API
  slug: doubao-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doubao/refs/heads/main/openapi/doubao-embeddings-api-openapi.yml
- filename: doubao-images-api-openapi.yml
  format: yaml
  label: ByteDance Doubao Images API
  slug: doubao-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doubao/refs/heads/main/openapi/doubao-images-api-openapi.yml
- filename: doubao-videos-api-openapi.yml
  format: yaml
  label: ByteDance Doubao Videos API
  slug: doubao-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doubao/refs/heads/main/openapi/doubao-videos-api-openapi.yml
consequence_counts:
  read: 1
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Doubao Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'ByteDance Doubao exposes 7 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ByteDance Doubao
provider_slug: doubao
slug: doubao-agentic-access
source_filename: doubao-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/doubao-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    acting: 6\n    connected: 1\n  by_consequence:\n    write: 6\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /chat/completions\n  method: post\n  operationId: createChatCompletion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /embeddings\n  method: post\n  operationId: createEmbeddings\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /images/generations\n  method: post\n  operationId: createImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contents/generations/tasks\n  method: post\n  operationId: createVideoTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contents/generations/tasks/{task_id}\n  method: get\n\
  \  operationId: getVideoTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contents/generations/tasks/{task_id}\n  method: delete\n  operationId: deleteVideoTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /batch/chat/completions\n  method: post\n  operationId: createBatchChatCompletion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doubao/refs/heads/main/agentic-access/doubao-agentic-access.yml
summary_line: 7 operations · 6 acting
tags:
- Artificial Intelligence
- LLM
- Inference
- ByteDance
- Multi-Modal
- Volcano Engine
---
