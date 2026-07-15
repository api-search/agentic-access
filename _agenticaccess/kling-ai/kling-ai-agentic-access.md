---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 9
api_specs:
- filename: kling-ai-openapi.yml
  format: yaml
  label: Kling AI Text-to-Video API
  slug: kling-ai-text-to-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kling-ai/refs/heads/main/openapi/kling-ai-openapi.yml
- filename: kling-ai-openapi.yml
  format: yaml
  label: Kling AI Image-to-Video API
  slug: kling-ai-image-to-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kling-ai/refs/heads/main/openapi/kling-ai-openapi.yml
- filename: kling-ai-openapi.yml
  format: yaml
  label: Kling AI Multi-Image-to-Video API
  slug: kling-ai-multi-image-to-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kling-ai/refs/heads/main/openapi/kling-ai-openapi.yml
- filename: kling-ai-openapi.yml
  format: yaml
  label: Kling AI Video Extension API
  slug: kling-ai-video-extension-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kling-ai/refs/heads/main/openapi/kling-ai-openapi.yml
- filename: kling-ai-openapi.yml
  format: yaml
  label: Kling AI Lip-Sync API
  slug: kling-ai-lip-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kling-ai/refs/heads/main/openapi/kling-ai-openapi.yml
- filename: kling-ai-openapi.yml
  format: yaml
  label: Kling AI Video Effects API
  slug: kling-ai-video-effects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kling-ai/refs/heads/main/openapi/kling-ai-openapi.yml
- filename: kling-ai-openapi.yml
  format: yaml
  label: Kling AI Image Generation API
  slug: kling-ai-image-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kling-ai/refs/heads/main/openapi/kling-ai-openapi.yml
- filename: kling-ai-openapi.yml
  format: yaml
  label: Kling AI Virtual Try-On API
  slug: kling-ai-virtual-try-on-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kling-ai/refs/heads/main/openapi/kling-ai-openapi.yml
- filename: kling-ai-openapi.yml
  format: yaml
  label: Kling AI Account Resource API
  slug: kling-ai-account-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kling-ai/refs/heads/main/openapi/kling-ai-openapi.yml
consequence_counts:
  read: 9
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Kling Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'Kling AI exposes 17 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Kling AI
provider_slug: kling-ai
slug: kling-ai-agentic-access
source_filename: kling-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/kling-ai-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    acting: 8\n    connected: 9\n  by_consequence:\n    write: 8\n    read: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/videos/text2video\n  method: post\n  operationId: createTextToVideoTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos/text2video/{task_id}\n  method: get\n  operationId: getTextToVideoTask\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/videos/image2video\n  method: post\n  operationId: createImageToVideoTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos/image2video/{task_id}\n  method: get\n  operationId: getImageToVideoTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/videos/multi-image2video\n  method: post\n  operationId: createMultiImageToVideoTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos/multi-image2video/{task_id}\n  method: get\n  operationId: getMultiImageToVideoTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/videos/video-extend\n  method: post\n  operationId: createVideoExtendTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos/video-extend/{task_id}\n  method: get\n  operationId: getVideoExtendTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/videos/lip-sync\n  method: post\n  operationId:\
  \ createLipSyncTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos/lip-sync/{task_id}\n  method: get\n  operationId: getLipSyncTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/videos/effects\n  method: post\n  operationId: createVideoEffectsTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos/effects/{task_id}\n  method: get\n  operationId: getVideoEffectsTask\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/images/generations\n  method: post\n  operationId: createImageGenerationTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/images/generations/{task_id}\n  method: get\n  operationId: getImageGenerationTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/images/kolors-virtual-try-on\n  method: post\n  operationId: createVirtualTryOnTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n    \
  \  human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/images/kolors-virtual-try-on/{task_id}\n  method: get\n  operationId: getVirtualTryOnTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/costs\n  method: get\n  operationId: getAccountResourcePacks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kling-ai/refs/heads/main/agentic-access/kling-ai-agentic-access.yml
summary_line: 17 operations · 8 acting
tags:
- Video Generation
- AI Video
- Generative AI
- Text-to-Video
- Image-to-Video
- AI
- Generative Video
- Lip Sync
- Virtual Try-On
- Image Generation
---
