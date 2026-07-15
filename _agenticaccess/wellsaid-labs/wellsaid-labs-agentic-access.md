---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 8
api_specs:
- filename: wellsaid-labs-openapi.yml
  format: yaml
  label: WellSaid Labs Text-to-Speech API
  slug: wellsaid-labs-text-to-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellsaid-labs/refs/heads/main/openapi/wellsaid-labs-openapi.yml
- filename: wellsaid-labs-openapi.yml
  format: yaml
  label: WellSaid Labs Clips API
  slug: wellsaid-labs-clips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellsaid-labs/refs/heads/main/openapi/wellsaid-labs-openapi.yml
- filename: wellsaid-labs-openapi.yml
  format: yaml
  label: WellSaid Labs Voice Avatars API
  slug: wellsaid-labs-voice-avatars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellsaid-labs/refs/heads/main/openapi/wellsaid-labs-openapi.yml
- filename: wellsaid-labs-openapi.yml
  format: yaml
  label: WellSaid Labs Pronunciation API
  slug: wellsaid-labs-pronunciation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellsaid-labs/refs/heads/main/openapi/wellsaid-labs-openapi.yml
consequence_counts:
  read: 8
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Wellsaid Labs Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'WellSaid Labs exposes 16 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: WellSaid Labs
provider_slug: wellsaid-labs
slug: wellsaid-labs-agentic-access
source_filename: wellsaid-labs-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/wellsaid-labs-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    acting: 8\n    connected: 8\n  by_consequence:\n    write: 8\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /tts/stream\n  method: post\n  operationId: renderTtsStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /word-timing\n  method: post\n  operationId: renderWordTiming\n  x-agentic-access:\n    action-class: acting\n   \
  \ consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clips\n  method: get\n  operationId: listClips\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clips\n  method: post\n  operationId: createClip\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clips/{clip_id}\n  method: get\n  operationId: getClip\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clips/combine\n\
  \  method: post\n  operationId: combineClips\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /avatars\n  method: get\n  operationId: listAvatars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /replacement-libraries\n  method: get\n  operationId: listReplacementLibraries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /replacement-libraries\n  method: post\n  operationId: createReplacementLibrary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /replacement-libraries/{library_id}\n  method: get\n  operationId: getReplacementLibrary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /replacement-libraries/{library_id}\n  method: delete\n  operationId: deleteReplacementLibrary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /replacement-libraries/{library_id}/replacements\n  method: get\n  operationId: listReplacements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /replacement-libraries/{library_id}/replacements\n  method: post\n  operationId: createReplacement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /replacement-libraries/{library_id}/replacements/{replacement_id}\n  method: get\n  operationId: getReplacement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /replacement-libraries/{library_id}/replacements/{replacement_id}\n  method: delete\n  operationId: deleteReplacement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /respelling-suggestions\n  method: get\n  operationId: getRespellingSuggestions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wellsaid-labs/refs/heads/main/agentic-access/wellsaid-labs-agentic-access.yml
summary_line: 16 operations · 8 acting
tags:
- AI
- Text to Speech
- TTS
- Voice
- Voiceover
- Speech Synthesis
- Audio
---
