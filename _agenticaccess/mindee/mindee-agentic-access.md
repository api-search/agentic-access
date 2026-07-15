---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 7
api_specs:
- filename: mindee-extraction-api-openapi.yml
  format: yaml
  label: Mindee Extraction API
  slug: mindee-extraction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindee/refs/heads/main/openapi/mindee-extraction-api-openapi.yml
- filename: mindee-classification-api-openapi.yml
  format: yaml
  label: Mindee Classification API
  slug: mindee-classification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindee/refs/heads/main/openapi/mindee-classification-api-openapi.yml
- filename: mindee-crop-api-openapi.yml
  format: yaml
  label: Mindee Crop API
  slug: mindee-crop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindee/refs/heads/main/openapi/mindee-crop-api-openapi.yml
- filename: mindee-ocr-api-openapi.yml
  format: yaml
  label: Mindee OCR API
  slug: mindee-ocr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindee/refs/heads/main/openapi/mindee-ocr-api-openapi.yml
- filename: mindee-split-api-openapi.yml
  format: yaml
  label: Mindee Split API
  slug: mindee-split-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindee/refs/heads/main/openapi/mindee-split-api-openapi.yml
- filename: mindee-jobs-api-openapi.yml
  format: yaml
  label: Mindee Jobs API
  slug: mindee-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindee/refs/heads/main/openapi/mindee-jobs-api-openapi.yml
consequence_counts:
  physical: 6
  read: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Mindee Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/inferences/enqueue
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/products/classification/enqueue
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/products/crop/enqueue
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/products/extraction/enqueue
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/products/ocr/enqueue
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/products/split/enqueue
operation_count: 13
overview: 'Mindee exposes 13 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 6 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Mindee
provider_slug: mindee
slug: mindee-agentic-access
source_filename: mindee-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/mindee-classification-api-openapi.yml, openapi/mindee-crop-api-openapi.yml,\n  openapi/mindee-extraction-api-openapi.yml, openapi/mindee-jobs-api-openapi.yml, openapi/mindee-ocr-api-openapi.yml,\n  openapi/mindee-split-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    acting: 6\n    connected: 7\n  by_consequence:\n    physical: 6\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/products/classification/enqueue\n  method: post\n  operationId: Enqueue_Classification_Product_Inference_v2_products_classification_enqueue_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/products/classification/results/{inference_id}\n  method: get\n  operationId: Get_classification_Product_Result_v2_products_classification_results__inference_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/products/crop/enqueue\n  method: post\n  operationId: Enqueue_Crop_Product_Inference_v2_products_crop_enqueue_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v2/products/crop/results/{inference_id}\n  method: get\n  operationId: Get_Crop_Product_Result_v2_products_crop_results__inference_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/products/extraction/enqueue\n  method: post\n  operationId: Enqueue_Extraction_Product_Inference_v2_products_extraction_enqueue_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/inferences/enqueue\n  method: post\n  operationId: Enqueue_Extraction_Product_Inference_v2_inferences_enqueue_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n  \
  \  subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/products/extraction/results/{inference_id}\n  method: get\n  operationId: Get_Extraction_Product_Result_v2_products_extraction_results__inference_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/inferences/{inference_id}\n  method: get\n  operationId: Get_Extraction_Product_Result_v2_inferences__inference_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/jobs/{job_id}\n  method: get\n  operationId: Get_Job_Status_v2_jobs__job_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/products/ocr/enqueue\n  method: post\n  operationId: Enqueue_OCR_Product_Inference_v2_products_ocr_enqueue_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/products/ocr/results/{inference_id}\n  method: get\n  operationId: Get_OCR_Product_Result_v2_products_ocr_results__inference_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/products/split/enqueue\n  method: post\n  operationId: Enqueue_Split_Product_Inference_v2_products_split_enqueue_post\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/products/split/results/{inference_id}\n  method: get\n  operationId: Get_Split_Product_Result_v2_products_split_results__inference_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mindee/refs/heads/main/agentic-access/mindee-agentic-access.yml
summary_line: 13 operations · 6 acting
tags:
- Document Parsing
- OCR
- IDP
- AI
- Machine Learning
- Invoices
- Receipts
- IDs
- Computer Vision
---
