---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 1
api_specs:
- filename: kotoba-transcription-openapi-original.yml
  format: yaml
  label: Kotoba Transcription API (Batch REST)
  slug: kotoba-transcription-api-batch-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kotoba/refs/heads/main/openapi/kotoba-transcription-openapi-original.yml
- filename: kotoba-asr-realtime-openapi-original.yml
  format: yaml
  label: Kotoba ASR Realtime API (WebSocket)
  slug: kotoba-asr-realtime-api-websocket
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kotoba/refs/heads/main/openapi/kotoba-asr-realtime-openapi-original.yml
- filename: kotoba-sts-realtime-openapi-original.yml
  format: yaml
  label: Kotoba Speech-to-Speech Translation API (WebSocket)
  slug: kotoba-speech-to-speech-translation-api-websocket
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kotoba/refs/heads/main/openapi/kotoba-sts-realtime-openapi-original.yml
- filename: kotoba-tts-realtime-openapi-original.yml
  format: yaml
  label: Kotoba TTS Realtime API (WebSocket)
  slug: kotoba-tts-realtime-api-websocket
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kotoba/refs/heads/main/openapi/kotoba-tts-realtime-openapi-original.yml
consequence_counts:
  read: 1
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Kotoba Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 2
overview: 'Kotoba exposes 2 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Kotoba
provider_slug: kotoba
slug: kotoba-agentic-access
source_filename: kotoba-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/kotoba-transcription-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 2\n  by_action_class:\n    acting: 1\n    connected: 1\n  by_consequence:\n    write: 1\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/transcription_jobs\n  method: post\n  operationId: submit-transcription-job-v-1-transcription-jobs-post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transcription_jobs/{job_id}\n  method: get\n  operationId:\
  \ get-transcription-job-v-1-transcription-jobs-job-id-get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kotoba/refs/heads/main/agentic-access/kotoba-agentic-access.yml
summary_line: 2 operations · 1 acting
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Voice
- Speech Recognition
- Speech to Text
- Text to Speech
- Translation
- Real Time
- WebSockets
- Audio
- Transcription
---
