---
acting_count: 21
action_class_counts:
  acting: 21
  connected: 12
api_specs:
- filename: cloudflare-stream-openapi.yml
  format: yaml
  label: Cloudflare Stream Videos API
  slug: cloudflare-stream-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudflare-stream/refs/heads/main/openapi/cloudflare-stream-openapi.yml
- filename: cloudflare-stream-openapi.yml
  format: yaml
  label: Cloudflare Stream Live Inputs API
  slug: cloudflare-stream-live-inputs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudflare-stream/refs/heads/main/openapi/cloudflare-stream-openapi.yml
- filename: cloudflare-stream-openapi.yml
  format: yaml
  label: Cloudflare Stream Captions API
  slug: cloudflare-stream-captions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudflare-stream/refs/heads/main/openapi/cloudflare-stream-openapi.yml
- filename: cloudflare-stream-openapi.yml
  format: yaml
  label: Cloudflare Stream Signed URLs API
  slug: cloudflare-stream-signed-urls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudflare-stream/refs/heads/main/openapi/cloudflare-stream-openapi.yml
- filename: cloudflare-stream-openapi.yml
  format: yaml
  label: Cloudflare Stream Webhooks API
  slug: cloudflare-stream-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudflare-stream/refs/heads/main/openapi/cloudflare-stream-openapi.yml
- filename: cloudflare-stream-openapi.yml
  format: yaml
  label: Cloudflare Stream Analytics API
  slug: cloudflare-stream-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudflare-stream/refs/heads/main/openapi/cloudflare-stream-openapi.yml
consequence_counts:
  read: 12
  write: 21
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cloudflare Stream Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 33
overview: 'Cloudflare Stream exposes 33 API operations that an AI agent could call, of which 21 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read and 21 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cloudflare Stream
provider_slug: cloudflare-stream
slug: cloudflare-stream-agentic-access
source_filename: cloudflare-stream-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/cloudflare-stream-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 33\n  by_action_class:\n    connected: 12\n    acting: 21\n  by_consequence:\n    read: 12\n    write: 21\n  human_in_the_loop_required: 0\noperations:\n- path: /accounts/{account_id}/stream\n  method: get\n  operationId: listVideos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/stream\n  method: post\n  operationId: uploadVideoTus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/stream/{identifier}\n  method: get\n  operationId: getVideoDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/stream/{identifier}\n  method: post\n  operationId: editVideo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/stream/{identifier}\n  method: delete\n  operationId: deleteVideo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/stream/direct_upload\n  method: post\n  operationId: createDirectUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/stream/copy\n  method: post\n  operationId: copyVideoFromUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/stream/clip\n  method: post\n  operationId: clipVideo\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/stream/storage-usage\n  method: get\n  operationId: getStorageUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/stream/{identifier}/audio\n  method: get\n  operationId: listAudioTracks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/stream/{identifier}/audio/copy\n  method: post\n  operationId: addAudioTrack\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/stream/live_inputs\n  method: get\n  operationId: listLiveInputs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/stream/live_inputs\n  method: post\n  operationId: createLiveInput\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/stream/live_inputs/{live_input_identifier}\n  method: get\n  operationId: getLiveInput\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /accounts/{account_id}/stream/live_inputs/{live_input_identifier}\n  method: put\n  operationId: updateLiveInput\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/stream/live_inputs/{live_input_identifier}\n  method: delete\n  operationId: deleteLiveInput\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/stream/live_inputs/{live_input_identifier}/outputs\n  method: get\n  operationId: listOutputs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/stream/live_inputs/{live_input_identifier}/outputs\n  method: post\n  operationId: createOutput\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/stream/live_inputs/{live_input_identifier}/outputs/{output_identifier}\n  method: put\n  operationId: updateOutput\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/stream/live_inputs/{live_input_identifier}/outputs/{output_identifier}\n\
  \  method: delete\n  operationId: deleteOutput\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/stream/{identifier}/captions\n  method: get\n  operationId: listCaptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/stream/{identifier}/captions/{language}\n  method: get\n  operationId: getCaption\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/stream/{identifier}/captions/{language}\n  method: put\n  operationId: uploadCaption\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/stream/{identifier}/captions/{language}\n  method: delete\n  operationId: deleteCaption\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/stream/{identifier}/captions/{language}/generate\n  method: post\n  operationId: generateCaption\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /accounts/{account_id}/stream/{identifier}/captions/{language}/vtt\n  method: get\n  operationId: getCaptionVtt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/stream/keys\n  method: get\n  operationId: listSigningKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/stream/keys\n  method: post\n  operationId: createSigningKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/stream/keys/{key_id}\n  method: delete\n  operationId: deleteSigningKey\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/stream/{identifier}/token\n  method: post\n  operationId: createSignedToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/stream/webhook\n  method: get\n  operationId: getWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/stream/webhook\n  method: put\n  operationId: createWebhook\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/stream/webhook\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudflare-stream/refs/heads/main/agentic-access/cloudflare-stream-agentic-access.yml
summary_line: 33 operations · 21 acting
tags:
- Video
- Streaming
- Live Streaming
- Media
- Video Hosting
- Cloudflare
---
