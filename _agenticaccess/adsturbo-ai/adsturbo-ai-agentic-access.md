---
acting_count: 29
action_class_counts:
  acting: 29
  connected: 5
api_specs:
- filename: adsturbo-ai-adclone-api-openapi.yml
  format: yaml
  label: AdsTurbo Ad Clone API
  slug: adsturbo-ai-adclone-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adsturbo-ai/openapi/adsturbo-ai-adclone-api-openapi.yml
- filename: adsturbo-ai-adclone-v2beta-api-openapi.yml
  format: yaml
  label: AdsTurbo AdClone (v2beta) API
  slug: adsturbo-ai-adclone-v2beta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adsturbo-ai/openapi/adsturbo-ai-adclone-v2beta-api-openapi.yml
- filename: adsturbo-ai-aiactor-api-openapi.yml
  format: yaml
  label: AdsTurbo AI Actor API
  slug: adsturbo-ai-aiactor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adsturbo-ai/openapi/adsturbo-ai-aiactor-api-openapi.yml
- filename: adsturbo-ai-image-api-openapi.yml
  format: yaml
  label: AdsTurbo Image API
  slug: adsturbo-ai-image-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adsturbo-ai/openapi/adsturbo-ai-image-api-openapi.yml
- filename: adsturbo-ai-image-v2beta-api-openapi.yml
  format: yaml
  label: AdsTurbo Image (v2beta) API
  slug: adsturbo-ai-image-v2beta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adsturbo-ai/openapi/adsturbo-ai-image-v2beta-api-openapi.yml
- filename: adsturbo-ai-persona-api-openapi.yml
  format: yaml
  label: AdsTurbo Persona API
  slug: adsturbo-ai-persona-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adsturbo-ai/openapi/adsturbo-ai-persona-api-openapi.yml
- filename: adsturbo-ai-video-api-openapi.yml
  format: yaml
  label: AdsTurbo Video API
  slug: adsturbo-ai-video-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adsturbo-ai/openapi/adsturbo-ai-video-api-openapi.yml
- filename: adsturbo-ai-video-v2beta-api-openapi.yml
  format: yaml
  label: AdsTurbo Video (v2beta) API
  slug: adsturbo-ai-video-v2beta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adsturbo-ai/openapi/adsturbo-ai-video-v2beta-api-openapi.yml
- filename: adsturbo-ai-work-api-openapi.yml
  format: yaml
  label: AdsTurbo Work API
  slug: adsturbo-ai-work-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adsturbo-ai/openapi/adsturbo-ai-work-api-openapi.yml
consequence_counts:
  read: 5
  safety-critical: 1
  write: 28
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Adsturbo Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /openapi/v1/video/motion-control
operation_count: 34
overview: 'AdsTurbo exposes 34 API operations that an AI agent could call, of which 29 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read, 28 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AdsTurbo
provider_slug: adsturbo-ai
slug: adsturbo-ai-agentic-access
source_filename: adsturbo-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/adsturbo-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 34\n  by_action_class:\n    acting: 29\n    connected: 5\n  by_consequence:\n    write: 28\n    read: 5\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /openapi/v1/img/create\n  method: post\n  operationId: saasImageCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/aiactor/list\n  method: post\n  operationId: openAiActorList\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/v1/aiactor/say\n  method: post\n  operationId: openAiActorSay\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/aiactor/perform\n  method: post\n  operationId: openAiActorPerform\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/persona/create\n  method: post\n  operationId: openPersonaCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/persona/delete\n  method: post\n  operationId: openPersonaDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/persona/list\n  method: post\n  operationId: openPersonalList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/v1/adclone/analyze\n  method: post\n  operationId: openAdCloneAnalyze\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/adclone/generate\n  method: post\n  operationId: openAdCloneGenerate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/video/generate\n  method: post\n  operationId: openVideoGenerate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/video/extend\n  method: post\n  operationId: openVideoExtend\n  x-agentic-access:\n  \
  \  action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/video/edit\n  method: post\n  operationId: openVideoEdit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/video/analyze\n  method: post\n  operationId: openVideoAnalyze\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/video/lipsync\n\
  \  method: post\n  operationId: openVideoLipSync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/video/inpaint\n  method: post\n  operationId: openVideoInpaint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/video/translate\n  method: post\n  operationId: openVideoTranslate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n     \
  \ - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/video/upscale\n  method: post\n  operationId: openVideoUpscale\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/video/character-swap\n  method: post\n  operationId: openVideoCharacterSwap\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/video/motion-control\n  method: post\n  operationId: openVideoMotionControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /openapi/v1/video/subtitle\n  method: post\n  operationId: openVideoSubtitle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/work/batch-status\n  method: post\n  operationId: openBatchGetWorkStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/work/status\n  method: post\n  operationId: openGetWorkStatus\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/v1/persona/status\n  method: post\n  operationId: openGetPersonaStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/v2beta/image/cutout\n  method: post\n  operationId: openImageCutout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v2beta/image/ecommerce\n  method: post\n  operationId: openImageEcommerce\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v2beta/image/enhance\n  method: post\n  operationId: openImageEnhance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v2beta/image/magic-eraser\n  method: post\n  operationId: openImageMagicEraser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v2beta/image/poster\n  method: post\n  operationId: openImagePoster\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v2beta/video/enhance\n  method: post\n  operationId: openVideoEnhanceV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v2beta/video/magic-eraser\n  method: post\n  operationId: openVideoMagicEraser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v2beta/adclone/create\n  method:\
  \ post\n  operationId: openAdCloneCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v2beta/adclone/get\n  method: post\n  operationId: openAdCloneGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/v2beta/adclone/preview\n  method: post\n  operationId: openAdClonePreview\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v2beta/adclone/submit\n  method: post\n  operationId: openAdCloneSubmit\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/adsturbo-ai/agentic-access/adsturbo-ai-agentic-access.yml
summary_line: 34 operations · 29 acting · 1 human-in-the-loop
tags:
- Artificial Intelligence
- Video Ads
- E-Commerce
- Marketing
- Automation
---
