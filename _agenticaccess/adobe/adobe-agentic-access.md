---
acting_count: 20
action_class_counts:
  acting: 20
  connected: 2
api_specs:
- filename: adobe-accessibility-auto-tag-api-openapi.yml
  format: yaml
  label: Adobe PDF Services Accessibility Auto-Tag API
  slug: adobe-accessibility-auto-tag-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/openapi/adobe-accessibility-auto-tag-api-openapi.yml
- filename: adobe-assets-api-openapi.yml
  format: yaml
  label: Adobe PDF Services Assets API
  slug: adobe-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/openapi/adobe-assets-api-openapi.yml
- filename: adobe-combine-pdf-api-openapi.yml
  format: yaml
  label: Adobe PDF Services Combine PDF API
  slug: adobe-combine-pdf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/openapi/adobe-combine-pdf-api-openapi.yml
- filename: adobe-compress-pdf-api-openapi.yml
  format: yaml
  label: Adobe PDF Services Compress PDF API
  slug: adobe-compress-pdf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/openapi/adobe-compress-pdf-api-openapi.yml
- filename: adobe-create-pdf-api-openapi.yml
  format: yaml
  label: Adobe PDF Services Create PDF API
  slug: adobe-create-pdf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/openapi/adobe-create-pdf-api-openapi.yml
- filename: adobe-delete-pages-api-openapi.yml
  format: yaml
  label: Adobe PDF Services Delete Pages API
  slug: adobe-delete-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/openapi/adobe-delete-pages-api-openapi.yml
- filename: adobe-document-generation-api-openapi.yml
  format: yaml
  label: Adobe PDF Services Document Generation API
  slug: adobe-document-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/openapi/adobe-document-generation-api-openapi.yml
- filename: adobe-export-pdf-api-openapi.yml
  format: yaml
  label: Adobe PDF Services Export PDF API
  slug: adobe-export-pdf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/openapi/adobe-export-pdf-api-openapi.yml
- filename: adobe-extract-pdf-api-openapi.yml
  format: yaml
  label: Adobe PDF Services Extract PDF API
  slug: adobe-extract-pdf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/openapi/adobe-extract-pdf-api-openapi.yml
- filename: adobe-insert-pages-api-openapi.yml
  format: yaml
  label: Adobe PDF Services Insert Pages API
  slug: adobe-insert-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/openapi/adobe-insert-pages-api-openapi.yml
- filename: adobe-jobs-api-openapi.yml
  format: yaml
  label: Adobe PDF Services Jobs API
  slug: adobe-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/openapi/adobe-jobs-api-openapi.yml
- filename: adobe-linearize-pdf-api-openapi.yml
  format: yaml
  label: Adobe PDF Services Linearize PDF API
  slug: adobe-linearize-pdf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/openapi/adobe-linearize-pdf-api-openapi.yml
- filename: adobe-ocr-api-openapi.yml
  format: yaml
  label: Adobe PDF Services OCR API
  slug: adobe-ocr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/openapi/adobe-ocr-api-openapi.yml
- filename: adobe-pdf-properties-api-openapi.yml
  format: yaml
  label: Adobe PDF Services PDF Properties API
  slug: adobe-pdf-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/openapi/adobe-pdf-properties-api-openapi.yml
- filename: adobe-protect-pdf-api-openapi.yml
  format: yaml
  label: Adobe PDF Services Protect PDF API
  slug: adobe-protect-pdf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/openapi/adobe-protect-pdf-api-openapi.yml
- filename: adobe-remove-protection-api-openapi.yml
  format: yaml
  label: Adobe PDF Services Remove Protection API
  slug: adobe-remove-protection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/openapi/adobe-remove-protection-api-openapi.yml
- filename: adobe-reorder-pages-api-openapi.yml
  format: yaml
  label: Adobe PDF Services Reorder Pages API
  slug: adobe-reorder-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/openapi/adobe-reorder-pages-api-openapi.yml
- filename: adobe-replace-pages-api-openapi.yml
  format: yaml
  label: Adobe PDF Services Replace Pages API
  slug: adobe-replace-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/openapi/adobe-replace-pages-api-openapi.yml
- filename: adobe-rotate-pages-api-openapi.yml
  format: yaml
  label: Adobe PDF Services Rotate Pages API
  slug: adobe-rotate-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/openapi/adobe-rotate-pages-api-openapi.yml
- filename: adobe-split-pdf-api-openapi.yml
  format: yaml
  label: Adobe PDF Services Split PDF API
  slug: adobe-split-pdf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/openapi/adobe-split-pdf-api-openapi.yml
consequence_counts:
  physical: 1
  read: 2
  write: 19
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Adobe Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /operation/reorderpages
operation_count: 22
overview: 'Adobe exposes 22 API operations that an AI agent could call, of which 20 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read, 19 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Adobe
provider_slug: adobe
slug: adobe-agentic-access
source_filename: adobe-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/adobe-pdf-services-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    acting: 20\n    connected: 2\n  by_consequence:\n    write: 19\n    read: 2\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /assets\n  method: post\n  operationId: uploadAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/{assetID}\n  method: get\n  operationId: getAsset\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/{assetID}\n  method: delete\n  operationId: deleteAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operation/createpdf\n  method: post\n  operationId: createPDF\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operation/exportpdf\n  method: post\n  operationId: exportPDF\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operation/combinepdf\n  method: post\n  operationId: combinePDF\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operation/splitpdf\n  method: post\n  operationId: splitPDF\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operation/ocr\n  method: post\n  operationId: ocrPDF\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operation/compresspdf\n  method: post\n  operationId: compressPDF\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operation/protectpdf\n  method: post\n  operationId: protectPDF\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operation/removeprotection\n  method: post\n  operationId: removeProtection\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operation/linearizepdf\n  method: post\n  operationId: linearizePDF\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operation/extractpdf\n  method: post\n  operationId: extractPDF\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operation/accessibilitychecker\n  method: post\n\
  \  operationId: autoTagPDF\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operation/documentgeneration\n  method: post\n  operationId: generateDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operation/pdfproperties\n  method: post\n  operationId: getPDFProperties\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /operation/reorderpages\n  method: post\n  operationId: reorderPages\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operation/deletepages\n  method: post\n  operationId: deletePages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operation/rotatepages\n  method: post\n  operationId: rotatePages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operation/insertpages\n  method: post\n  operationId: insertPages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operation/replacepages\n  method: post\n  operationId: replacePages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operation/{operationType}/status/{jobID}\n  method: get\n  operationId: getJobStatus\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/agentic-access/adobe-agentic-access.yml
summary_line: 22 operations · 20 acting
tags:
- Fortune 1000
- Analytics
- Creative Cloud
- Digital Asset Management
- Document Services
- E-Commerce
- E-Signatures
- Experience Cloud
- Generative AI
- Marketing
- PDF
- Work Management
---
