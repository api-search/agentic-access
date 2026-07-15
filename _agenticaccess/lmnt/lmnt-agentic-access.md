---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 6
api_specs:
- filename: lmnt-speech-openapi.yml
  format: yaml
  label: LMNT Speech API
  slug: lmnt-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lmnt/refs/heads/main/openapi/lmnt-speech-openapi.yml
consequence_counts:
  read: 6
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Lmnt Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'LMNT exposes 14 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: LMNT
provider_slug: lmnt
slug: lmnt-agentic-access
source_filename: lmnt-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/lmnt-speech-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 6\n    acting: 8\n  by_consequence:\n    read: 6\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/ai/speech\n  method: get\n  operationId: get_handler_v1_ai_speech_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ai/speech\n  method: post\n  operationId: post_handler_v1_ai_speech_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ai/speech/bytes\n  method: post\n  operationId: bytes_post_handler_v1_ai_speech_bytes_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ai/speech/feedback\n  method: post\n  operationId: feedback_handler_v1_ai_speech_feedback_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ai/voice/list\n  method: get\n  operationId: list_handler_v1_ai_voice_list_get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ai/voice/{id}\n  method: get\n  operationId: get_handler_v1_ai_voice__id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ai/voice/{id}\n  method: put\n  operationId: update_handler_v1_ai_voice__id__put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ai/voice/{id}\n  method: delete\n  operationId: delete_handler_v1_ai_voice__id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ai/voice\n  method: post\n  operationId: create_handler_v1_ai_voice_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ai/voice/{id}/preview\n  method: get\n  operationId: preview_handler_v1_ai_voice__id__preview_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ai/voice/precheck\n  method: post\n  operationId: precheck_clone_handler_v1_ai_voice_precheck_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /speech/beta/synthesize\n  method: post\n  operationId: synthesize_beta_handler_speech_beta_synthesize_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /speech/beta/voices\n  method: get\n  operationId: list_beta_handler_speech_beta_voices_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health_check\n  method: get\n  operationId: health_check_health_check_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lmnt/refs/heads/main/agentic-access/lmnt-agentic-access.yml
summary_line: 14 operations · 8 acting
tags:
- text-to-speech
- voice synthesis
- voice cloning
- audio streaming
- conversational AI
- low latency
- real-time audio
---
