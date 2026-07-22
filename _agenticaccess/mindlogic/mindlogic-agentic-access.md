---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 8
api_specs:
- filename: mindlogic-api-gateway-openapi-original.json
  format: json
  label: FactChat API Gateway
  slug: factchat-api-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindlogic/refs/heads/main/openapi/mindlogic-api-gateway-openapi-original.json
consequence_counts:
  read: 8
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Mindlogic Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'Mindlogic exposes 17 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 9 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Mindlogic
provider_slug: mindlogic
slug: mindlogic-agentic-access
source_filename: mindlogic-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/mindlogic-api-gateway-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    connected: 8\n    acting: 9\n  by_consequence:\n    read: 8\n    write: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /models/\n  method: get\n  operationId: list_models_models__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /models/{model}/\n  method: get\n  operationId: get_model_models__model___get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /chat/completions/\n  method: post\n  operationId: chat_completions_chat_completions__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chatbots/{chatbot_id}/chat/completions/\n  method: post\n  operationId: GatewayChatbotChatCompletions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claude/v1/models/\n  method: get\n  operationId: AnthropicListModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /claude/v1/messages/\n\
  \  method: post\n  operationId: AnthropicMessages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claude/v1/messages/count_tokens/\n  method: post\n  operationId: AnthropicCountTokens\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /responses/\n  method: post\n  operationId: CreateResponse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /responses/{response_id}/\n  method: get\n  operationId: GetResponse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /responses/{response_id}/cancel/\n  method: post\n  operationId: CancelResponse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /audio/speech/\n  method: post\n  operationId: text_to_speech_audio_speech__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /images/generate/\n  method: post\n  operationId: generate_image_images_generate__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /images/generate/{operation_id}/\n  method: get\n  operationId: poll_image_status_images_generate__operation_id___get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /video/generation/\n  method: post\n  operationId: create_video_video_generation__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n \
  \   audit: required\n- path: /video/generation/{operation_id}/download/\n  method: get\n  operationId: download_video_file_video_generation__operation_id__download__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /video/generation/{operation_id}/\n  method: get\n  operationId: get_video_generation_status_video_generation__operation_id___get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /credits/\n  method: get\n  operationId: get_credit_balance_credits__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mindlogic/refs/heads/main/agentic-access/mindlogic-agentic-access.yml
summary_line: 17 operations · 9 acting
tags:
- Company
- AI/ML
- Generative AI
- Conversational AI
- LLM Gateway
- Chatbots
- API Gateway
- Korea
---
