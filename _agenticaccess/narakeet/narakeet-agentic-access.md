---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 4
api_specs:
- filename: narakeet-openapi.yml
  format: yaml
  label: Narakeet Text to Speech API
  slug: narakeet-text-to-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/narakeet/refs/heads/main/openapi/narakeet-openapi.yml
- filename: narakeet-openapi.yml
  format: yaml
  label: Narakeet Markdown to Video API
  slug: narakeet-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/narakeet/refs/heads/main/openapi/narakeet-openapi.yml
- filename: narakeet-openapi.yml
  format: yaml
  label: Narakeet Voice Listing API
  slug: narakeet-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/narakeet/refs/heads/main/openapi/narakeet-openapi.yml
- filename: narakeet-openapi.yml
  format: yaml
  label: Narakeet Account Credits API
  slug: narakeet-account-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/narakeet/refs/heads/main/openapi/narakeet-openapi.yml
consequence_counts:
  read: 4
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Narakeet Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Narakeet exposes 6 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Narakeet
provider_slug: narakeet
slug: narakeet-agentic-access
source_filename: narakeet-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/narakeet-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    acting: 2\n    connected: 4\n  by_consequence:\n    write: 2\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /text-to-speech/{format}\n  method: post\n  operationId: buildTextToSpeech\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /video/upload-request/zip\n  method: get\n  operationId: createVideoUploadRequest\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /video/build\n  method: post\n  operationId: buildVideo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /voices\n  method: get\n  operationId: listVoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/credits\n  method: get\n  operationId: getAccountCredits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status\n  method: get\n  operationId: pollBuildStatus\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/narakeet/refs/heads/main/agentic-access/narakeet-agentic-access.yml
summary_line: 6 operations · 2 acting
tags:
- Text to Speech
- TTS
- Voice
- Audio
- Video
- AI
- Media Generation
---
