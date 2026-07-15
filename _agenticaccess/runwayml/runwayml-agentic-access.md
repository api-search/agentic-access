---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 2
api_specs:
- filename: runwayml-openapi.yml
  format: yaml
  label: Runway Image-to-Video API
  slug: runwayml-image-to-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runwayml/refs/heads/main/openapi/runwayml-openapi.yml
- filename: runwayml-openapi.yml
  format: yaml
  label: Runway Text-to-Image API
  slug: runwayml-text-to-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runwayml/refs/heads/main/openapi/runwayml-openapi.yml
- filename: runwayml-openapi.yml
  format: yaml
  label: Runway Video-to-Video API
  slug: runwayml-video-to-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runwayml/refs/heads/main/openapi/runwayml-openapi.yml
- filename: runwayml-openapi.yml
  format: yaml
  label: Runway Character Performance API
  slug: runwayml-character-performance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runwayml/refs/heads/main/openapi/runwayml-openapi.yml
- filename: runwayml-openapi.yml
  format: yaml
  label: Runway Text-to-Speech API
  slug: runwayml-text-to-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runwayml/refs/heads/main/openapi/runwayml-openapi.yml
- filename: runwayml-openapi.yml
  format: yaml
  label: Runway Video Upscale API
  slug: runwayml-video-upscale-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runwayml/refs/heads/main/openapi/runwayml-openapi.yml
- filename: runwayml-openapi.yml
  format: yaml
  label: Runway Tasks API
  slug: runwayml-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runwayml/refs/heads/main/openapi/runwayml-openapi.yml
- filename: runwayml-openapi.yml
  format: yaml
  label: Runway Organization API
  slug: runwayml-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runwayml/refs/heads/main/openapi/runwayml-openapi.yml
consequence_counts:
  read: 2
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Runwayml Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'Runway exposes 9 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Runway
provider_slug: runwayml
slug: runwayml-agentic-access
source_filename: runwayml-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/runwayml-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    acting: 7\n    connected: 2\n  by_consequence:\n    write: 7\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /image_to_video\n  method: post\n  operationId: imageToVideo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /text_to_image\n  method: post\n  operationId: textToImage\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /video_to_video\n  method: post\n  operationId: videoToVideo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /character_performance\n  method: post\n  operationId: characterPerformance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /text_to_speech\n  method: post\n  operationId: textToSpeech\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /video_upscale\n  method: post\n  operationId: videoUpscale\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/{id}\n  method: get\n  operationId: getTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks/{id}\n  method: delete\n  operationId: cancelTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization\n  method: get\n  operationId: getOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/runwayml/refs/heads/main/agentic-access/runwayml-agentic-access.yml
summary_line: 9 operations · 7 acting
tags:
- Video Generation
- AI Video
- Generative AI
- Text-to-Video
- Image-to-Video
- Text-to-Image
- Video-to-Video
---
