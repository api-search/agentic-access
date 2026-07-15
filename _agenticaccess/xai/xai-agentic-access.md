---
acting_count: 16
action_class_counts:
  acting: 16
  connected: 17
api_specs:
- filename: xai-openapi.json
  format: json
  label: xAI Chat Completions API
  slug: xai-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xai/refs/heads/main/openapi/xai-openapi.json
- filename: xai-openapi.json
  format: json
  label: xAI Responses API
  slug: xai-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xai/refs/heads/main/openapi/xai-openapi.json
- filename: xai-openapi.json
  format: json
  label: xAI Images API
  slug: xai-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xai/refs/heads/main/openapi/xai-openapi.json
- filename: xai-openapi.json
  format: json
  label: xAI Video Generation API
  slug: xai-video-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xai/refs/heads/main/openapi/xai-openapi.json
- filename: xai-openapi.json
  format: json
  label: xAI Voice API
  slug: xai-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xai/refs/heads/main/openapi/xai-openapi.json
- filename: xai-openapi.json
  format: json
  label: xAI Embeddings API
  slug: xai-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xai/refs/heads/main/openapi/xai-openapi.json
- filename: xai-openapi.json
  format: json
  label: xAI Models API
  slug: xai-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xai/refs/heads/main/openapi/xai-openapi.json
- filename: xai-openapi.json
  format: json
  label: xAI Batch API
  slug: xai-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xai/refs/heads/main/openapi/xai-openapi.json
consequence_counts:
  read: 17
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Xai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 33
overview: 'xAI exposes 33 API operations that an AI agent could call, of which 16 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read and 16 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: xAI
provider_slug: xai
slug: xai-agentic-access
source_filename: xai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/xai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 33\n  by_action_class:\n    connected: 17\n    acting: 16\n  by_consequence:\n    read: 17\n    write: 16\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/api-key\n  method: get\n  operationId: handle_get_api_key_info_request\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chat/completions\n  method: post\n  operationId: handle_generic_completion_request\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chat/deferred-completion/{request_id}\n  method: get\n  operationId: handle_get_deferred_completion_request\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/complete\n  method: post\n  operationId: handle_generic_complete_request\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/completions\n  method: post\n  operationId: handle_sample_request\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/documents/search\n  method: post\n  operationId: handle_document_search_request_v2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/embedding-models\n  method: get\n  operationId: handle_embedding_models_list_request\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/embedding-models/{model_id}\n  method: get\n  operationId: handle_embedding_model_get_request\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/embeddings\n\
  \  method: post\n  operationId: handle_embedding_request\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/files\n  method: get\n  operationId: handle_list_files_request\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/files\n  method: post\n  operationId: handle_upload_file_request\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/files/{file_id}\n  method: get\n  operationId: handle_retrieve_file_request\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/files/{file_id}\n  method: delete\n  operationId: handle_delete_file_request\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/files/{file_id}/content\n  method: get\n  operationId: handle_download_file_content_request\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/image-generation-models\n  method: get\n  operationId: handle_image_generation_models_list_request\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/image-generation-models/{model_id}\n  method: get\n  operationId: handle_image_generation_model_get_request\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/images/edits\n  method: post\n  operationId: handle_edit_image_request\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/images/generations\n  method: post\n  operationId: handle_generate_image_request\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/language-models\n  method: get\n  operationId: handle_language_models_list_request\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/language-models/{model_id}\n  method: get\n  operationId: handle_language_model_get_request\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/messages\n  method: post\n  operationId: handle_generic_messages_request\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/models\n  method: get\n  operationId: handle_models_list_request\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/models/{model_id}\n  method: get\n  operationId: handle_model_get_request\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/responses\n  method: post\n  operationId: handle_generic_model_request\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/responses/{response_id}\n  method: get\n  operationId: handle_get_stored_completion_request\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/responses/{response_id}\n  method: delete\n  operationId:\
  \ handle_delete_stored_completion_request\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tokenize-text\n  method: post\n  operationId: handle_tokenize_text_request\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/video-generation-models\n  method: get\n  operationId: handle_video_generation_models_list_request\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/video-generation-models/{model_id}\n  method:\
  \ get\n  operationId: handle_video_generation_model_get_request\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/videos/edits\n  method: post\n  operationId: handle_edit_video_request\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos/extensions\n  method: post\n  operationId: handle_extend_video_request\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos/generations\n  method: post\n  operationId:\
  \ handle_generate_video_request\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos/{request_id}\n  method: get\n  operationId: handle_get_deferred_video_request\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xai/refs/heads/main/agentic-access/xai-agentic-access.yml
summary_line: 33 operations · 16 acting
tags:
- AI
- LLM
- Foundation Models
- Grok
- Generative AI
---
