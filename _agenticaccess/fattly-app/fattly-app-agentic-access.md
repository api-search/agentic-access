---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 3
api_specs:
- filename: fattly-app-account-api-openapi.yml
  format: yaml
  label: Fattly AI Account API
  slug: fattly-app-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fattly-app/openapi/fattly-app-account-api-openapi.yml
- filename: fattly-app-ad-studio-api-openapi.yml
  format: yaml
  label: Fattly AI Ad Studio API
  slug: fattly-app-ad-studio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fattly-app/openapi/fattly-app-ad-studio-api-openapi.yml
- filename: fattly-app-audio-api-openapi.yml
  format: yaml
  label: Fattly AI Audio API
  slug: fattly-app-audio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fattly-app/openapi/fattly-app-audio-api-openapi.yml
- filename: fattly-app-images-api-openapi.yml
  format: yaml
  label: Fattly AI Images API
  slug: fattly-app-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fattly-app/openapi/fattly-app-images-api-openapi.yml
- filename: fattly-app-video-api-openapi.yml
  format: yaml
  label: Fattly AI Video API
  slug: fattly-app-video-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fattly-app/openapi/fattly-app-video-api-openapi.yml
consequence_counts:
  read: 3
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Fattly App Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'Fattly AI exposes 11 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Fattly AI
provider_slug: fattly-app
slug: fattly-app-agentic-access
source_filename: fattly-app-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: generated\nsource: openapi/fattly-app-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 3\n    acting: 8\n  by_consequence:\n    read: 3\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /api/credits\n  method: get\n  operationId: getCredits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/models\n  method: get\n  operationId: listModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/upload\n  method: post\n  operationId:\
  \ uploadImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/ugc/video\n  method: post\n  operationId: createAdVideo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/ugc\n  method: post\n  operationId: createAdImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/generate\n\
  \  method: post\n  operationId: generateImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/video/generate\n  method: post\n  operationId: generateVideo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/video/status\n  method: get\n  operationId: getJobStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/audio/generate\n  method: post\n  operationId: generateAudio\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/upscale\n  method: post\n  operationId: upscaleImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/remove-bg\n  method: post\n  operationId: removeBackground\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/fattly-app/agentic-access/fattly-app-agentic-access.yml
summary_line: 11 operations · 8 acting
tags:
- AI
- Image Generation
- Video Generation
- Marketing
- Content Creation
---
