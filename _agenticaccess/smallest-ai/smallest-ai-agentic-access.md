---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 2
api_specs:
- filename: smallest-ai-openapi.yml
  format: yaml
  label: Smallest AI Text-to-Speech (Waves)
  slug: text-to-speech-waves
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smallest-ai/refs/heads/main/openapi/smallest-ai-openapi.yml
- filename: smallest-ai-openapi.yml
  format: yaml
  label: Smallest AI Streaming / Realtime TTS
  slug: streaming-realtime-tts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smallest-ai/refs/heads/main/openapi/smallest-ai-openapi.yml
- filename: smallest-ai-openapi.yml
  format: yaml
  label: Smallest AI Voices / Cloning
  slug: voices-cloning
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smallest-ai/refs/heads/main/openapi/smallest-ai-openapi.yml
consequence_counts:
  read: 2
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Smallest Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Smallest AI exposes 6 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Smallest AI
provider_slug: smallest-ai
slug: smallest-ai-agentic-access
source_filename: smallest-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/smallest-ai-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    acting: 4\n    connected: 2\n  by_consequence:\n    write: 4\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /lightning/get_speech\n  method: post\n  operationId: getSpeech\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lightning-v2/get_speech/stream\n  method: post\n  operationId: streamSpeech\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lightning/get_voices\n  method: get\n  operationId: getVoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lightning/add_voice\n  method: post\n  operationId: addVoice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lightning/get_cloned_voices\n  method: get\n  operationId: getClonedVoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /lightning/delete_voice/{voiceId}\n  method: delete\n  operationId: deleteVoice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smallest-ai/refs/heads/main/agentic-access/smallest-ai-agentic-access.yml
summary_line: 6 operations · 4 acting
tags:
- AI
- Text to Speech
- Voice
- Realtime
- Voice Agents
---
