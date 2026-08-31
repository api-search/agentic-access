---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 1
api_specs:
- filename: flexai-audio-api-openapi.yml
  format: yaml
  label: FlexAI Audio API
  slug: flexai-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flexai/refs/heads/main/openapi/flexai-audio-api-openapi.yml
- filename: flexai-chat-api-openapi.yml
  format: yaml
  label: FlexAI Chat API
  slug: flexai-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flexai/refs/heads/main/openapi/flexai-chat-api-openapi.yml
- filename: flexai-completions-api-openapi.yml
  format: yaml
  label: FlexAI Completions API
  slug: flexai-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flexai/refs/heads/main/openapi/flexai-completions-api-openapi.yml
- filename: flexai-embeddings-api-openapi.yml
  format: yaml
  label: FlexAI Embeddings API
  slug: flexai-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flexai/refs/heads/main/openapi/flexai-embeddings-api-openapi.yml
- filename: flexai-images-api-openapi.yml
  format: yaml
  label: FlexAI Images API
  slug: flexai-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flexai/refs/heads/main/openapi/flexai-images-api-openapi.yml
- filename: flexai-models-api-openapi.yml
  format: yaml
  label: FlexAI Models API
  slug: flexai-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flexai/refs/heads/main/openapi/flexai-models-api-openapi.yml
- filename: flexai-video-api-openapi.yml
  format: yaml
  label: FlexAI Video API
  slug: flexai-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flexai/refs/heads/main/openapi/flexai-video-api-openapi.yml
consequence_counts:
  read: 1
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Flexai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'FlexAI exposes 8 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: FlexAI
provider_slug: flexai
slug: flexai-agentic-access
source_filename: flexai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/flexai-token-factory-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 7\n    connected: 1\n  by_consequence:\n    write: 7\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /chat/completions\n  method: post\n  operationId: createChatCompletion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /completions\n  method: post\n  operationId: createCompletion\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /models\n  method: get\n  operationId: listModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /embeddings\n  method: post\n  operationId: createEmbedding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /audio/transcriptions\n  method: post\n  operationId: createTranscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /audio/speech\n  method: post\n  operationId: createSpeech\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /images/generations\n  method: post\n  operationId: createImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /videos/generations\n  method: post\n  operationId: createVideo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flexai/refs/heads/main/agentic-access/flexai-agentic-access.yml
summary_line: 8 operations · 7 acting
tags:
- Company
- Ai/Ml
- Artificial Intelligence
- Machine-Learning
- Inference
- LLM
- Large Language Models
- OpenAI-Compatible
- GPU Compute
- Embeddings
- Fine-Tuning
- Agents
---
