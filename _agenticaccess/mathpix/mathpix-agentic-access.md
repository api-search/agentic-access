---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 3
api_specs:
- filename: mathpix-image-ocr-api-openapi.yml
  format: yaml
  label: Mathpix Image OCR API
  slug: mathpix-image-ocr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mathpix/refs/heads/main/openapi/mathpix-image-ocr-api-openapi.yml
- filename: mathpix-document-ocr-api-openapi.yml
  format: yaml
  label: Mathpix Document OCR API
  slug: mathpix-document-ocr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mathpix/refs/heads/main/openapi/mathpix-document-ocr-api-openapi.yml
- filename: mathpix-convert-api-openapi.yml
  format: yaml
  label: Mathpix Convert API
  slug: mathpix-convert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mathpix/refs/heads/main/openapi/mathpix-convert-api-openapi.yml
- filename: mathpix-batch-api-openapi.yml
  format: yaml
  label: Mathpix Batch API
  slug: mathpix-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mathpix/refs/heads/main/openapi/mathpix-batch-api-openapi.yml
- filename: mathpix-strokes-api-openapi.yml
  format: yaml
  label: Mathpix Strokes API
  slug: mathpix-strokes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mathpix/refs/heads/main/openapi/mathpix-strokes-api-openapi.yml
- filename: mathpix-app-tokens-api-openapi.yml
  format: yaml
  label: Mathpix App Tokens API
  slug: mathpix-app-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mathpix/refs/heads/main/openapi/mathpix-app-tokens-api-openapi.yml
- filename: mathpix-ocr-usage-api-openapi.yml
  format: yaml
  label: Mathpix OCR Usage API
  slug: mathpix-ocr-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mathpix/refs/heads/main/openapi/mathpix-ocr-usage-api-openapi.yml
consequence_counts:
  read: 3
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Mathpix Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Mathpix exposes 8 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Mathpix
provider_slug: mathpix
slug: mathpix-agentic-access
source_filename: mathpix-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/mathpix-app-tokens-api-openapi.yml, openapi/mathpix-batch-api-openapi.yml, openapi/mathpix-convert-api-openapi.yml,\n  openapi/mathpix-image-ocr-api-openapi.yml, openapi/mathpix-ocr-usage-api-openapi.yml, openapi/mathpix-strokes-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 5\n    connected: 3\n  by_consequence:\n    write: 5\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /v3/app-tokens\n  method: post\n  operationId: createAppToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/batch\n  method: post\n  operationId: submitBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/batch/{batch_id}\n  method: get\n  operationId: getBatchResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/converter\n  method: post\n  operationId: convertMarkdown\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v3/converter/{conversion_id}\n  method: get\n  operationId: getConversionStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/text\n  method: post\n  operationId: processImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/ocr-usage\n  method: get\n  operationId: queryOcrUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/strokes\n  method: post\n  operationId: processStrokes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mathpix/refs/heads/main/agentic-access/mathpix-agentic-access.yml
summary_line: 8 operations · 5 acting
tags:
- OCR
- STEM
- Math
- Chemistry
- Document Conversion
- PDF
- LaTeX
- Handwriting
- AI
- Machine Learning
---
