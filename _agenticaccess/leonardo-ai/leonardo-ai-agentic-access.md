---
acting_count: 32
action_class_counts:
  acting: 32
  connected: 21
api_specs:
- filename: leonardo-ai-image-generation-openapi.json
  format: json
  label: Leonardo.AI Image Generation API
  slug: leonardo-ai-image-generation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leonardo-ai/refs/heads/main/openapi/leonardo-ai-image-generation-openapi.json
- filename: leonardo-ai-video-generation-openapi.json
  format: json
  label: Leonardo.AI Video Generation API
  slug: leonardo-ai-video-generation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leonardo-ai/refs/heads/main/openapi/leonardo-ai-video-generation-openapi.json
- filename: leonardo-ai-variation-openapi.json
  format: json
  label: Leonardo.AI Variation and Upscale API
  slug: leonardo-ai-variation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leonardo-ai/refs/heads/main/openapi/leonardo-ai-variation-openapi.json
- filename: leonardo-ai-realtime-canvas-openapi.json
  format: json
  label: Leonardo.AI Realtime Canvas API
  slug: leonardo-ai-realtime-canvas
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leonardo-ai/refs/heads/main/openapi/leonardo-ai-realtime-canvas-openapi.json
- filename: leonardo-ai-models-openapi.json
  format: json
  label: Leonardo.AI Models API
  slug: leonardo-ai-models
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leonardo-ai/refs/heads/main/openapi/leonardo-ai-models-openapi.json
- filename: leonardo-ai-elements-openapi.json
  format: json
  label: Leonardo.AI Elements API
  slug: leonardo-ai-elements
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leonardo-ai/refs/heads/main/openapi/leonardo-ai-elements-openapi.json
- filename: leonardo-ai-datasets-openapi.json
  format: json
  label: Leonardo.AI Datasets API
  slug: leonardo-ai-datasets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leonardo-ai/refs/heads/main/openapi/leonardo-ai-datasets-openapi.json
- filename: leonardo-ai-init-images-openapi.json
  format: json
  label: Leonardo.AI Init Images API
  slug: leonardo-ai-init-images
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leonardo-ai/refs/heads/main/openapi/leonardo-ai-init-images-openapi.json
- filename: leonardo-ai-media-openapi.json
  format: json
  label: Leonardo.AI Media API
  slug: leonardo-ai-media
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leonardo-ai/refs/heads/main/openapi/leonardo-ai-media-openapi.json
- filename: leonardo-ai-3d-model-assets-openapi.json
  format: json
  label: Leonardo.AI 3D Model Assets API
  slug: leonardo-ai-3d-model-assets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leonardo-ai/refs/heads/main/openapi/leonardo-ai-3d-model-assets-openapi.json
- filename: leonardo-ai-blueprints-openapi.json
  format: json
  label: Leonardo.AI Blueprints API
  slug: leonardo-ai-blueprints
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leonardo-ai/refs/heads/main/openapi/leonardo-ai-blueprints-openapi.json
- filename: leonardo-ai-prompt-openapi.json
  format: json
  label: Leonardo.AI Prompt API
  slug: leonardo-ai-prompt
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leonardo-ai/refs/heads/main/openapi/leonardo-ai-prompt-openapi.json
- filename: leonardo-ai-pricing-calculator-openapi.json
  format: json
  label: Leonardo.AI Pricing Calculator API
  slug: leonardo-ai-pricing-calculator
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leonardo-ai/refs/heads/main/openapi/leonardo-ai-pricing-calculator-openapi.json
- filename: leonardo-ai-user-openapi.json
  format: json
  label: Leonardo.AI User API
  slug: leonardo-ai-user
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leonardo-ai/refs/heads/main/openapi/leonardo-ai-user-openapi.json
consequence_counts:
  read: 21
  write: 32
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Leonardo Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 53
overview: 'Leonardo.AI exposes 53 API operations that an AI agent could call, of which 32 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read and 32 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Leonardo.AI
provider_slug: leonardo-ai
slug: leonardo-ai-agentic-access
source_filename: leonardo-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/leonardo-ai-3d-model-assets-openapi.json, openapi/leonardo-ai-blueprints-openapi.json,\n  openapi/leonardo-ai-datasets-openapi.json, openapi/leonardo-ai-elements-openapi.json, openapi/leonardo-ai-image-generation-openapi.json,\n  openapi/leonardo-ai-init-images-openapi.json, openapi/leonardo-ai-media-openapi.json, openapi/leonardo-ai-models-openapi.json,\n  openapi/leonardo-ai-pricing-calculator-openapi.json, openapi/leonardo-ai-prompt-openapi.json,\n  openapi/leonardo-ai-realtime-canvas-openapi.json, openapi/leonardo-ai-user-openapi.json, openapi/leonardo-ai-variation-openapi.json,\n  openapi/leonardo-ai-video-generation-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations:\
  \ 53\n  by_action_class:\n    acting: 32\n    connected: 21\n  by_consequence:\n    write: 32\n    read: 21\n  human_in_the_loop_required: 0\noperations:\n- path: /models-3d/upload\n  method: post\n  operationId: uploadModelAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /models-3d/user/{userId}\n  method: get\n  operationId: get3DModelsByUserId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /models-3d/{id}\n  method: get\n  operationId: get3DModelById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /models-3d/{id}\n  method: delete\n\
  \  operationId: delete3DModelById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /blueprints\n  method: get\n  operationId: listBlueprints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /blueprints/{id}\n  method: get\n  operationId: getBlueprintById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /blueprints/{id}/versions\n  method: get\n  operationId: getBlueprintVersionsByBlueprintId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /blueprint-executions\n\
  \  method: post\n  operationId: executeBlueprint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /blueprint-executions/{id}\n  method: get\n  operationId: getBlueprintExecution\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /blueprint-executions/{id}/generations\n  method: get\n  operationId: getBlueprintExecutionGenerations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets\n  method: post\n  operationId: createDataset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets/{id}\n  method: get\n  operationId: getDatasetById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets/{id}\n  method: delete\n  operationId: deleteDatasetById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets/{datasetId}/upload\n  method: post\n  operationId: uploadDatasetImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets/{datasetId}/upload/gen\n  method: post\n  operationId: uploadDatasetImageFromGen\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /elements/{id}\n  method: get\n  operationId: getElementById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /elements/{id}\n  method: delete\n  operationId: deleteElementById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n   \
  \   - high-value\n    audit: required\n- path: /elements/user/{userId}\n  method: get\n  operationId: getCustomElementsByUserId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /elements\n  method: post\n  operationId: createElement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /elements\n  method: get\n  operationId: listElements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /generations\n  method: post\n  operationId: createGeneration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /generations/{id}\n  method: get\n  operationId: getGenerationById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /generations/{id}\n  method: delete\n  operationId: deleteGenerationById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /generations/user/{userId}\n  method: get\n  operationId: getGenerationsByUserId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /init-image\n\
  \  method: post\n  operationId: uploadInitImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /init-image/{id}\n  method: get\n  operationId: getInitImageById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /init-image/{id}\n  method: delete\n  operationId: deleteInitImageById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /canvas-init-image\n  method: post\n  operationId: uploadCanvasInitImage\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /media\n  method: post\n  operationId: uploadMedia\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /media/{id}\n  method: get\n  operationId: getUploadedMediaById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /media/{id}\n  method: delete\n  operationId: deleteUploadedMediaById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /models\n  method: post\n  operationId: createModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /models/{id}\n  method: get\n  operationId: getModelById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /models/{id}\n  method: delete\n  operationId: deleteModelById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n     \
  \ triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /models/user/{userId}\n  method: get\n  operationId: getCustomModelsByUserId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platformModels\n  method: get\n  operationId: listPlatformModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pricing-calculator\n  method: post\n  operationId: pricingCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /prompt/random\n  method: post\n  operationId: promptRandom\n  x-agentic-access:\n    action-class: acting\n  \
  \  consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /prompt/improve\n  method: post\n  operationId: promptImprove\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /generations-lcm\n  method: post\n  operationId: createLCMGeneration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lcm-instant-refine\n  method: post\n  operationId: performInstantRefine\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lcm-inpainting\n  method: post\n  operationId: performInpaintingLCM\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lcm-upscale\n  method: post\n  operationId: performAlchemyUpscaleLCM\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me\n\
  \  method: get\n  operationId: getUserSelf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /variations/unzoom\n  method: post\n  operationId: createVariationUnzoom\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /variations/upscale\n  method: post\n  operationId: createVariationUpscale\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /variations/nobg\n  method: post\n  operationId: createVariationNoBG\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /variations/universal-upscaler\n  method: post\n  operationId: CreateUniversalUpscalerJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /variations/{id}\n  method: get\n  operationId: getVariationById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /motion-variations/{id}\n  method: get\n  operationId: getMotionVariationById\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /generations-motion-svd\n  method: post\n  operationId: createSVDMotionGeneration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /generations-image-to-video\n  method: post\n  operationId: createImageToVideoGeneration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /generations-text-to-video\n  method: post\n  operationId: createTextToVideoGeneration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leonardo-ai/refs/heads/main/agentic-access/leonardo-ai-agentic-access.yml
summary_line: 53 operations · 32 acting
tags:
- AI
- Artificial Intelligence
- Image Generation
- Video Generation
- Generative AI
- Creative
- 3D
- Diffusion
- Canva
---
