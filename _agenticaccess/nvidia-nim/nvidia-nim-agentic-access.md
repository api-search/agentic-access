---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 5
api_specs:
- filename: nvidia-nim-chat-completions-api-openapi.yml
  format: yaml
  label: NVIDIA NIM Chat Completions API
  slug: nvidia-nim-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nvidia-nim/refs/heads/main/openapi/nvidia-nim-chat-completions-api-openapi.yml
- filename: nvidia-nim-completions-api-openapi.yml
  format: yaml
  label: NVIDIA NIM Completions API
  slug: nvidia-nim-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nvidia-nim/refs/heads/main/openapi/nvidia-nim-completions-api-openapi.yml
- filename: nvidia-nim-embeddings-api-openapi.yml
  format: yaml
  label: NVIDIA NIM Embeddings API
  slug: nvidia-nim-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nvidia-nim/refs/heads/main/openapi/nvidia-nim-embeddings-api-openapi.yml
- filename: nvidia-nim-reranking-api-openapi.yml
  format: yaml
  label: NVIDIA NIM Reranking API
  slug: nvidia-nim-reranking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nvidia-nim/refs/heads/main/openapi/nvidia-nim-reranking-api-openapi.yml
- filename: nvidia-nim-models-api-openapi.yml
  format: yaml
  label: NVIDIA NIM Models API
  slug: nvidia-nim-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nvidia-nim/refs/heads/main/openapi/nvidia-nim-models-api-openapi.yml
- filename: nvidia-nim-vision-api-openapi.yml
  format: yaml
  label: NVIDIA NIM Vision Language Models API
  slug: nvidia-nim-vision-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nvidia-nim/refs/heads/main/openapi/nvidia-nim-vision-api-openapi.yml
- filename: nvidia-nim-health-api-openapi.yml
  format: yaml
  label: NVIDIA NIM Health API
  slug: nvidia-nim-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nvidia-nim/refs/heads/main/openapi/nvidia-nim-health-api-openapi.yml
- filename: nvidia-nim-image-generation-api-openapi.yml
  format: yaml
  label: NVIDIA NIM Image Generation API
  slug: nvidia-nim-image-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nvidia-nim/refs/heads/main/openapi/nvidia-nim-image-generation-api-openapi.yml
- filename: nvidia-nim-speech-api-openapi.yml
  format: yaml
  label: NVIDIA NIM Speech API
  slug: nvidia-nim-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nvidia-nim/refs/heads/main/openapi/nvidia-nim-speech-api-openapi.yml
- filename: nvidia-nim-biology-api-openapi.yml
  format: yaml
  label: NVIDIA NIM Biology (BioNeMo) API
  slug: nvidia-nim-biology-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nvidia-nim/refs/heads/main/openapi/nvidia-nim-biology-api-openapi.yml
consequence_counts:
  read: 5
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Nvidia Nim Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'NVIDIA NIM exposes 16 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 11 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: NVIDIA NIM
provider_slug: nvidia-nim
slug: nvidia-nim-agentic-access
source_filename: nvidia-nim-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/nvidia-nim-biology-api-openapi.yml, openapi/nvidia-nim-chat-completions-api-openapi.yml,\n  openapi/nvidia-nim-completions-api-openapi.yml, openapi/nvidia-nim-embeddings-api-openapi.yml,\n  openapi/nvidia-nim-health-api-openapi.yml, openapi/nvidia-nim-image-generation-api-openapi.yml,\n  openapi/nvidia-nim-models-api-openapi.yml, openapi/nvidia-nim-reranking-api-openapi.yml, openapi/nvidia-nim-speech-api-openapi.yml,\n  openapi/nvidia-nim-vision-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    acting: 11\n    connected: 5\n  by_consequence:\n    write: 11\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/biology/nvidia/alphafold2/predict-structure-from-sequence\n\
  \  method: post\n  operationId: predictProteinStructure\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/biology/mit/diffdock\n  method: post\n  operationId: dockLigand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/biology/nvidia/molmim/generate\n  method: post\n  operationId: generateMolecules\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chat/completions\n  method: post\n  operationId: createChatCompletion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/completions\n  method: post\n  operationId: createCompletion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/embeddings\n  method: post\n  operationId: createEmbedding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/health/live\n  method: get\n  operationId: getLiveness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/health/ready\n  method: get\n  operationId: getReadiness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/metrics\n  method: get\n  operationId: getMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/genai/{publisher}/{model}\n  method: post\n  operationId: generateImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/models\n  method: get\n  operationId: listModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/models/{model_id}\n  method: get\n  operationId: getModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ranking\n  method: post\n  operationId: rankPassages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/audio/transcriptions\n  method: post\n  operationId: createTranscription\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/audio/speech\n  method: post\n  operationId: createSpeech\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chat/completions\n  method: post\n  operationId: createVisionChatCompletion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nvidia-nim/refs/heads/main/agentic-access/nvidia-nim-agentic-access.yml
summary_line: 16 operations · 11 acting
tags:
- AI
- Artificial Intelligence
- Inference
- Microservices
- LLM
- Foundation Models
- GPU
- Kubernetes
- NVIDIA
- OpenAI Compatible
---
