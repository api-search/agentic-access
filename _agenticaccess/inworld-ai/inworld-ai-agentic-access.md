---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 7
api_specs:
- filename: inworld-tts-api-openapi.yml
  format: yaml
  label: Inworld TTS API
  slug: inworld-tts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inworld-ai/refs/heads/main/openapi/inworld-tts-api-openapi.yml
- filename: inworld-voice-api-openapi.yml
  format: yaml
  label: Inworld Voice API
  slug: inworld-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inworld-ai/refs/heads/main/openapi/inworld-voice-api-openapi.yml
- filename: inworld-stt-api-openapi.yml
  format: yaml
  label: Inworld STT API
  slug: inworld-stt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inworld-ai/refs/heads/main/openapi/inworld-stt-api-openapi.yml
- filename: inworld-realtime-api-openapi.yml
  format: yaml
  label: Inworld Realtime API
  slug: inworld-realtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inworld-ai/refs/heads/main/openapi/inworld-realtime-api-openapi.yml
- filename: inworld-router-api-openapi.yml
  format: yaml
  label: Inworld LLM Router API
  slug: inworld-router-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inworld-ai/refs/heads/main/openapi/inworld-router-api-openapi.yml
- filename: inworld-models-api-openapi.yml
  format: yaml
  label: Inworld Models API
  slug: inworld-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inworld-ai/refs/heads/main/openapi/inworld-models-api-openapi.yml
consequence_counts:
  read: 7
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Inworld Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'Inworld AI exposes 16 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 9 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Inworld AI
provider_slug: inworld-ai
slug: inworld-ai-agentic-access
source_filename: inworld-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/inworld-models-api-openapi.yml, openapi/inworld-realtime-api-openapi.yml, openapi/inworld-stt-api-openapi.yml,\n  openapi/inworld-tts-api-openapi.yml, openapi/inworld-voice-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 7\n    acting: 9\n  by_consequence:\n    read: 7\n    write: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/models\n  method: get\n  operationId: listModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/realtime/session\n  method: get\n  operationId: realtimeWebsocket\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/realtime/webrtc\n  method: post\n  operationId: realtimeWebrtc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stt/v1/transcribe\n  method: post\n  operationId: transcribeAudio\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stt/v1/transcribe:stream\n  method: get\n  operationId: streamTranscribe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tts/v1/voice\n  method: post\n  operationId: synthesizeSpeech\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tts/v1/voice:stream\n  method: post\n  operationId: streamSynthesizeSpeech\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tts/v1/voice:websocket\n  method: get\n  operationId: websocketSynthesizeSpeech\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /tts/v1/voices\n  method: get\n  operationId: listTtsVoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /voices/v1/voices\n  method: get\n  operationId: listVoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /voices/v1/voices:clone\n  method: post\n  operationId: cloneVoice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /voices/v1/voices:design\n  method: post\n  operationId: designVoice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n    \
  \  max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /voices/v1/voices:publish\n  method: post\n  operationId: publishVoice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /voices/v1/voices/{voiceId}\n  method: get\n  operationId: getVoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /voices/v1/voices/{voiceId}\n  method: patch\n  operationId: updateVoice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /voices/v1/voices/{voiceId}\n  method: delete\n  operationId: deleteVoice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inworld-ai/refs/heads/main/agentic-access/inworld-ai-agentic-access.yml
summary_line: 16 operations · 9 acting
tags:
- AI
- Artificial Intelligence
- Voice
- Text To Speech
- Speech To Text
- Realtime
- LLM Routing
- Voice Cloning
- Conversational AI
- Game AI
---
