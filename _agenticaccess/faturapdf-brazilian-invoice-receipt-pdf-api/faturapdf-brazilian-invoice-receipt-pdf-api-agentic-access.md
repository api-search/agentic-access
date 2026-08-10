---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 1
api_specs:
- filename: faturapdf-brazilian-invoice-receipt-pdf-api-documents-api-openapi.yml
  format: yaml
  label: FaturaPDF — Brazilian Invoice & Receipt PDF API Documents API
  slug: faturapdf-brazilian-invoice-receipt-pdf-api-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/faturapdf-brazilian-invoice-receipt-pdf-api/refs/heads/main/openapi/faturapdf-brazilian-invoice-receipt-pdf-api-documents-api-openapi.yml
consequence_counts:
  read: 1
  write: 2
description: Recommended x-agentic-access execution contracts for exposing this API to AI agents. A governance starting point, not a provider claim — review and bind `audience` per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Faturapdf Brazilian Invoice Receipt Pdf Api Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 3
overview: 'FaturaPDF — Brazilian Invoice & Receipt PDF API exposes 3 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: FaturaPDF — Brazilian Invoice & Receipt PDF API
provider_slug: faturapdf-brazilian-invoice-receipt-pdf-api
slug: faturapdf-brazilian-invoice-receipt-pdf-api-agentic-access
source_filename: faturapdf-brazilian-invoice-receipt-pdf-api-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: generated\nsource: openapi/faturapdf-brazilian-invoice-receipt-pdf-api-openapi-original.yml\ncurated: '2026-08-09'\ncuration_note: >-\n  The mechanical heuristic classified both POST operations as consequence \"physical\" because\n  their descriptions contain payment/invoice keywords. That is an over-classification here and\n  has been curated down to \"write\": no money moves, no order is placed, nothing is transmitted\n  to a bank, a PSP or a tax authority. The operations render a PDF from caller-supplied data and\n  return the bytes; nothing is stored server-side and there is no resource to reverse. Token TTL\n  is raised from 300s to the write ceiling of 900s and the token-exchange / purpose-required\n  requirements are dropped accordingly. Curated against the provider's own scope statements at\n  https://faturapdf.com/terms/ and https://faturapdf.com/guides/brazilian-fiscal-documents/.\ndescription: >-\n  Recommended x-agentic-access execution\
  \ contracts for exposing this API to AI agents. A\n  governance starting point, not a provider claim — review and bind `audience` per deployment.\n  See research/curity/agentic-governance/.\nsummary:\n  operations: 3\n  by_action_class:\n    acting: 2\n    connected: 1\n  by_consequence:\n    write: 2\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /invoice\n  method: post\n  operationId: generateInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n      exchange: false\n      purpose-required: false\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n  notes: >-\n    The output is a customer-facing financial document carrying real party names and tax IDs, so\n    audit the call even though the API itself is stateless. Two agent-specific hazards: the\n    success body is binary PDF (every\
  \ other status is JSON), and omitting `data` stamps the\n    current server date, which breaks reproducibility across a midnight UTC boundary.\n- path: /receipt\n  method: post\n  operationId: generateReceipt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n      exchange: false\n      purpose-required: false\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n  notes: >-\n    Same contract as generateInvoice with tipo forced to \"recibo\". A recibo asserts that money was\n    received — escalate to a human where the agent cannot verify that independently.\n- path: /health\n  method: get\n  operationId: healthCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n  notes: >-\n    The origin copy at https://faturapdf.com/health\
  \ is public, unauthenticated and unmetered —\n    prefer it for agent preflight so a liveness probe never spends document quota.\nout_of_scope_guardrail: >-\n  No operation in this API issues, cancels or registers a fiscal document. An agent must not\n  present the output as a Nota Fiscal Eletronica (NF-e/NFC-e/NFS-e), and must not claim a chave\n  de acesso, protocolo de autorizacao, DANFE or signed XML exists. If a task requires a real\n  nota fiscal, this API is the wrong tool and the agent should say so.\npersonal_data_note: >-\n  Request payloads carry real personal and company identifiers (CPF, CNPJ, names, addresses,\n  emails). The provider states payload contents are not logged and nothing is persisted, but the\n  agent side must still treat these as personal data under LGPD and must never use a real\n  document as an illustrative example — synthetic check-digit-valid values are published at\n  https://faturapdf.com/cpf-cnpj.html.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/faturapdf-brazilian-invoice-receipt-pdf-api/refs/heads/main/agentic-access/faturapdf-brazilian-invoice-receipt-pdf-api-agentic-access.yml
summary_line: 3 operations · 2 acting
tags:
- Invoices
- Receipts
- PDF Generation
- Documents
- Brazil
- Billing
- CPF Validation
- CNPJ Validation
- PIX
- Fintech
- Data Validation
---
