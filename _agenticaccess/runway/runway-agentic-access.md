---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 2
api_specs:
- filename: runway-avatars-api-openapi.yml
  format: yaml
  label: Runway Avatars API
  slug: runway-avatars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runway/refs/heads/main/openapi/runway-avatars-api-openapi.yml
- filename: runway-character-performance-api-openapi.yml
  format: yaml
  label: Runway Character Performance API
  slug: runway-character-performance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runway/refs/heads/main/openapi/runway-character-performance-api-openapi.yml
- filename: runway-documents-api-openapi.yml
  format: yaml
  label: Runway Documents API
  slug: runway-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runway/refs/heads/main/openapi/runway-documents-api-openapi.yml
- filename: runway-frame-interpolation-api-openapi.yml
  format: yaml
  label: Runway Frame Interpolation API
  slug: runway-frame-interpolation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runway/refs/heads/main/openapi/runway-frame-interpolation-api-openapi.yml
- filename: runway-image-to-video-api-openapi.yml
  format: yaml
  label: Runway Image to Video API
  slug: runway-image-to-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runway/refs/heads/main/openapi/runway-image-to-video-api-openapi.yml
- filename: runway-lip-sync-api-openapi.yml
  format: yaml
  label: Runway Lip Sync API
  slug: runway-lip-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runway/refs/heads/main/openapi/runway-lip-sync-api-openapi.yml
- filename: runway-realtime-sessions-api-openapi.yml
  format: yaml
  label: Runway Realtime Sessions API
  slug: runway-realtime-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runway/refs/heads/main/openapi/runway-realtime-sessions-api-openapi.yml
- filename: runway-sound-effects-api-openapi.yml
  format: yaml
  label: Runway Sound Effects API
  slug: runway-sound-effects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runway/refs/heads/main/openapi/runway-sound-effects-api-openapi.yml
- filename: runway-tasks-api-openapi.yml
  format: yaml
  label: Runway Tasks API
  slug: runway-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runway/refs/heads/main/openapi/runway-tasks-api-openapi.yml
- filename: runway-text-to-image-api-openapi.yml
  format: yaml
  label: Runway Text to Image API
  slug: runway-text-to-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runway/refs/heads/main/openapi/runway-text-to-image-api-openapi.yml
- filename: runway-text-to-video-api-openapi.yml
  format: yaml
  label: Runway Text to Video API
  slug: runway-text-to-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runway/refs/heads/main/openapi/runway-text-to-video-api-openapi.yml
- filename: runway-uploads-api-openapi.yml
  format: yaml
  label: Runway Uploads API
  slug: runway-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runway/refs/heads/main/openapi/runway-uploads-api-openapi.yml
- filename: runway-video-to-video-api-openapi.yml
  format: yaml
  label: Runway Video to Video API
  slug: runway-video-to-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runway/refs/heads/main/openapi/runway-video-to-video-api-openapi.yml
- filename: runway-video-upscale-api-openapi.yml
  format: yaml
  label: Runway Video Upscale API
  slug: runway-video-upscale-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runway/refs/heads/main/openapi/runway-video-upscale-api-openapi.yml
consequence_counts:
  read: 2
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Runway Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'Runway exposes 17 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 15 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Runway
provider_slug: runway
slug: runway-agentic-access
source_filename: runway-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/runway-characters-openapi.yml, openapi/runway-image-generation-openapi.yml,\n  openapi/runway-video-generation-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    acting: 15\n    connected: 2\n  by_consequence:\n    write: 15\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /avatars\n  method: post\n  operationId: createAvatar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /realtime_sessions\n\
  \  method: post\n  operationId: createRealtimeSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents\n  method: post\n  operationId: createDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{id}\n  method: delete\n  operationId: deleteDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /text_to_image\n  method: post\n  operationId: createTextToImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/{id}\n  method: get\n  operationId: getTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /image_to_video\n  method: post\n  operationId: createImageToVideo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /text_to_video\n  method: post\n  operationId: createTextToVideo\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /video_to_video\n  method: post\n  operationId: createVideoToVideo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /character_performance\n  method: post\n  operationId: createCharacterPerformance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /lip_sync\n  method: post\n  operationId: createLipSync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /video_upscale\n  method: post\n  operationId: createVideoUpscale\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /frame_interpolation\n  method: post\n  operationId: createFrameInterpolation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /sound_effect\n  method: post\n  operationId: createSoundEffect\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/{id}\n  method: get\n  operationId: getTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks/{id}\n  method: delete\n  operationId: deleteTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /uploads\n  method: post\n  operationId:\
  \ createUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/runway/refs/heads/main/agentic-access/runway-agentic-access.yml
summary_line: 17 operations · 15 acting
tags:
- Video Generation
- Image Generation
- Artificial Intelligence
- Machine Learning
- Generative AI
- Avatars
- Characters
- WebRTC
- Creative Tools
---
