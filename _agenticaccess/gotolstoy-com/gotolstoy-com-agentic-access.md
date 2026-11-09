---
acting_count: 23
action_class_counts:
  acting: 23
  connected: 14
api_specs:
- filename: gotolstoy-com-ai-tools-api-openapi.yml
  format: yaml
  label: gotolstoy-com AI Tools API
  slug: gotolstoy-com-ai-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gotolstoy-com/openapi/gotolstoy-com-ai-tools-api-openapi.yml
- filename: gotolstoy-com-products-api-openapi.yml
  format: yaml
  label: gotolstoy-com Products API
  slug: gotolstoy-com-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gotolstoy-com/openapi/gotolstoy-com-products-api-openapi.yml
- filename: gotolstoy-com-stores-api-openapi.yml
  format: yaml
  label: gotolstoy-com Stores API
  slug: gotolstoy-com-stores-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gotolstoy-com/openapi/gotolstoy-com-stores-api-openapi.yml
- filename: gotolstoy-com-studio-api-openapi.yml
  format: yaml
  label: gotolstoy-com Studio API
  slug: gotolstoy-com-studio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gotolstoy-com/openapi/gotolstoy-com-studio-api-openapi.yml
- filename: gotolstoy-com-video-api-openapi.yml
  format: yaml
  label: gotolstoy-com Video API
  slug: gotolstoy-com-video-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gotolstoy-com/openapi/gotolstoy-com-video-api-openapi.yml
consequence_counts:
  read: 14
  safety-critical: 1
  write: 22
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Gotolstoy Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /ai-tools-service/motionControl
operation_count: 37
overview: 'gotolstoy-com exposes 37 API operations that an AI agent could call, of which 23 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read, 22 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: gotolstoy-com
provider_slug: gotolstoy-com
slug: gotolstoy-com-agentic-access
source_filename: gotolstoy-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/gotolstoy-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 37\n  by_action_class:\n    connected: 14\n    acting: 23\n  by_consequence:\n    read: 14\n    write: 22\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /products-service/getProduct\n  method: post\n  operationId: products_getProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - workspace\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products-service/getProductMedia\n  method: post\n  operationId: products_getProductMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    scope:\n    - workspace\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products-service/searchProductsCursor\n  method: post\n  operationId: products_searchProductsCursor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - workspace\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products-service/getProductsCount\n  method: post\n  operationId: products_getProductsCount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - workspace\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products-service/getProductCategoryBucketCounts\n  method: post\n  operationId: products_getProductCategoryBucketCounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - workspace\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products-service/getCollections\n\
  \  method: post\n  operationId: products_getCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - workspace\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products-service/getProductCollections\n  method: post\n  operationId: products_getProductCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - workspace\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products-service/getCollectionProducts\n  method: post\n  operationId: products_getCollectionProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - workspace\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account-service/listStores\n  method: post\n  operationId: stores_listStores\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n\
  \    - workspace\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /studio/getDraftStudioAssetCountsByProductIds\n  method: post\n  operationId: studio_getDraftStudioAssetCountsByProductIds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - workspace\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /studio/getStudioAssetComments\n  method: post\n  operationId: studio_getStudioAssetComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - workspace\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /studio/createStudioAssetComment\n  method: post\n  operationId: studio_createStudioAssetComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n  \
  \  - workspace\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /video-service/searchVodByIds\n  method: post\n  operationId: video_searchVodByIds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - workspace\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /video-service/searchVodAssetsByProductId\n  method: post\n  operationId: video_searchVodAssetsByProductId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - workspace\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /video-service/getVodLabels\n  method: post\n  operationId: video_getVodLabels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - workspace\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /video-service/listViews\n  method: post\n  operationId: video_listViews\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - workspace\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai-tools-service/textToImage\n  method: post\n  operationId: ai-tools_textToImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - workspace\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai-tools-service/editImage\n  method: post\n  operationId: ai-tools_editImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n \
  \   - workspace\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai-tools-service/animateImage\n  method: post\n  operationId: ai-tools_animateImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - workspace\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai-tools-service/textToVideo\n  method: post\n  operationId: ai-tools_textToVideo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - workspace\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /ai-tools-service/multiImage2Video\n  method: post\n  operationId: ai-tools_multiImage2Video\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - workspace\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai-tools-service/upscaleImage\n  method: post\n  operationId: ai-tools_upscaleImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - workspace\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai-tools-service/editCameraAngle\n  method: post\n  operationId: ai-tools_editCameraAngle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    scope:\n    - workspace\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai-tools-service/analyzeMedia\n  method: post\n  operationId: ai-tools_analyzeMedia\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - workspace\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai-tools-service/llm\n  method: post\n  operationId: ai-tools_llm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - workspace\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /ai-tools-service/tryon\n  method: post\n  operationId: ai-tools_tryon\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - workspace\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai-tools-service/googleBatch\n  method: post\n  operationId: ai-tools_googleBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - workspace\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai-tools-service/transcribeVideo\n  method: post\n  operationId: ai-tools_transcribeVideo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - workspace\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai-tools-service/textToSpeech\n  method: post\n  operationId: ai-tools_textToSpeech\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - workspace\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai-tools-service/listVoices\n  method: post\n  operationId: ai-tools_listVoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - workspace\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai-tools-service/generateMusic\n  method: post\n  operationId: ai-tools_generateMusic\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    scope:\n    - workspace\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai-tools-service/motionControl\n  method: post\n  operationId: ai-tools_motionControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - workspace\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /ai-tools-service/lipsync\n  method: post\n  operationId: ai-tools_lipsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - workspace\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n  \
  \    triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai-tools-service/removeBackground\n  method: post\n  operationId: ai-tools_removeBackground\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - workspace\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai-tools-service/generateSfx\n  method: post\n  operationId: ai-tools_generateSfx\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - workspace\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai-tools-service/getMultiTurnEditSession\n  method: post\n  operationId: ai-tools_getMultiTurnEditSession\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - workspace\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai-tools-service/getToolStatus\n  method: post\n  operationId: ai-tools_getToolStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - workspace\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/gotolstoy-com/agentic-access/gotolstoy-com-agentic-access.yml
summary_line: 37 operations · 23 acting · 1 human-in-the-loop
tags:
- Artificial Intelligence
- E-Commerce
- Platform
- Automation
- Marketing
---
