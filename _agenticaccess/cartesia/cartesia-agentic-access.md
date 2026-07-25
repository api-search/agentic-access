---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 2
api_specs:
- filename: cartesia-asyncapi.yml
  format: yaml
  label: Cartesia Sonic Text-to-Speech API
  slug: tts-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/cartesia/refs/heads/main/asyncapi/cartesia-asyncapi.yml
- filename: cartesia-asyncapi.yml
  format: yaml
  label: Cartesia Ink Speech-to-Text API
  slug: stt-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/cartesia/refs/heads/main/asyncapi/cartesia-asyncapi.yml
- filename: cartesia-auth-api-openapi.yml
  format: yaml
  label: Cartesia Auth API
  slug: cartesia-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cartesia/refs/heads/main/openapi/cartesia-auth-api-openapi.yml
- filename: cartesia-stt-api-openapi.yml
  format: yaml
  label: Cartesia STT API
  slug: cartesia-stt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cartesia/refs/heads/main/openapi/cartesia-stt-api-openapi.yml
- filename: cartesia-tts-api-openapi.yml
  format: yaml
  label: Cartesia TTS API
  slug: cartesia-tts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cartesia/refs/heads/main/openapi/cartesia-tts-api-openapi.yml
- filename: cartesia-voices-api-openapi.yml
  format: yaml
  label: Cartesia Voices API
  slug: cartesia-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cartesia/refs/heads/main/openapi/cartesia-voices-api-openapi.yml
consequence_counts:
  read: 2
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cartesia Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'Cartesia exposes 10 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cartesia
provider_slug: cartesia
slug: cartesia-agentic-access
source_filename: cartesia-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/cartesia-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    acting: 8\n    connected: 2\n  by_consequence:\n    write: 8\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /tts/bytes\n  method: post\n  operationId: ttsBytes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tts/sse\n  method: post\n  operationId: ttsSse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stt/transcribe\n  method: post\n  operationId: sttTranscribe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /voices\n  method: get\n  operationId: listVoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /voices/{id}\n  method: get\n  operationId: getVoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /voices/{id}\n  method: patch\n  operationId:\
  \ updateVoice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /voices/{id}\n  method: delete\n  operationId: deleteVoice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /voices/clone\n  method: post\n  operationId: cloneVoice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /voices/localize\n\
  \  method: post\n  operationId: localizeVoice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/access-token\n  method: post\n  operationId: generateAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cartesia/refs/heads/main/agentic-access/cartesia-agentic-access.yml
summary_line: 10 operations · 8 acting
tags:
- Voice
- TTS
- Text to Speech
- STT
- Speech to Text
- Streaming
- WebSocket
- Voice Agents
- Voice Clone
- Sonic
- Ink
- Real-Time
---
