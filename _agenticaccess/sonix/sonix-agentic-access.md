---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 11
api_specs:
- filename: sonix-openapi.yml
  format: yaml
  label: Sonix Media & Transcription API
  slug: sonix-media-transcription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonix/refs/heads/main/openapi/sonix-openapi.yml
- filename: sonix-openapi.yml
  format: yaml
  label: Sonix Transcripts API
  slug: sonix-transcripts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonix/refs/heads/main/openapi/sonix-openapi.yml
- filename: sonix-openapi.yml
  format: yaml
  label: Sonix Translations API
  slug: sonix-translations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonix/refs/heads/main/openapi/sonix-openapi.yml
- filename: sonix-openapi.yml
  format: yaml
  label: Sonix Exports & Subtitles API
  slug: sonix-exports-subtitles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonix/refs/heads/main/openapi/sonix-openapi.yml
- filename: sonix-openapi.yml
  format: yaml
  label: Sonix AI Analysis API
  slug: sonix-ai-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonix/refs/heads/main/openapi/sonix-openapi.yml
consequence_counts:
  read: 11
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sonix Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 22
overview: 'Sonix exposes 22 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 11 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Sonix
provider_slug: sonix
slug: sonix-agentic-access
source_filename: sonix-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/sonix-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 11\n    acting: 11\n  by_consequence:\n    read: 11\n    write: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /media\n  method: get\n  operationId: listMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /media\n  method: post\n  operationId: createMedia\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /media/{id}\n  method: get\n  operationId: getMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /media/{id}\n  method: put\n  operationId: updateMedia\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /media/{id}\n  method: delete\n  operationId: deleteMedia\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /media/{id}/media_exports\n  method: post\n\
  \  operationId: createMediaExport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /media_exports/{id}\n  method: get\n  operationId: getMediaExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /media/{id}/transcript\n  method: get\n  operationId: getTranscript\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /media/{id}/transcript\n  method: put\n  operationId: updateTranscript\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /media/{id}/transcript.srt\n  method: get\n  operationId: getTranscriptSrt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /media/{id}/transcript.vtt\n  method: get\n  operationId: getTranscriptVtt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /media/{id}/transcript.json\n  method: get\n  operationId: getTranscriptJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /media/{id}/transcript/split\n  method: put\n  operationId: splitTranscript\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /media/{id}/translations\n  method: post\n  operationId: createTranslation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /media/{id}/translations/{language}\n  method: get\n  operationId: getTranslation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /media/{id}/summarizations\n  method: post\n  operationId: createSummarization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /summarizations/{id}\n  method: get\n  operationId: getSummarization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /media/{id}/video_burn_ins\n  method: post\n  operationId: createVideoBurnIn\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /video_burn_ins/{id}\n  method: get\n  operationId: getVideoBurnIn\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /folders\n  method: get\n  operationId: listFolders\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /folders\n  method: post\n  operationId: createFolder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /folders/{id}\n  method: put\n  operationId: updateFolder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sonix/refs/heads/main/agentic-access/sonix-agentic-access.yml
summary_line: 22 operations · 11 acting
tags:
- Audio Transcription
- Transcription
- Speech-to-Text
- Subtitles
- Captions
- Translation
- AI
- Media
---
