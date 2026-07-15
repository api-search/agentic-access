---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 6
api_specs:
- filename: docsumo-openapi.yml
  format: yaml
  label: Docsumo Documents & Extraction API
  slug: docsumo-documents-extraction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docsumo/refs/heads/main/openapi/docsumo-openapi.yml
- filename: docsumo-openapi.yml
  format: yaml
  label: Docsumo Document Types API
  slug: docsumo-document-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docsumo/refs/heads/main/openapi/docsumo-openapi.yml
- filename: docsumo-openapi.yml
  format: yaml
  label: Docsumo Review & Validation API
  slug: docsumo-review-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docsumo/refs/heads/main/openapi/docsumo-openapi.yml
consequence_counts:
  read: 6
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Docsumo Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'Docsumo exposes 10 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Docsumo
provider_slug: docsumo
slug: docsumo-agentic-access
source_filename: docsumo-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/docsumo-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    acting: 4\n    connected: 6\n  by_consequence:\n    write: 4\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /eevee/apikey/upload/\n  method: post\n  operationId: uploadDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /eevee/apikey/upload/custom/\n  method: post\n  operationId: uploadDocumentCustom\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /eevee/apikey/documents/\n  method: get\n  operationId: listDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /eevee/apikey/documents/summary/\n  method: get\n  operationId: documentsSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /eevee/apikey/documents/{doc_id}/detail/\n  method: get\n  operationId: getDocumentDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /eevee/apikey/documents/{doc_id}/\n  method: delete\n\
  \  operationId: deleteDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /eevee/apikey/documents/{doc_id}/review-url/\n  method: get\n  operationId: getReviewUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /eevee/apikey/documents/{doc_id}/review-status/\n  method: patch\n  operationId: updateReviewStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /eevee/apikey/user/document-types/\n  method: get\n \
  \ operationId: listDocumentTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /eevee/apikey/user/detail/\n  method: get\n  operationId: getUserDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docsumo/refs/heads/main/agentic-access/docsumo-agentic-access.yml
summary_line: 10 operations · 4 acting
tags:
- Document Processing
- IDP
- OCR
- Data Extraction
- AI
---
