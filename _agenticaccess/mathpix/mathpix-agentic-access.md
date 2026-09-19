---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 12
api_specs:
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
- filename: mathpix-batches-api-openapi.yml
  format: yaml
  label: Mathpix Batches API
  slug: mathpix-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mathpix/refs/heads/main/openapi/mathpix-batches-api-openapi.yml
- filename: mathpix-conversions-api-openapi.yml
  format: yaml
  label: Mathpix Conversions API
  slug: mathpix-conversions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mathpix/refs/heads/main/openapi/mathpix-conversions-api-openapi.yml
- filename: mathpix-images-api-openapi.yml
  format: yaml
  label: Mathpix Images API
  slug: mathpix-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mathpix/refs/heads/main/openapi/mathpix-images-api-openapi.yml
- filename: mathpix-usage-api-openapi.yml
  format: yaml
  label: Mathpix Usage API
  slug: mathpix-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mathpix/refs/heads/main/openapi/mathpix-usage-api-openapi.yml
- filename: mathpix-documents-api-openapi.yml
  format: yaml
  label: Mathpix Documents API
  slug: mathpix-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mathpix/refs/heads/main/openapi/mathpix-documents-api-openapi.yml
consequence_counts:
  read: 12
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Mathpix Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 19
overview: 'Mathpix exposes 19 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Mathpix
provider_slug: mathpix
slug: mathpix-agentic-access
source_filename: mathpix-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: generated\nsource: openapi/mathpix-app-tokens-api-openapi.yml, openapi/mathpix-batches-api-openapi.yml,\n  openapi/mathpix-conversions-api-openapi.yml, openapi/mathpix-documents-api-openapi.yml, openapi/mathpix-images-api-openapi.yml,\n  openapi/mathpix-strokes-api-openapi.yml, openapi/mathpix-usage-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    acting: 7\n    connected: 12\n  by_consequence:\n    write: 7\n    read: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /v3/app-tokens\n  method: post\n  operationId: createAppToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n    \
  \  max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/batch\n  method: post\n  operationId: submitBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/batch/{batch_id}\n  method: get\n  operationId: getBatchResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/converter\n  method: post\n  operationId: convertMarkdown\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v3/converter/{conversion_id}\n  method: get\n  operationId: getConversionStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/pdf\n  method: post\n  operationId: processDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/pdf/{pdf_id}\n  method: get\n  operationId: getDocumentStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/pdf/{pdf_id}\n  method: delete\n  operationId: deleteDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/pdf/{pdf_id}/stream\n  method: get\n  operationId: streamDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/pdf/{pdf_id}.mmd\n  method: get\n  operationId: downloadMmd\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/pdf/{pdf_id}.md\n  method: get\n  operationId: downloadMd\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/pdf/{pdf_id}.docx\n  method: get\n  operationId: downloadDocx\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/pdf/{pdf_id}.tex.zip\n  method: get\n  operationId: downloadTexZip\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/pdf/{pdf_id}.html\n  method: get\n  operationId: downloadHtml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/pdf/{pdf_id}.pptx\n  method: get\n  operationId: downloadPptx\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/pdf/{pdf_id}.lines.json\n  method: get\n  operationId: downloadLinesJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/text\n\
  \  method: post\n  operationId: processImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/strokes\n  method: post\n  operationId: processStrokes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/ocr-usage\n  method: get\n  operationId: queryOcrUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mathpix/refs/heads/main/agentic-access/mathpix-agentic-access.yml
summary_line: 19 operations · 7 acting
tags:
- OCR
- STEM
- Math
- Chemistry
- Document Conversion
- PDF
- LaTeX
- Handwriting
- Artificial Intelligence
- Machine-Learning
---
