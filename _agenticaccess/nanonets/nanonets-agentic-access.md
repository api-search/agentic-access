---
acting_count: 16
action_class_counts:
  acting: 16
  connected: 4
api_specs:
- filename: nanonets-ocr-api-openapi.yml
  format: yaml
  label: Nanonets OCR API
  slug: nanonets-ocr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nanonets/refs/heads/main/openapi/nanonets-ocr-api-openapi.yml
- filename: nanonets-image-classification-api-openapi.yml
  format: yaml
  label: Nanonets Image Classification API
  slug: nanonets-image-classification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nanonets/refs/heads/main/openapi/nanonets-image-classification-api-openapi.yml
- filename: nanonets-file-management-api-openapi.yml
  format: yaml
  label: Nanonets File Management API
  slug: nanonets-file-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nanonets/refs/heads/main/openapi/nanonets-file-management-api-openapi.yml
- filename: nanonets-external-integrations-api-openapi.yml
  format: yaml
  label: Nanonets External Integrations API
  slug: nanonets-external-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nanonets/refs/heads/main/openapi/nanonets-external-integrations-api-openapi.yml
consequence_counts:
  read: 4
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Nanonets Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 20
overview: 'Nanonets exposes 20 API operations that an AI agent could call, of which 16 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 16 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Nanonets
provider_slug: nanonets
slug: nanonets-agentic-access
source_filename: nanonets-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/nanonets-external-integrations-api-openapi.yml, openapi/nanonets-file-management-api-openapi.yml,\n  openapi/nanonets-image-classification-api-openapi.yml, openapi/nanonets-ocr-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    connected: 4\n    acting: 16\n  by_consequence:\n    read: 4\n    write: 16\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v2/externalIntegrations\n  method: get\n  operationId: getExternalIntegrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/externalIntegrations/{external_integration_id}/executequery\n\
  \  method: post\n  operationId: executeQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/ImageLevelInferences/Model/{model_id}/Verify/{request_file_id}\n  method: post\n  operationId: verifyFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/ImageLevelInferences/Model/{model_id}/UnVerify/{request_file_id}\n  method: post\n  operationId: unverifyFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n   \
  \ escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/team/members/model/{model_id}/assign/files\n  method: post\n  operationId: assignFiles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/Inferences/Model/{model_id}/ImageLevelInference\n  method: patch\n  operationId: updateFileFields\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/Inferences/Model/{model_id}/InferenceRequestFiles/{file_id}\n  method: delete\n  operationId:\
  \ deleteFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/Inferences/Model/{model_id}/ImageLevelInferences/retryallexports\n  method: post\n  operationId: retryAllExports\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ImageCategorization/LabelFile/\n  method: post\n  operationId: imageCategorizationLabelFilePost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ImageCategorization/LabelUrls/\n  method: post\n  operationId: imageCategorizationLabelUrlsPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /OCR/Model/{model_id}/LabelFile/\n  method: post\n  operationId: ocrModelLabelFileByModelIdPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /OCR/Model/{model_id}/LabelFile/Async/\n  method: post\n  operationId: ocrModelLabelFileAsyncByModelIdPost\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /OCR/Model/{model_id}/LabelUrls/\n  method: post\n  operationId: ocrModelLabelUrlsByModelIdPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /OCR/Model/{model_id}/LabelUrls/Async/\n  method: post\n  operationId: ocrModelLabelUrlsAsyncByModelIdPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /Inferences/Model/{model_id}/InferenceRequest/{request_file_id}\n  method: get\n  operationId: ocrModelGetPredictionFileByFileId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Inferences/Model/{model_id}/InferenceRequest/{request_file_id}/page/{page_id}\n  method: get\n  operationId: ocrModelGetPredictionFileByPageId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Inferences/Model/{model_id}/InferenceRequest/\n  method: get\n  operationId: ocrModelListPredictionFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /OCR/Model/{model_id}/UploadFile/\n  method: post\n  operationId: ocrModelUploadFileByModelIdPost\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /OCR/Model/{model_id}/UploadUrls/\n  method: post\n  operationId: ocrModelUploadUrlsByModelIdPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /OCR/Model/{model_id}/Train/\n  method: post\n  operationId: ocrModelTrainByModelIdPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nanonets/refs/heads/main/agentic-access/nanonets-agentic-access.yml
summary_line: 20 operations · 16 acting
tags:
- AI
- Artificial Intelligence
- OCR
- Document AI
- Intelligent Document Processing
- Data Extraction
- Workflow Automation
- Computer Vision
- No-Code
---
