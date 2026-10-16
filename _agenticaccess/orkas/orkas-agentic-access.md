---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 5
api_specs:
- filename: orkas-audio-api-openapi.yml
  format: yaml
  label: Orkas Audio API
  slug: orkas-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orkas/refs/heads/main/openapi/orkas-audio-api-openapi.yml
- filename: orkas-images-api-openapi.yml
  format: yaml
  label: Orkas Images API
  slug: orkas-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orkas/refs/heads/main/openapi/orkas-images-api-openapi.yml
- filename: orkas-openapi-json-api-openapi.yml
  format: yaml
  label: Orkas Openapi.json API
  slug: orkas-openapi-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orkas/refs/heads/main/openapi/orkas-openapi-json-api-openapi.yml
- filename: orkas-search-api-openapi.yml
  format: yaml
  label: Orkas Search API
  slug: orkas-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orkas/refs/heads/main/openapi/orkas-search-api-openapi.yml
- filename: orkas-videos-api-openapi.yml
  format: yaml
  label: Orkas Videos API
  slug: orkas-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orkas/refs/heads/main/openapi/orkas-videos-api-openapi.yml
- filename: orkas-chat-completions-api-openapi.yml
  format: yaml
  label: Orkas Chat Completions API
  slug: orkas-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orkas/refs/heads/main/openapi/orkas-chat-completions-api-openapi.yml
consequence_counts:
  read: 5
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Orkas Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'Orkas exposes 9 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Orkas
provider_slug: orkas
slug: orkas-agentic-access
source_filename: orkas-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: generated\nsource: openapi/orkas-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 5\n    acting: 4\n  by_consequence:\n    read: 5\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/openapi.json\n  method: get\n  operationId: openapi_document_v1_openapi_json_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chat/completions\n  method: post\n  operationId: chat_completions_v1_chat_completions_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/search\n  method: post\n  operationId: search_v1_search_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/audio/voices\n  method: get\n  operationId: audio_voices_v1_audio_voices_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/audio/speech\n  method: post\n  operationId: audio_speech_v1_audio_speech_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/images/generations\n  method:\
  \ post\n  operationId: image_generations_v1_images_generations_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/images/generations/{task_id}\n  method: get\n  operationId: image_generation_v1_images_generations__task_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/videos\n  method: post\n  operationId: videos_v1_videos_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos/{task_id}\n\
  \  method: get\n  operationId: video_v1_videos__task_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orkas/refs/heads/main/agentic-access/orkas-agentic-access.yml
summary_line: 9 operations · 4 acting
tags:
- Company
- AI
- API
- Chatbot
- Media
---
