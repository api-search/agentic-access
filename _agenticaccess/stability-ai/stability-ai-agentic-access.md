---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 2
api_specs:
- filename: stability-ai-3d-generation-api-openapi.yml
  format: yaml
  label: Stability AI 3D Generation API
  slug: stability-ai-3d-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stability-ai/refs/heads/main/openapi/stability-ai-3d-generation-api-openapi.yml
- filename: stability-ai-conservative-upscale-api-openapi.yml
  format: yaml
  label: Stability AI Conservative Upscale API
  slug: stability-ai-conservative-upscale-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stability-ai/refs/heads/main/openapi/stability-ai-conservative-upscale-api-openapi.yml
- filename: stability-ai-creative-upscale-api-openapi.yml
  format: yaml
  label: Stability AI Creative Upscale API
  slug: stability-ai-creative-upscale-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stability-ai/refs/heads/main/openapi/stability-ai-creative-upscale-api-openapi.yml
- filename: stability-ai-erase-api-openapi.yml
  format: yaml
  label: Stability AI Erase API
  slug: stability-ai-erase-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stability-ai/refs/heads/main/openapi/stability-ai-erase-api-openapi.yml
- filename: stability-ai-fast-upscale-api-openapi.yml
  format: yaml
  label: Stability AI Fast Upscale API
  slug: stability-ai-fast-upscale-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stability-ai/refs/heads/main/openapi/stability-ai-fast-upscale-api-openapi.yml
- filename: stability-ai-generate-core-api-openapi.yml
  format: yaml
  label: Stability AI Generate Core API
  slug: stability-ai-generate-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stability-ai/refs/heads/main/openapi/stability-ai-generate-core-api-openapi.yml
- filename: stability-ai-generate-sd3-api-openapi.yml
  format: yaml
  label: Stability AI Generate SD3 API
  slug: stability-ai-generate-sd3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stability-ai/refs/heads/main/openapi/stability-ai-generate-sd3-api-openapi.yml
- filename: stability-ai-generate-ultra-api-openapi.yml
  format: yaml
  label: Stability AI Generate Ultra API
  slug: stability-ai-generate-ultra-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stability-ai/refs/heads/main/openapi/stability-ai-generate-ultra-api-openapi.yml
- filename: stability-ai-image-to-video-api-openapi.yml
  format: yaml
  label: Stability AI Image to Video API
  slug: stability-ai-image-to-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stability-ai/refs/heads/main/openapi/stability-ai-image-to-video-api-openapi.yml
- filename: stability-ai-inpaint-api-openapi.yml
  format: yaml
  label: Stability AI Inpaint API
  slug: stability-ai-inpaint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stability-ai/refs/heads/main/openapi/stability-ai-inpaint-api-openapi.yml
- filename: stability-ai-outpaint-api-openapi.yml
  format: yaml
  label: Stability AI Outpaint API
  slug: stability-ai-outpaint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stability-ai/refs/heads/main/openapi/stability-ai-outpaint-api-openapi.yml
- filename: stability-ai-remove-background-api-openapi.yml
  format: yaml
  label: Stability AI Remove Background API
  slug: stability-ai-remove-background-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stability-ai/refs/heads/main/openapi/stability-ai-remove-background-api-openapi.yml
- filename: stability-ai-replace-background-and-relight-api-openapi.yml
  format: yaml
  label: Stability AI Replace Background and Relight API
  slug: stability-ai-replace-background-and-relight-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stability-ai/refs/heads/main/openapi/stability-ai-replace-background-and-relight-api-openapi.yml
- filename: stability-ai-search-and-recolor-api-openapi.yml
  format: yaml
  label: Stability AI Search and Recolor API
  slug: stability-ai-search-and-recolor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stability-ai/refs/heads/main/openapi/stability-ai-search-and-recolor-api-openapi.yml
- filename: stability-ai-search-and-replace-api-openapi.yml
  format: yaml
  label: Stability AI Search and Replace API
  slug: stability-ai-search-and-replace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stability-ai/refs/heads/main/openapi/stability-ai-search-and-replace-api-openapi.yml
- filename: stability-ai-sketch-api-openapi.yml
  format: yaml
  label: Stability AI Sketch API
  slug: stability-ai-sketch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stability-ai/refs/heads/main/openapi/stability-ai-sketch-api-openapi.yml
- filename: stability-ai-structure-api-openapi.yml
  format: yaml
  label: Stability AI Structure API
  slug: stability-ai-structure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stability-ai/refs/heads/main/openapi/stability-ai-structure-api-openapi.yml
- filename: stability-ai-style-api-openapi.yml
  format: yaml
  label: Stability AI Style API
  slug: stability-ai-style-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stability-ai/refs/heads/main/openapi/stability-ai-style-api-openapi.yml
consequence_counts:
  read: 2
  safety-critical: 3
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Stability Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2beta/stable-image/control/sketch
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2beta/stable-image/control/structure
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2beta/stable-image/control/style
operation_count: 20
overview: 'Stability AI exposes 20 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read, 15 write, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Stability AI
provider_slug: stability-ai
slug: stability-ai-agentic-access
source_filename: stability-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/stability-ai-stable-fast-3d-openapi.yml, openapi/stability-ai-stable-image-control-openapi.yml,\n  openapi/stability-ai-stable-image-edit-openapi.yml, openapi/stability-ai-stable-image-generate-openapi.yml,\n  openapi/stability-ai-stable-image-upscale-openapi.yml, openapi/stability-ai-stable-video-diffusion-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    acting: 18\n    connected: 2\n  by_consequence:\n    write: 15\n    safety-critical: 3\n    read: 2\n  human_in_the_loop_required: 3\noperations:\n- path: /v2beta/3d/stable-fast-3d\n  method: post\n  operationId: generateStableFast3D\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2beta/stable-image/control/sketch\n  method: post\n  operationId: controlImageSketch\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2beta/stable-image/control/structure\n  method: post\n  operationId: controlImageStructure\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /v2beta/stable-image/control/style\n  method: post\n  operationId: controlImageStyle\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2beta/stable-image/edit/inpaint\n  method: post\n  operationId: editImageInpaint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2beta/stable-image/edit/outpaint\n  method: post\n  operationId: editImageOutpaint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n \
  \   audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2beta/stable-image/edit/erase\n  method: post\n  operationId: editImageErase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2beta/stable-image/edit/search-and-replace\n  method: post\n  operationId: editImageSearchAndReplace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2beta/stable-image/edit/search-and-recolor\n  method:\
  \ post\n  operationId: editImageSearchAndRecolor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2beta/stable-image/edit/remove-background\n  method: post\n  operationId: editImageRemoveBackground\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2beta/stable-image/edit/replace-background-and-relight\n  method: post\n  operationId: editImageReplaceBackgroundAndRelight\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n   \
  \ escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2beta/stable-image/generate/ultra\n  method: post\n  operationId: generateImageUltra\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2beta/stable-image/generate/core\n  method: post\n  operationId: generateImageCore\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2beta/stable-image/generate/sd3\n  method: post\n  operationId: generateImageSD3\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2beta/stable-image/upscale/fast\n  method: post\n  operationId: upscaleImageFast\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2beta/stable-image/upscale/conservative\n  method: post\n  operationId: upscaleImageConservative\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /v2beta/stable-image/upscale/creative\n  method: post\n  operationId: upscaleImageCreative\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2beta/stable-image/upscale/creative/result/{id}\n  method: get\n  operationId: getUpscaleCreativeResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2beta/image-to-video\n  method: post\n  operationId: startImageToVideo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2beta/image-to-video/result/{id}\n\
  \  method: get\n  operationId: getImageToVideoResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stability-ai/refs/heads/main/agentic-access/stability-ai-agentic-access.yml
summary_line: 20 operations · 18 acting · 3 human-in-the-loop
tags:
- 3D Generation
- Artificial Intelligence
- Generative AI
- Image-Generation
- Image Editing
- Machine-Learning
- Stable Diffusion
- Text-to-Image
- Video Generation
---
