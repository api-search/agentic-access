---
acting_count: 5
action_class_counts:
  acting: 5
api_specs:
- filename: podcastle-openapi.yml
  format: yaml
  label: Podcastle Text-to-Speech API
  slug: text-to-speech
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podcastle/refs/heads/main/openapi/podcastle-openapi.yml
- filename: podcastle-openapi.yml
  format: yaml
  label: Podcastle Voices API
  slug: voices
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podcastle/refs/heads/main/openapi/podcastle-openapi.yml
- filename: podcastle-openapi.yml
  format: yaml
  label: Podcastle Voice Cloning API
  slug: voice-cloning
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podcastle/refs/heads/main/openapi/podcastle-openapi.yml
consequence_counts:
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Podcastle Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Podcastle exposes 5 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Podcastle
provider_slug: podcastle
slug: podcastle-agentic-access
source_filename: podcastle-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/podcastle-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    acting: 5\n  by_consequence:\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /text_to_speech\n  method: post\n  operationId: createSpeech\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /text_to_speech/streaming\n  method: post\n  operationId: createSpeechStreaming\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /text_to_speech/with_timestamps\n  method: post\n  operationId: createSpeechWithTimestamps\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /voices\n  method: post\n  operationId: listVoices\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /voices/clone\n  method: post\n  operationId: cloneVoice\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/podcastle/refs/heads/main/agentic-access/podcastle-agentic-access.yml
summary_line: 5 operations · 5 acting
tags:
- AI
- Audio
- Text to Speech
- Voice Cloning
- Podcasting
---
