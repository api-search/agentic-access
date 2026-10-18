---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 7
api_specs:
- filename: llmgateway-io-audio-api-openapi.yml
  format: yaml
  label: LLM Gateway Audio API
  slug: llmgateway-io-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llmgateway-io/refs/heads/main/openapi/llmgateway-io-audio-api-openapi.yml
- filename: llmgateway-io-decisions-api-openapi.yml
  format: yaml
  label: LLM Gateway Decisions API
  slug: llmgateway-io-decisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llmgateway-io/refs/heads/main/openapi/llmgateway-io-decisions-api-openapi.yml
- filename: llmgateway-io-embeddings-api-openapi.yml
  format: yaml
  label: LLM Gateway Embeddings API
  slug: llmgateway-io-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llmgateway-io/refs/heads/main/openapi/llmgateway-io-embeddings-api-openapi.yml
- filename: llmgateway-io-images-api-openapi.yml
  format: yaml
  label: LLM Gateway Images API
  slug: llmgateway-io-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llmgateway-io/refs/heads/main/openapi/llmgateway-io-images-api-openapi.yml
- filename: llmgateway-io-key-api-openapi.yml
  format: yaml
  label: LLM Gateway Key API
  slug: llmgateway-io-key-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llmgateway-io/refs/heads/main/openapi/llmgateway-io-key-api-openapi.yml
- filename: llmgateway-io-llm-gateway-api-api-openapi.yml
  format: yaml
  label: LLM Gateway LLM Gateway API
  slug: llmgateway-io-llm-gateway-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llmgateway-io/refs/heads/main/openapi/llmgateway-io-llm-gateway-api-api-openapi.yml
- filename: llmgateway-io-messages-api-openapi.yml
  format: yaml
  label: LLM Gateway Messages API
  slug: llmgateway-io-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llmgateway-io/refs/heads/main/openapi/llmgateway-io-messages-api-openapi.yml
- filename: llmgateway-io-models-api-openapi.yml
  format: yaml
  label: LLM Gateway Models API
  slug: llmgateway-io-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llmgateway-io/refs/heads/main/openapi/llmgateway-io-models-api-openapi.yml
- filename: llmgateway-io-moderations-api-openapi.yml
  format: yaml
  label: LLM Gateway Moderations API
  slug: llmgateway-io-moderations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llmgateway-io/refs/heads/main/openapi/llmgateway-io-moderations-api-openapi.yml
- filename: llmgateway-io-ocr-api-openapi.yml
  format: yaml
  label: LLM Gateway Ocr API
  slug: llmgateway-io-ocr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llmgateway-io/refs/heads/main/openapi/llmgateway-io-ocr-api-openapi.yml
- filename: llmgateway-io-realtime-api-openapi.yml
  format: yaml
  label: LLM Gateway Realtime API
  slug: llmgateway-io-realtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llmgateway-io/refs/heads/main/openapi/llmgateway-io-realtime-api-openapi.yml
- filename: llmgateway-io-rerank-api-openapi.yml
  format: yaml
  label: LLM Gateway Rerank API
  slug: llmgateway-io-rerank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llmgateway-io/refs/heads/main/openapi/llmgateway-io-rerank-api-openapi.yml
- filename: llmgateway-io-search-api-openapi.yml
  format: yaml
  label: LLM Gateway Search API
  slug: llmgateway-io-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llmgateway-io/refs/heads/main/openapi/llmgateway-io-search-api-openapi.yml
- filename: llmgateway-io-systemone-api-openapi.yml
  format: yaml
  label: LLM Gateway Systemone API
  slug: llmgateway-io-systemone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llmgateway-io/refs/heads/main/openapi/llmgateway-io-systemone-api-openapi.yml
- filename: llmgateway-io-videos-api-openapi.yml
  format: yaml
  label: LLM Gateway Videos API
  slug: llmgateway-io-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llmgateway-io/refs/heads/main/openapi/llmgateway-io-videos-api-openapi.yml
- filename: llmgateway-io-chat-completions-api-openapi.yml
  format: yaml
  label: LLM Gateway Chat Completions API
  slug: llmgateway-io-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llmgateway-io/refs/heads/main/openapi/llmgateway-io-chat-completions-api-openapi.yml
consequence_counts:
  read: 7
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Llmgateway Io Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 21
overview: 'LLM Gateway exposes 21 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 14 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: LLM Gateway
provider_slug: llmgateway-io
slug: llmgateway-io-agentic-access
source_filename: llmgateway-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: generated\nsource: openapi/llmgateway-io-gateway-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    connected: 7\n    acting: 14\n  by_consequence:\n    read: 7\n    write: 14\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chat/completions\n  method: post\n  operationId: v1_chat_completions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/embeddings\n  method: post\n  operationId: v1_embeddings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/images/generations\n  method: post\n  operationId: v1_images_generations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/images/edits\n  method: post\n  operationId: v1_images_edits\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/key\n  method: get\n  operationId: v1_key_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/models\n  method: get\n  operationId: v1_models\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/moderations\n  method: post\n  operationId: v1_moderations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ocr\n  method: post\n  operationId: v1_ocr\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/rerank\n  method: post\n  operationId: v1_rerank\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/search\n  method: post\n  operationId: v1_search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/decisions\n  method: post\n  operationId: v1_decisions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/systemone\n  method: post\n  operationId: v1_systemone\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/messages\n  method: post\n  operationId: v1_messages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/audio/speech\n  method: post\n  operationId: v1_audio_speech\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/audio/transcriptions\n  method: post\n  operationId: v1_audio_transcriptions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/realtime/client_secrets\n  method: post\n  operationId: v1_realtime_client_secrets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos\n  method: post\n  operationId: v1_videos_create\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos/{video_id}\n  method: get\n  operationId: v1_videos_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/videos/logs/{log_id}/content\n  method: get\n  operationId: v1_videos_log_content\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/videos/{video_id}/content\n  method: get\n  operationId: v1_videos_content\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/llmgateway-io/refs/heads/main/agentic-access/llmgateway-io-agentic-access.yml
summary_line: 21 operations · 14 acting
tags:
- Artificial Intelligence
- LLM Gateway
- Decision Support
- Structured Outputs
- Inference
- MCP
---
