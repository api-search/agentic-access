---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 18
api_specs:
- filename: creatify-openapi.yml
  format: yaml
  label: Creatify AI Avatar API
  slug: creatify-ai-avatar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatify/refs/heads/main/openapi/creatify-openapi.yml
- filename: creatify-openapi.yml
  format: yaml
  label: Creatify Link-to-Video API
  slug: creatify-link-to-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatify/refs/heads/main/openapi/creatify-openapi.yml
- filename: creatify-openapi.yml
  format: yaml
  label: Creatify AI Shorts API
  slug: creatify-ai-shorts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatify/refs/heads/main/openapi/creatify-openapi.yml
- filename: creatify-openapi.yml
  format: yaml
  label: Creatify Custom Templates API
  slug: creatify-custom-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatify/refs/heads/main/openapi/creatify-openapi.yml
- filename: creatify-openapi.yml
  format: yaml
  label: Creatify Product-to-Video API
  slug: creatify-product-to-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatify/refs/heads/main/openapi/creatify-openapi.yml
- filename: creatify-openapi.yml
  format: yaml
  label: Creatify Text-to-Speech API
  slug: creatify-text-to-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatify/refs/heads/main/openapi/creatify-openapi.yml
- filename: creatify-openapi.yml
  format: yaml
  label: Creatify Personas API
  slug: creatify-personas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatify/refs/heads/main/openapi/creatify-openapi.yml
- filename: creatify-openapi.yml
  format: yaml
  label: Creatify Voices API
  slug: creatify-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatify/refs/heads/main/openapi/creatify-openapi.yml
- filename: creatify-openapi.yml
  format: yaml
  label: Creatify Music API
  slug: creatify-music-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatify/refs/heads/main/openapi/creatify-openapi.yml
- filename: creatify-openapi.yml
  format: yaml
  label: Creatify AI Editing API
  slug: creatify-ai-editing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatify/refs/heads/main/openapi/creatify-openapi.yml
consequence_counts:
  read: 18
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Creatify Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 31
overview: 'Creatify exposes 31 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read and 13 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Creatify
provider_slug: creatify
slug: creatify-agentic-access
source_filename: creatify-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/creatify-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 31\n  by_action_class:\n    acting: 13\n    connected: 18\n  by_consequence:\n    write: 13\n    read: 18\n  human_in_the_loop_required: 0\noperations:\n- path: /links/\n  method: post\n  operationId: createLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /link_to_videos/\n  method: get\n  operationId: listLinkToVideos\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /link_to_videos/\n  method: post\n  operationId: createLinkToVideo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /link_to_videos/{id}/\n  method: get\n  operationId: getLinkToVideo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /link_to_videos/{id}/render/\n  method: post\n  operationId: renderLinkToVideo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /lipsyncs/\n  method: post\n  operationId: createLipsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lipsyncs/preview/\n  method: post\n  operationId: previewLipsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lipsyncs/{id}/\n  method: get\n  operationId: getLipsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lipsyncs/{id}/render/\n  method: post\n  operationId: renderLipsync\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lipsyncs_v2/\n  method: post\n  operationId: createLipsyncV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lipsyncs_v2/{id}/\n  method: get\n  operationId: getLipsyncV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai_shorts/\n  method: post\n  operationId: createAiShort\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai_shorts/\n  method: get\n  operationId: listAiShorts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai_shorts/{id}/\n  method: get\n  operationId: getAiShort\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /custom_templates/\n  method: post\n  operationId: createCustomTemplateVideo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /custom_templates/{id}/\n\
  \  method: get\n  operationId: getCustomTemplateVideo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /product_to_video/\n  method: post\n  operationId: createProductToVideo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /product_to_video/{id}/\n  method: get\n  operationId: getProductToVideo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /text_to_speech/\n  method: post\n  operationId: createTextToSpeech\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /text_to_speech/{id}/\n  method: get\n  operationId: getTextToSpeech\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /personas/\n  method: get\n  operationId: listPersonas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /personas/paginated/\n  method: get\n  operationId: listPersonasPaginated\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /personas/{id}/\n  method: get\n  operationId: getPersona\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n- path: /voices/\n  method: get\n  operationId: listVoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /voices/paginated/\n  method: get\n  operationId: listVoicesPaginated\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /music_categories/\n  method: get\n  operationId: listMusicCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /musics/\n  method: get\n  operationId: listMusics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai_editing/\n  method: post\n  operationId: createAiEditing\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai_editing/{id}/\n  method: get\n  operationId: getAiEditing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inspiration_jobs/\n  method: get\n  operationId: listInspirationJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inspiration_jobs/\n  method: post\n  operationId: createInspirationJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/creatify/refs/heads/main/agentic-access/creatify-agentic-access.yml
summary_line: 31 operations · 13 acting
tags:
- AI Avatars
- Video Generation
- AI Video
- Generative AI
- Marketing Video
- Text to Speech
- UGC Ads
- AI Avatar
---
