---
acting_count: 19
action_class_counts:
  acting: 19
  connected: 10
api_specs:
- filename: openapi.json
  format: json
  label: Mistral AI Chat API
  slug: mistral-ai-chat-api
  spec_type: OpenAPI
  url: https://docs.mistral.ai/openapi.json
- filename: mistral-embeddings-openapi.yml
  format: yaml
  label: Mistral Embeddings API
  slug: mistral-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-embeddings-openapi.yml
- filename: mistral-moderation-openapi.yml
  format: yaml
  label: Mistral Moderation API
  slug: mistral-moderation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-moderation-openapi.yml
- filename: mistral-agents-openapi.yml
  format: yaml
  label: Mistral AI Agents API
  slug: mistral-ai-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-agents-openapi.yml
- filename: mistral-fim-openapi.yml
  format: yaml
  label: Mistral AI FIM API
  slug: mistral-ai-fim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-fim-openapi.yml
- filename: mistral-ocr-openapi.yml
  format: yaml
  label: Mistral AI OCR API
  slug: mistral-ai-ocr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-ocr-openapi.yml
- filename: mistral-fine-tuning-openapi.yml
  format: yaml
  label: Mistral AI Fine-Tuning API
  slug: mistral-ai-fine-tuning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-fine-tuning-openapi.yml
- filename: mistral-files-openapi.yml
  format: yaml
  label: Mistral AI Files API
  slug: mistral-ai-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-files-openapi.yml
- filename: mistral-models-openapi.yml
  format: yaml
  label: Mistral AI Models API
  slug: mistral-ai-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-models-openapi.yml
- filename: mistral-batch-openapi.yml
  format: yaml
  label: Mistral AI Batch API
  slug: mistral-ai-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-batch-openapi.yml
- filename: mistral-audio-transcription-openapi.yml
  format: yaml
  label: Mistral AI Audio Transcription API
  slug: mistral-ai-audio-transcription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-audio-transcription-openapi.yml
consequence_counts:
  read: 10
  write: 19
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Mistral Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 29
overview: 'Mistral AI exposes 29 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 19 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Mistral AI
provider_slug: mistral
slug: mistral-agentic-access
source_filename: mistral-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/mistral-agents-openapi.yml, openapi/mistral-audio-transcription-openapi.yml,\n  openapi/mistral-batch-openapi.yml, openapi/mistral-chat-openapi.yml, openapi/mistral-embeddings-openapi.yml,\n  openapi/mistral-files-openapi.yml, openapi/mistral-fim-openapi.yml, openapi/mistral-fine-tuning-openapi.yml,\n  openapi/mistral-models-openapi.yml, openapi/mistral-moderation-openapi.yml, openapi/mistral-ocr-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 29\n  by_action_class:\n    acting: 19\n    connected: 10\n  by_consequence:\n    write: 19\n    read: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /agents/completions\n  method: post\n  operationId: createAgentCompletion\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /audio/transcriptions\n  method: post\n  operationId: createTranscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /batch/jobs\n  method: get\n  operationId: listBatchJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /batch/jobs\n  method: post\n  operationId: createBatchJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /batch/jobs/{job_id}\n  method: get\n  operationId: getBatchJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /batch/jobs/{job_id}/cancel\n  method: post\n  operationId: cancelBatchJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chat/completions\n  method: post\n  operationId: createChatCompletion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /embeddings\n  method: post\n  operationId: createEmbedding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files\n  method: get\n  operationId: listFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files\n  method: post\n  operationId: uploadFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n   \
  \ audit: required\n- path: /files/{file_id}\n  method: get\n  operationId: getFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/{file_id}\n  method: delete\n  operationId: deleteFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files/{file_id}/content\n  method: get\n  operationId: downloadFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/{file_id}/url\n  method: get\n  operationId: getFileSignedUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /fim/completions\n  method: post\n  operationId: createFimCompletion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fine_tuning/jobs\n  method: get\n  operationId: listFineTuningJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fine_tuning/jobs\n  method: post\n  operationId: createFineTuningJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fine_tuning/jobs/{job_id}\n  method:\
  \ get\n  operationId: getFineTuningJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fine_tuning/jobs/{job_id}/cancel\n  method: post\n  operationId: cancelFineTuningJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fine_tuning/jobs/{job_id}/start\n  method: post\n  operationId: startFineTuningJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /models\n  method: get\n  operationId: listModels\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /models/{model_id}\n  method: get\n  operationId: getModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /models/{model_id}\n  method: patch\n  operationId: updateModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /models/{model_id}\n  method: delete\n  operationId: deleteModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /models/{model_id}/archive\n  method: post\n  operationId: archiveModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /models/{model_id}/unarchive\n  method: post\n  operationId: unarchiveModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /moderations\n  method: post\n  operationId: createModeration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n   \
  \   human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chat/moderations\n  method: post\n  operationId: createChatModeration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ocr\n  method: post\n  operationId: processDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/agentic-access/mistral-agentic-access.yml
summary_line: 29 operations · 19 acting
tags: []
---
