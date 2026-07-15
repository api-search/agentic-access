---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 13
api_specs:
- filename: zuva-openapi.yml
  format: yaml
  label: Zuva Files API
  slug: files
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuva/refs/heads/main/openapi/zuva-openapi.yml
- filename: zuva-openapi.yml
  format: yaml
  label: Zuva Field Extraction API
  slug: field-extraction
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuva/refs/heads/main/openapi/zuva-openapi.yml
- filename: zuva-openapi.yml
  format: yaml
  label: Zuva Classification API
  slug: classification
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuva/refs/heads/main/openapi/zuva-openapi.yml
- filename: zuva-openapi.yml
  format: yaml
  label: Zuva Language API
  slug: language
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuva/refs/heads/main/openapi/zuva-openapi.yml
- filename: zuva-openapi.yml
  format: yaml
  label: Zuva OCR API
  slug: ocr
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuva/refs/heads/main/openapi/zuva-openapi.yml
- filename: zuva-openapi.yml
  format: yaml
  label: Zuva Fields Catalog API
  slug: fields-catalog
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zuva/refs/heads/main/openapi/zuva-openapi.yml
consequence_counts:
  read: 13
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Zuva Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 22
overview: 'Zuva exposes 22 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read and 9 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Zuva
provider_slug: zuva
slug: zuva-agentic-access
source_filename: zuva-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/zuva-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    acting: 9\n    connected: 13\n  by_consequence:\n    write: 9\n    read: 13\n  human_in_the_loop_required: 0\noperations:\n- path: /files\n  method: post\n  operationId: createFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files\n  method: delete\n  operationId: deleteFiles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files/{file_id}\n  method: delete\n  operationId: deleteFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files/{file_id}/expiration\n  method: put\n  operationId: updateFileExpiration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /extraction\n  method: post\n  operationId: createExtraction\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /extractions\n  method: get\n  operationId: getExtractions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /extraction/{request_id}\n  method: get\n  operationId: getExtraction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /extraction/{request_id}/results/text\n  method: get\n  operationId: getExtractionResultsText\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mlc\n  method: post\n  operationId: createClassification\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mlcs\n  method: get\n  operationId: getClassifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mlc/{request_id}\n  method: get\n  operationId: getClassification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ocr\n  method: post\n  operationId: createOcr\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /ocrs\n  method: get\n  operationId: getOcrs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ocr/{request_id}\n  method: get\n  operationId: getOcr\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ocr/{request_id}/text\n  method: get\n  operationId: getOcrText\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ocr/{request_id}/images\n  method: get\n  operationId: getOcrImages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ocr/{request_id}/images/{page_number}\n  method: get\n  operationId: getOcrImagePage\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ocr/{request_id}/layouts\n  method: get\n  operationId: getOcrLayouts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fields\n  method: get\n  operationId: getFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fields\n  method: post\n  operationId: createField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fields/{field_id}/metadata\n  method: get\n  operationId: getFieldMetadata\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fields/{field_id}/metadata\n  method: put\n  operationId: updateFieldMetadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zuva/refs/heads/main/agentic-access/zuva-agentic-access.yml
summary_line: 22 operations · 9 acting
tags:
- AI
- Document AI
- Contract Analysis
- Field Extraction
- Classification
- OCR
---
