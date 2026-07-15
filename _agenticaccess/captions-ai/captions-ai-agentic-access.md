---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 6
api_specs:
- filename: add-captions-to-a-video
  format: yaml
  label: Captions Video Captions API
  slug: captions-ai-video-captions-api
  spec_type: OpenAPI
  url: https://captions.ai/help/api-reference/video-captions/add-captions-to-a-video
- filename: captions-ai-creator-ads-openapi.yml
  format: yaml
  label: Captions AI Creator API
  slug: captions-ai-creator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captions-ai/refs/heads/main/openapi/captions-ai-creator-ads-openapi.yml
- filename: captions-ai-creator-ads-openapi.yml
  format: yaml
  label: Captions AI Ads API
  slug: captions-ai-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captions-ai/refs/heads/main/openapi/captions-ai-creator-ads-openapi.yml
- filename: captions-ai-mirage-video-openapi.yml
  format: yaml
  label: Mirage Video Generation API
  slug: captions-mirage-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captions-ai/refs/heads/main/openapi/captions-ai-mirage-video-openapi.yml
consequence_counts:
  read: 6
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Captions Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'Captions exposes 15 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 9 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Captions
provider_slug: captions-ai
slug: captions-ai-agentic-access
source_filename: captions-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/captions-ai-creator-ads-openapi.yml, openapi/captions-ai-mirage-video-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    acting: 9\n    connected: 6\n  by_consequence:\n    write: 9\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /creator/list\n  method: post\n  operationId: listCreators\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /creator/submit\n  method: post\n  operationId: submitCreatorJob\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /creator/poll\n  method: post\n  operationId: pollCreatorJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ads/submit\n  method: post\n  operationId: submitAdsJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ads/poll\n  method: post\n\
  \  operationId: pollAdsJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos\n  method: post\n  operationId: createVideo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos\n  method: get\n  operationId: listVideos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/videos/{video_id}\n  method: get\n  operationId: getVideo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n \
  \   subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/videos/{video_id}/content\n  method: get\n  operationId: getVideoContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/videos/captions\n  method: post\n  operationId: addCaptions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos/captions/templates\n  method: get\n  operationId: listCaptionTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/videos/captions/templates/{template_id}\n  method: get\n  operationId: getCaptionTemplate\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/audio/text-to-speech/{voice_id}\n  method: post\n  operationId: generateSpeech\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/meta/text_overlays\n  method: post\n  operationId: createMetaTextOverlay\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/meta/text_overlays/{text_overlay_id}\n  method: get\n  operationId: getMetaTextOverlay\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/captions-ai/refs/heads/main/agentic-access/captions-ai-agentic-access.yml
summary_line: 15 operations · 9 acting
tags:
- AI Video
- Video Generation
- Video Captioning
- AI Dubbing
- Lip Sync
- AI Twin
- Text to Video
- Generative AI
- Video Translation
---
