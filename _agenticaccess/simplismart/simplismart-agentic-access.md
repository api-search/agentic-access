---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 10
api_specs:
- filename: simplismart-llama-3.3-70b-openapi.yml
  format: yaml
  label: Simplismart LLM Inference API
  slug: simplismart-llm-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplismart/refs/heads/main/openapi/simplismart-llama-3.3-70b-openapi.yml
- filename: simplismart-flux-dev-openapi.yml
  format: yaml
  label: Simplismart Image Generation API
  slug: simplismart-image-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplismart/refs/heads/main/openapi/simplismart-flux-dev-openapi.yml
- filename: simplismart-whisper-v3-openapi.yml
  format: yaml
  label: Simplismart Audio Transcription API
  slug: simplismart-audio-transcription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplismart/refs/heads/main/openapi/simplismart-whisper-v3-openapi.yml
- filename: simplismart-llm-training-openapi.yml
  format: yaml
  label: Simplismart Training API
  slug: simplismart-training-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplismart/refs/heads/main/openapi/simplismart-llm-training-openapi.yml
consequence_counts:
  read: 10
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Simplismart Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 25
overview: 'Simplismart exposes 25 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 15 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Simplismart
provider_slug: simplismart
slug: simplismart-agentic-access
source_filename: simplismart-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/simplismart-deepseek-r1-qwen-32b-openapi.yml, openapi/simplismart-devstral-small-openapi.yml,\n  openapi/simplismart-flux-dev-openapi.yml, openapi/simplismart-flux-jobs-list-openapi.yml,\n  openapi/simplismart-flux-post-training-openapi.yml, openapi/simplismart-flux-training-openapi.yml,\n  openapi/simplismart-gemma3-27b-openapi.yml, openapi/simplismart-gemma3-4b-openapi.yml, openapi/simplismart-job-by-request-openapi.yml,\n  openapi/simplismart-llama-3.3-70b-openapi.yml, openapi/simplismart-llama-4-maverick-17b-openapi.yml,\n  openapi/simplismart-llama-8b-openapi.yml, openapi/simplismart-llm-jobs-list-openapi.yml, openapi/simplismart-llm-metrics-openapi.yml,\n  openapi/simplismart-llm-training-openapi.yml, openapi/simplismart-mixtral-8x7b-openapi.yml,\n  openapi/simplismart-qwen-32b-openapi.yml, openapi/simplismart-whisper-v2-openapi.yml, openapi/simplismart-whisper-v3-openapi.yml\ndescription: Recommended x-agentic-access\
  \ execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 25\n  by_action_class:\n    acting: 15\n    connected: 10\n  by_consequence:\n    write: 15\n    read: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /chat/completions\n  method: post\n  operationId: createChatCompletion70B\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chat/completions\n  method: post\n  operationId: createChatCompletion8B\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /model/infer/flux\n  method: post\n  operationId: generateImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/flux/training_job/list/\n  method: get\n  operationId: listFluxTrainingJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/flux/train/\n  method: post\n  operationId: trainModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/flux/train/\n  method: post\n  operationId: startFluxTrainingJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/flux/training_job/list/\n  method: get\n  operationId: listFluxTrainingJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/flux/training_job/get/\n  method: get\n  operationId: getFluxTrainingJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/flux/training_job/get/mlflow-metrics/\n  method: get\n  operationId: getFluxTrainingMetrics\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chat/completions\n  method: post\n  operationId: createChatCompletionGemma34B\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chat/completions\n  method: post\n  operationId: createChatCompletionGemma34B\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/llm/training_job/list/\n  method: get\n  operationId: listTrainingJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chat/completions\n  method: post\n  operationId: createChatCompletion70B\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chat/completions\n  method: post\n  operationId: createChatCompletion70B\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chat/completions\n  method: post\n  operationId: createChatCompletion8B\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/llm/training_job/list/\n  method: get\n  operationId: listTrainingJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get/metrics/{request_id}\n  method: get\n  operationId: getChatMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /job/\n  method: post\n  operationId: createTrainingJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /job/list/\n  method: get\n  operationId:\
  \ listTrainingJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /job/get/\n  method: get\n  operationId: getTrainingJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /job/metrics/\n  method: get\n  operationId: getTrainingMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chat/completions\n  method: post\n  operationId: createChatCompletion8B\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chat/completions\n  method: post\n \
  \ operationId: createChatCompletionQwen32B\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /model/v2/infer/whisper\n  method: post\n  operationId: transcribeAudioV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /model/infer/whisper\n  method: post\n  operationId: transcribeAudioV3\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n  \
  \    - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simplismart/refs/heads/main/agentic-access/simplismart-agentic-access.yml
summary_line: 25 operations · 15 acting
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Inference
- LLM
- Model Deployment
- Fine-Tuning
- MLOps
- GPU
- Speech to Text
- Image Generation
---
