---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 8
api_specs:
- filename: ffmpeg-micro-com-blueprints-api-openapi.yml
  format: yaml
  label: ffmpeg-micro-com Blueprints API
  slug: ffmpeg-micro-com-blueprints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ffmpeg-micro-com/openapi/ffmpeg-micro-com-blueprints-api-openapi.yml
- filename: ffmpeg-micro-com-ffprobe-api-openapi.yml
  format: yaml
  label: ffmpeg-micro-com Ffprobe API
  slug: ffmpeg-micro-com-ffprobe-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ffmpeg-micro-com/openapi/ffmpeg-micro-com-ffprobe-api-openapi.yml
- filename: ffmpeg-micro-com-generate-api-openapi.yml
  format: yaml
  label: ffmpeg-micro-com Generate API
  slug: ffmpeg-micro-com-generate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ffmpeg-micro-com/openapi/ffmpeg-micro-com-generate-api-openapi.yml
- filename: ffmpeg-micro-com-transcodes-api-openapi.yml
  format: yaml
  label: ffmpeg-micro-com Transcodes API
  slug: ffmpeg-micro-com-transcodes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ffmpeg-micro-com/openapi/ffmpeg-micro-com-transcodes-api-openapi.yml
- filename: ffmpeg-micro-com-transcribe-api-openapi.yml
  format: yaml
  label: ffmpeg-micro-com Transcribe API
  slug: ffmpeg-micro-com-transcribe-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ffmpeg-micro-com/openapi/ffmpeg-micro-com-transcribe-api-openapi.yml
- filename: ffmpeg-micro-com-transcribes-api-openapi.yml
  format: yaml
  label: ffmpeg-micro-com Transcribes API
  slug: ffmpeg-micro-com-transcribes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ffmpeg-micro-com/openapi/ffmpeg-micro-com-transcribes-api-openapi.yml
- filename: ffmpeg-micro-com-upload-api-openapi.yml
  format: yaml
  label: ffmpeg-micro-com Upload API
  slug: ffmpeg-micro-com-upload-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ffmpeg-micro-com/openapi/ffmpeg-micro-com-upload-api-openapi.yml
consequence_counts:
  physical: 1
  read: 8
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ffmpeg Micro Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/generate/translate
operation_count: 21
overview: 'ffmpeg-micro-com exposes 21 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 12 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ffmpeg-micro-com
provider_slug: ffmpeg-micro-com
slug: ffmpeg-micro-com-agentic-access
source_filename: ffmpeg-micro-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/ffmpeg-micro-com-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    acting: 13\n    connected: 8\n  by_consequence:\n    write: 12\n    read: 8\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/upload/presigned-url\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/upload/confirm\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n  \
  \  subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ffprobe\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transcodes\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transcodes\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/transcodes/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transcodes/{id}/cancel\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transcodes/{id}/download\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transcribe\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n    \
  \  - abnormal\n      - high-value\n    audit: required\n- path: /v1/transcribe/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transcribe/{id}/download\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transcribes\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/blueprints/{slug}/runs\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/blueprints/runs/{id}\n  method:\
  \ get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/blueprints/runs/{id}/continue\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/generate/scenes\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/generate/translate\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/generate/image\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/generate/speech\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/generate/animate\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/generate/animate/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/ffmpeg-micro-com/agentic-access/ffmpeg-micro-com-agentic-access.yml
summary_line: 21 operations · 13 acting
tags:
- Video
- Automation
- FFmpeg
- Cloud
- Media Processing
---
