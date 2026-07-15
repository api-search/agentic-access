---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 1
api_specs:
- filename: vidu-ai-openapi.yml
  format: yaml
  label: Vidu Text-to-Video API
  slug: vidu-ai-text-to-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vidu-ai/refs/heads/main/openapi/vidu-ai-openapi.yml
- filename: vidu-ai-openapi.yml
  format: yaml
  label: Vidu Image-to-Video API
  slug: vidu-ai-image-to-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vidu-ai/refs/heads/main/openapi/vidu-ai-openapi.yml
- filename: vidu-ai-openapi.yml
  format: yaml
  label: Vidu Reference-to-Video API
  slug: vidu-ai-reference-to-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vidu-ai/refs/heads/main/openapi/vidu-ai-openapi.yml
- filename: vidu-ai-openapi.yml
  format: yaml
  label: Vidu Start-End Frame API
  slug: vidu-ai-start-end-frame-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vidu-ai/refs/heads/main/openapi/vidu-ai-openapi.yml
- filename: vidu-ai-openapi.yml
  format: yaml
  label: Vidu Upscale API
  slug: vidu-ai-upscale-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vidu-ai/refs/heads/main/openapi/vidu-ai-openapi.yml
- filename: vidu-ai-openapi.yml
  format: yaml
  label: Vidu Task Query API
  slug: vidu-ai-task-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vidu-ai/refs/heads/main/openapi/vidu-ai-openapi.yml
consequence_counts:
  read: 1
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Vidu Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Vidu exposes 6 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Vidu
provider_slug: vidu-ai
slug: vidu-ai-agentic-access
source_filename: vidu-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/vidu-ai-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    acting: 5\n    connected: 1\n  by_consequence:\n    write: 5\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /text2video\n  method: post\n  operationId: createText2Video\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /img2video\n  method: post\n  operationId: createImg2Video\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reference2video\n  method: post\n  operationId: createReference2Video\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /start-end2video\n  method: post\n  operationId: createStartEnd2Video\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /upscale\n  method: post\n  operationId: createUpscale\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/{id}/creations\n  method: get\n  operationId: getTaskCreations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vidu-ai/refs/heads/main/agentic-access/vidu-ai-agentic-access.yml
summary_line: 6 operations · 5 acting
tags:
- Video Generation
- AI Video
- Generative AI
- Text-to-Video
- Image-to-Video
- Reference-to-Video
- U-ViT
- Diffusion
---
