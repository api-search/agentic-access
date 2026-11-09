---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 5
api_specs:
- filename: api-video-videos-api-openapi.yml
  format: yaml
  label: API.Video Videos API
  slug: api-video-videos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-video/openapi/api-video-videos-api-openapi.yml
- filename: api-video-advanced-authentication-api-openapi.yml
  format: yaml
  label: API.Video Advanced authentication API
  slug: api-video-advanced-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-video/openapi/api-video-advanced-authentication-api-openapi.yml
- filename: api-video-analytics-api-openapi.yml
  format: yaml
  label: API.Video Analytics API
  slug: api-video-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-video/openapi/api-video-analytics-api-openapi.yml
- filename: api-video-captions-api-openapi.yml
  format: yaml
  label: API.Video Captions API
  slug: api-video-captions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-video/openapi/api-video-captions-api-openapi.yml
- filename: api-video-chapters-api-openapi.yml
  format: yaml
  label: API.Video Chapters API
  slug: api-video-chapters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-video/openapi/api-video-chapters-api-openapi.yml
- filename: api-video-live-streams-api-openapi.yml
  format: yaml
  label: API.Video Live Streams API
  slug: api-video-live-streams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-video/openapi/api-video-live-streams-api-openapi.yml
- filename: api-video-player-themes-api-openapi.yml
  format: yaml
  label: API.Video Player Themes API
  slug: api-video-player-themes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-video/openapi/api-video-player-themes-api-openapi.yml
- filename: api-video-summaries-api-openapi.yml
  format: yaml
  label: API.Video Summaries API
  slug: api-video-summaries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-video/openapi/api-video-summaries-api-openapi.yml
- filename: api-video-tags-api-openapi.yml
  format: yaml
  label: API.Video Tags API
  slug: api-video-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-video/openapi/api-video-tags-api-openapi.yml
- filename: api-video-upload-tokens-api-openapi.yml
  format: yaml
  label: API.Video Upload Tokens API
  slug: api-video-upload-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-video/openapi/api-video-upload-tokens-api-openapi.yml
- filename: api-video-watermarks-api-openapi.yml
  format: yaml
  label: API.Video Watermarks API
  slug: api-video-watermarks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-video/openapi/api-video-watermarks-api-openapi.yml
- filename: api-video-webhooks-api-openapi.yml
  format: yaml
  label: API.Video Webhooks API
  slug: api-video-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-video/openapi/api-video-webhooks-api-openapi.yml
consequence_counts:
  read: 5
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Api Video Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'API.Video exposes 13 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: API.Video
provider_slug: api-video
slug: api-video-agentic-access
source_filename: api-video-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/api-video-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 5\n    acting: 8\n  by_consequence:\n    read: 5\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /videos\n  method: get\n  operationId: listVideos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /videos\n  method: post\n  operationId: createVideo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n    \
  \  triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /videos/upload\n  method: post\n  operationId: uploadVideo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /videos/thumbnail\n  method: post\n  operationId: uploadThumbnail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /videos/thumbnail\n  method: patch\n  operationId: updateThumbnail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /videos/{id}\n  method: get\n  operationId: getVideo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /videos/{id}\n  method: delete\n  operationId: deleteVideo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /videos/{id}\n  method: patch\n  operationId: updateVideo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /videos/discarded\n  method: get\n  operationId: listDiscardedVideos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /videos/discarded/{id}\n  method: get\n  operationId: getDiscardedVideo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /videos/discarded/{id}\n  method: patch\n  operationId: updateDiscardedVideo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /videos/{id}/status\n  method: get\n  operationId: getVideoStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /videos/upload-token\n  method: post\n  operationId: createUploadToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/api-video/agentic-access/api-video-agentic-access.yml
summary_line: 13 operations · 8 acting
tags:
- Artificial Intelligence
- Analytics
- CDN
- Encoding
- Live Streaming
- Transcription
- Video
- Video-on-Demand
---
