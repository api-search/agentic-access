---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 1
api_specs:
- filename: ex-human-openapi.yml
  format: yaml
  label: Ex-Human API
  slug: ex-human-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ex-human/refs/heads/main/openapi/ex-human-openapi.yml
consequence_counts:
  read: 1
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ex Human Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Ex-Human exposes 12 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 11 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Ex-Human
provider_slug: ex-human
slug: ex-human-agentic-access
source_filename: ex-human-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/ex-human-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    acting: 11\n    connected: 1\n  by_consequence:\n    write: 11\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /chatbot/v3/response\n  method: post\n  operationId: get_response_chatbot_v3_response_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chatbot/v2/get_smart_replies\n  method: post\n  operationId: get_smart_replies_chatbot_v2_get_smart_replies_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chatbot/v3/memory\n  method: delete\n  operationId: delete_memory_chatbot_v3_memory_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /animations/v3/create_bot\n  method: post\n  operationId: create_bot_v3_animations_v3_create_bot_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /animations/v3/generate_lipsync\n  method: post\n  operationId: generate_lipsync_v3_animations_v3_generate_lipsync_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /animations/v3/generate_lipsync_from_audio\n  method: post\n  operationId: generate_lipsync_from_audio_v3_animations_v3_generate_lipsync_from_audio_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /animations/v3/jobs\n  method: post\n  operationId: create_animation_job_animations_v3_jobs_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /animations/v3/jobs/{task_id}\n  method: get\n  operationId: get_animation_job_animations_v3_jobs__task_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /animations/v3/prolong_jobs\n  method: post\n  operationId: create_prolong_animation_job_animations_v3_prolong_jobs_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tts/v1/generate_speech\n  method: post\n  operationId: generate_speech_tts_v1_generate_speech_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /image/v1/generate_gallery_image\n  method: post\n  operationId: generate_gallery_image_image_v1_generate_gallery_image_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /image/v1/generate_avatar\n  method: post\n  operationId: generate_avatar_image_v1_generate_avatar_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ex-human/refs/heads/main/agentic-access/ex-human-agentic-access.yml
summary_line: 12 operations · 11 acting
tags:
- Company
- Artificial Intelligence
- Conversational AI
- AI Companions
- Generative AI
- Text to Speech
- Image Generation
- Video Generation
- Avatars
- Multimodal
---
