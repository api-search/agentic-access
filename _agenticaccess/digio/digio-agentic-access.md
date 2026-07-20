---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 4
api_specs:
- filename: digio-openapi.yml
  format: yaml
  label: Digio eSign API
  slug: digio-esign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digio/refs/heads/main/openapi/digio-openapi.yml
- filename: digio-openapi.yml
  format: yaml
  label: Digio eMandate (eNACH) API
  slug: digio-emandate-enach-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digio/refs/heads/main/openapi/digio-openapi.yml
- filename: digio-openapi.yml
  format: yaml
  label: Digio KYC API
  slug: digio-kyc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digio/refs/heads/main/openapi/digio-openapi.yml
- filename: digio-openapi.yml
  format: yaml
  label: Digio Documents & eStamp API
  slug: digio-documents-estamp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digio/refs/heads/main/openapi/digio-openapi.yml
consequence_counts:
  read: 4
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents - review and bind audience per deployment. Digio operations act on regulated, legally-binding artifacts (signatures, mandates, KYC), so write/high-consequence operations default to human-in-the-loop. See research/curity/agentic-governance/.
human_in_the_loop: 4
kind: agentic-access
layout: agentic-access
method: generated
name: Digio Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'Digio exposes 10 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 6 write.


  4 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Digio
provider_slug: digio
slug: digio-agentic-access
source_filename: digio-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: generated\nsource: openapi/digio-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents - review and bind\n  audience per deployment. Digio operations act on regulated, legally-binding artifacts\n  (signatures, mandates, KYC), so write/high-consequence operations default to human-in-the-loop.\n  See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    acting: 6\n    connected: 4\n  by_consequence:\n    write: 6\n    read: 4\n  human_in_the_loop_required: 4\noperations:\n- path: /v2/client/document/upload\n  method: post\n  operationId: uploadDocumentForSign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      -\
  \ legally-binding\n      - high-value\n    audit: required\n- path: /v2/client/document/uploadpdf\n  method: post\n  operationId: uploadPdfForSign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - legally-binding\n      - high-value\n    audit: required\n- path: /v2/client/document/{document_id}\n  method: get\n  operationId: getDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/client/document/download/{document_id}\n  method: get\n  operationId: downloadSignedDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    token:\n      max-ttl: 900\n    audit: required\n- path: /v2/client/template/multi_templates/create_sign_request\n  method: post\n  operationId:\
  \ createSignRequestFromTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - legally-binding\n      - high-value\n    audit: required\n- path: /v3/client/mandate/create\n  method: post\n  operationId: createMandate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - financial\n      - legally-binding\n    audit: required\n- path: /v3/client/mandate/{mandate_id}\n  method: get\n  operationId: getMandate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/client/mandate/{mandate_id}/cancel\n  method: post\n  operationId: cancelMandate\n \
  \ x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - financial\n      - abnormal\n    audit: required\n- path: /client/kyc/v2/request/with_template\n  method: post\n  operationId: createKycRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - pii\n      - abnormal\n    audit: required\n- path: /client/kyc/v2/{request_id}/response\n  method: get\n  operationId: getKycResponse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    token:\n      max-ttl: 900\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/digio/refs/heads/main/agentic-access/digio-agentic-access.yml
summary_line: 10 operations · 6 acting · 4 human-in-the-loop
tags:
- eSign
- KYC
- eNACH
- eMandate
- Digital Signature
- India
- Fintech
- Identity Verification
---
