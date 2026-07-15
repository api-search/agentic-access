---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 4
api_specs:
- filename: pika-text-to-video-openapi.yml
  format: yaml
  label: Pika Video API
  slug: pika-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pika/refs/heads/main/openapi/pika-text-to-video-openapi.yml
consequence_counts:
  read: 4
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Pika Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Pika exposes 8 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Pika
provider_slug: pika
slug: pika-agentic-access
source_filename: pika-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/pika-image-to-video-openapi.yml, openapi/pika-text-to-video-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 4\n    connected: 4\n  by_consequence:\n    write: 4\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /fal-ai/pika/v2.2/image-to-video\n  method: post\n  operationId: submitImageToVideoRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fal-ai/pika/v2.2/image-to-video/requests/{request_id}\n\
  \  method: get\n  operationId: getImageToVideoResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fal-ai/pika/v2.2/image-to-video/requests/{request_id}/status\n  method: get\n  operationId: getImageToVideoStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fal-ai/pika/v2.2/image-to-video/requests/{request_id}/cancel\n  method: put\n  operationId: cancelImageToVideoRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fal-ai/pika/v2.2/text-to-video\n  method: post\n  operationId: submitTextToVideoRequest\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fal-ai/pika/v2.2/text-to-video/requests/{request_id}\n  method: get\n  operationId: getTextToVideoResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fal-ai/pika/v2.2/text-to-video/requests/{request_id}/status\n  method: get\n  operationId: getTextToVideoStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fal-ai/pika/v2.2/text-to-video/requests/{request_id}/cancel\n  method: put\n  operationId: cancelTextToVideoRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pika/refs/heads/main/agentic-access/pika-agentic-access.yml
summary_line: 8 operations · 4 acting
tags:
- AI
- Video Generation
- Text-to-Video
- Image-to-Video
- Diffusion Models
- Generative AI
- Media
- Creative Tools
---
