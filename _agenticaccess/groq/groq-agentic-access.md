---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 9
api_specs:
- filename: groq-openapi.yml
  format: yaml
  label: Groq Chat Completions API
  slug: groq-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/openapi/groq-openapi.yml
- filename: groq-openapi.yml
  format: yaml
  label: Groq Reasoning API
  slug: groq-reasoning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/openapi/groq-openapi.yml
- filename: groq-openapi.yml
  format: yaml
  label: Groq Vision API
  slug: groq-vision-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/openapi/groq-openapi.yml
- filename: groq-openapi.yml
  format: yaml
  label: Groq Speech-to-Text API
  slug: groq-speech-to-text-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/openapi/groq-openapi.yml
- filename: groq-openapi.yml
  format: yaml
  label: Groq Text-to-Speech API
  slug: groq-text-to-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/openapi/groq-openapi.yml
- filename: groq-openapi.yml
  format: yaml
  label: Groq Content Moderation API
  slug: groq-content-moderation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/openapi/groq-openapi.yml
- filename: groq-openapi.yml
  format: yaml
  label: Groq Batch API
  slug: groq-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/openapi/groq-openapi.yml
- filename: groq-openapi.yml
  format: yaml
  label: Groq Flex Processing API
  slug: groq-flex-processing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/openapi/groq-openapi.yml
- filename: groq-openapi.yml
  format: yaml
  label: Groq Files API
  slug: groq-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/openapi/groq-openapi.yml
- filename: groq-openapi.yml
  format: yaml
  label: Groq Models API
  slug: groq-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/openapi/groq-openapi.yml
- filename: groq-openapi.yml
  format: yaml
  label: Groq Tools API
  slug: groq-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/openapi/groq-openapi.yml
- filename: groq-openapi.yml
  format: yaml
  label: Groq LoRA Inference API
  slug: groq-lora-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/openapi/groq-openapi.yml
- filename: groq-openapi.yml
  format: yaml
  label: Groq Prompt Caching
  slug: groq-prompt-caching-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/openapi/groq-openapi.yml
consequence_counts:
  read: 9
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Groq Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 23
overview: 'Groq exposes 23 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 14 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Groq
provider_slug: groq
slug: groq-agentic-access
source_filename: groq-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/groq-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    acting: 14\n    connected: 9\n  by_consequence:\n    write: 14\n    read: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /openai/v1/audio/speech\n  method: post\n  operationId: createSpeech\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openai/v1/audio/transcriptions\n  method: post\n  operationId: createTranscription\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openai/v1/audio/translations\n  method: post\n  operationId: createTranslation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openai/v1/batches\n  method: post\n  operationId: createBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openai/v1/batches\n  method: get\n \
  \ operationId: listBatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openai/v1/batches/{batch_id}\n  method: get\n  operationId: retrieveBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openai/v1/batches/{batch_id}/cancel\n  method: post\n  operationId: cancelBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openai/v1/chat/completions\n  method: post\n  operationId: createChatCompletion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openai/v1/embeddings\n  method: post\n  operationId: createEmbedding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openai/v1/files\n  method: get\n  operationId: listFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openai/v1/files\n  method: post\n  operationId: uploadFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n     \
  \ - abnormal\n      - high-value\n    audit: required\n- path: /openai/v1/files/{file_id}\n  method: delete\n  operationId: deleteFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openai/v1/files/{file_id}\n  method: get\n  operationId: retrieveFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openai/v1/files/{file_id}/content\n  method: get\n  operationId: downloadFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fine_tunings\n  method: get\n  operationId: listFineTunings\n  x-agentic-access:\n    action-class: connected\n   \
  \ consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fine_tunings\n  method: post\n  operationId: createFineTuning\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/fine_tunings/{id}\n  method: delete\n  operationId: deleteFineTuning\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/fine_tunings/{id}\n  method: get\n  operationId: getFineTuning\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /openai/v1/models\n  method: get\n  operationId: listModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openai/v1/models/{model}\n  method: get\n  operationId: retrieveModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openai/v1/models/{model}\n  method: delete\n  operationId: deleteModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openai/v1/reranking\n  method: post\n  operationId: createReranking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n   \
  \ audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openai/v1/responses\n  method: post\n  operationId: createResponse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/agentic-access/groq-agentic-access.yml
summary_line: 23 operations · 14 acting
tags:
- AI
- LLM
- Inference
- LPU
- Low Latency
---
