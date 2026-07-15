---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 8
api_specs:
- filename: wellsaid-openapi.yml
  format: yaml
  label: WellSaid Text-to-Speech API
  slug: wellsaid-text-to-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellsaid/refs/heads/main/openapi/wellsaid-openapi.yml
- filename: wellsaid-openapi.yml
  format: yaml
  label: WellSaid Streaming TTS API
  slug: wellsaid-streaming-tts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellsaid/refs/heads/main/openapi/wellsaid-openapi.yml
- filename: wellsaid-openapi.yml
  format: yaml
  label: WellSaid Voices and Speakers API
  slug: wellsaid-voices-speakers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellsaid/refs/heads/main/openapi/wellsaid-openapi.yml
consequence_counts:
  read: 8
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Wellsaid Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'WellSaid Labs exposes 16 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: WellSaid Labs
provider_slug: wellsaid
slug: wellsaid-agentic-access
source_filename: wellsaid-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/wellsaid-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    acting: 8\n    connected: 8\n  by_consequence:\n    write: 8\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /tts/stream\n  method: post\n  operationId: streamTextToSpeech\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tts/clips\n  method: post\n  operationId: createClip\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tts/clips\n  method: get\n  operationId: listClips\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tts/clips/{clip-id}\n  method: get\n  operationId: getClip\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tts/clips/combine\n  method: post\n  operationId: combineClips\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tts/word-timing\n\
  \  method: post\n  operationId: renderWordTiming\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tts/avatars\n  method: get\n  operationId: getAvatars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tts/respelling-suggestions\n  method: get\n  operationId: getRespellingSuggestions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tts/replacement-libraries\n  method: get\n  operationId: listReplacementLibraries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n- path: /tts/replacement-libraries\n  method: post\n  operationId: createReplacementLibrary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tts/replacement-libraries/{library-id}\n  method: get\n  operationId: getReplacementLibrary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tts/replacement-libraries/{library-id}\n  method: delete\n  operationId: deleteReplacementLibrary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n \
  \   audit: required\n- path: /tts/replacement-libraries/{library-id}/replacements\n  method: get\n  operationId: listReplacements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tts/replacement-libraries/{library-id}/replacements\n  method: post\n  operationId: createReplacement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tts/replacement-libraries/{library-id}/replacements/{replacement-id}\n  method: get\n  operationId: getReplacement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tts/replacement-libraries/{library-id}/replacements/{replacement-id}\n\
  \  method: delete\n  operationId: deleteReplacement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wellsaid/refs/heads/main/agentic-access/wellsaid-agentic-access.yml
summary_line: 16 operations · 8 acting
tags:
- AI
- Text to Speech
- Voice
- Audio
- TTS
---
