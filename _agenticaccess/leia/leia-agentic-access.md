---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 2
api_specs:
- filename: leia-media-transformation-api-openapi.yml
  format: yaml
  label: Leia Media Transformation API
  slug: leia-media-transformation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leia/refs/heads/main/openapi/leia-media-transformation-api-openapi.yml
- filename: leia-product-pricing-api-openapi.yml
  format: yaml
  label: Leia Product Pricing API
  slug: leia-product-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leia/refs/heads/main/openapi/leia-product-pricing-api-openapi.yml
- filename: leia-protocol-api-openapi.yml
  format: yaml
  label: Leia Protocol API
  slug: leia-protocol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leia/refs/heads/main/openapi/leia-protocol-api-openapi.yml
- filename: leia-storage-api-openapi.yml
  format: yaml
  label: Leia Storage API
  slug: leia-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leia/refs/heads/main/openapi/leia-storage-api-openapi.yml
consequence_counts:
  read: 2
  write: 10
description: Recommended x-agentic-access execution contracts for the Immersity Cloud API. Classified from the OpenAPI, then curated against the published metering and result-delivery model. A governance starting point — bind audience per deployment.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: searched
name: Leia Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Leia exposes 12 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 10 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Leia
provider_slug: leia
slug: leia-agentic-access
source_filename: leia-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: openapi/leia-immersity-authentication-openapi.yml, openapi/leia-immersity-cloud-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts for the Immersity Cloud API. Classified from the OpenAPI,\n  then curated against the published metering and result-delivery model. A governance starting point — bind audience\n  per deployment.\nsummary:\n  operations: 12\n  by_action_class:\n    acting: 10\n    connected: 2\n  by_consequence:\n    write: 10\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /protocol/openid-connect/token\n  method: post\n  operationId: get-access-token-1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/prices\n  method: get\n\
  \  operationId: ProductPricingController_getPrices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/disparity\n  method: post\n  operationId: TransactionController_estimateMonoDepth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - high-value\n      - abnormal\n    audit: required\n    note: credit-metered media transformation; writes to a caller-supplied presigned URL\n- path: /api/v1/animation\n  method: post\n  operationId: TransactionController_generateAnimation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - high-value\n\
  \      - abnormal\n    audit: required\n    note: credit-metered media transformation; writes to a caller-supplied presigned URL\n- path: /api/v1/transaction/callback\n  method: post\n  operationId: TransactionController_transactionCallback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - high-value\n      - abnormal\n    audit: required\n    note: credit-metered media transformation; writes to a caller-supplied presigned URL\n- path: /api/v1/sbs\n  method: post\n  operationId: TransactionController_generateStereoSbs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - high-value\n      - abnormal\n    audit: required\n    note: credit-metered\
  \ media transformation; writes to a caller-supplied presigned URL\n- path: /api/v1/topBottom\n  method: post\n  operationId: TransactionController_generateStereoTopBottom\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - high-value\n      - abnormal\n    audit: required\n    note: credit-metered media transformation; writes to a caller-supplied presigned URL\n- path: /api/v1/decode\n  method: post\n  operationId: TransactionController_decodeLif\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - high-value\n      - abnormal\n    audit: required\n    note: credit-metered media transformation; writes to a caller-supplied presigned URL\n- path:\
  \ /api/v1/encode\n  method: post\n  operationId: TransactionController_encodeLif\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - high-value\n      - abnormal\n    audit: required\n    note: credit-metered media transformation; writes to a caller-supplied presigned URL\n- path: /api/v1/video\n  method: post\n  operationId: TransactionController_generateVideoConversion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - high-value\n      - abnormal\n    audit: required\n    note: credit-metered media transformation; writes to a caller-supplied presigned URL\n- path: /api/v1/spatial\n  method: post\n  operationId: TransactionController_generateSpatialVideoConversion\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - high-value\n      - abnormal\n    audit: required\n    note: credit-metered media transformation; writes to a caller-supplied presigned URL\n- path: /api/v1/get-upload-url\n  method: get\n  operationId: StorageController_getStoragePresignedUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\ncuration: 'Curated correction of the heuristic pass. The mechanical classifier raised nine operations to consequence:\n  safety-critical because their NestJS-style operationIds contain the substring ''Controller'', which matched the\n  control/stop/dispatch keyword rule. Nothing in the Immersity Cloud API is physical or safety-critical: every write\n  is a media transformation that\
  \ spends prepaid credits and writes a file to a caller-supplied presigned URL. Those\n  nine are reclassified to consequence: write, with human-in-the-loop conditional on high-value spend, since the\n  real agent risk is credit consumption (each call is metered, 402 on empty balance) and writing to caller-controlled\n  storage.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leia/refs/heads/main/agentic-access/leia-agentic-access.yml
summary_line: 12 operations · 10 acting
tags:
- 3D
- Spatial Computing
- Computer-Vision
- depth-estimation
- Image Processing
- Video Processing
- Generative AI
- Displays
- Media Transformation
- Immersive Experiences
---
