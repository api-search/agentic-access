---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 11
api_specs:
- filename: trint-openapi.yml
  format: yaml
  label: Trint Upload and Transcribe API
  slug: trint-upload-transcribe-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trint/refs/heads/main/openapi/trint-openapi.yml
- filename: trint-openapi.yml
  format: yaml
  label: Trint Transcripts and Files API
  slug: trint-transcripts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trint/refs/heads/main/openapi/trint-openapi.yml
- filename: trint-openapi.yml
  format: yaml
  label: Trint Export API
  slug: trint-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trint/refs/heads/main/openapi/trint-openapi.yml
- filename: trint-openapi.yml
  format: yaml
  label: Trint Translations API
  slug: trint-translations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trint/refs/heads/main/openapi/trint-openapi.yml
- filename: trint-openapi.yml
  format: yaml
  label: Trint Realtime Transcription API
  slug: trint-realtime-transcription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trint/refs/heads/main/openapi/trint-openapi.yml
- filename: trint-openapi.yml
  format: yaml
  label: Trint Webhooks API
  slug: trint-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trint/refs/heads/main/openapi/trint-openapi.yml
consequence_counts:
  read: 11
  safety-critical: 1
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Trint Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /realtime/{id}/stop
operation_count: 20
overview: 'Trint exposes 20 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 8 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Trint
provider_slug: trint
slug: trint-agentic-access
source_filename: trint-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/trint-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    acting: 9\n    connected: 11\n  by_consequence:\n    write: 8\n    read: 11\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /upload\n  method: post\n  operationId: uploadAndTranscribe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ingest\n  method: post\n  operationId: ingestFromUrl\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ingest/status\n  method: get\n  operationId: getIngestStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transcripts/\n  method: get\n  operationId: listTranscripts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transcripts/{id}\n  method: get\n  operationId: getTranscript\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /folders\n  method: get\n  operationId: listFolders\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /folders\n  method: post\n  operationId: createFolder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shared-drives\n  method: get\n  operationId: listSharedDrives\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /export/{id}\n  method: get\n  operationId: exportTranscript\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /captions/{id}\n  method: get\n  operationId: getCaptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /translation-languages\n  method: get\n  operationId: listTranslationLanguages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /translations\n  method: post\n  operationId: createTranslation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /translations/{fileId}\n  method: get\n  operationId: getTranslations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /realtime/stream\n  method: post\n  operationId: createRealtimeStream\n  x-agentic-access:\n    action-class: acting\n  \
  \  consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /realtime/{id}/start\n  method: post\n  operationId: startRealtime\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /realtime/{id}/stop\n  method: post\n  operationId: stopRealtime\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /realtime/{id}/status\n\
  \  method: get\n  operationId: getRealtimeStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/register\n  method: post\n  operationId: registerWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{id}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook-events\n  method: get\n  operationId: listWebhookEvents\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trint/refs/heads/main/agentic-access/trint-agentic-access.yml
summary_line: 20 operations · 9 acting · 1 human-in-the-loop
tags:
- Audio Transcription
- Transcription
- Speech-to-Text
- Media
- Journalism
- AI
- Captions
---
