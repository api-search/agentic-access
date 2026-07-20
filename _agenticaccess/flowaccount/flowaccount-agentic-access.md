---
acting_count: 104
action_class_counts:
  acting: 104
  connected: 49
api_specs:
- filename: flowaccount-openapi-original.json
  format: json
  label: FlowAccount Open API
  slug: flowaccount-open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowaccount/refs/heads/main/openapi/flowaccount-openapi-original.json
consequence_counts:
  physical: 48
  read: 49
  write: 56
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Flowaccount Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{culture}/billing-notes/{id}/payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{culture}/cash-invoices/batch-import-history
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{culture}/cash-invoices/custom-template
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /{culture}/cash-invoices/custom-template/{templateId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{culture}/cash-invoices/get-presign-for-upload-simpledoc
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{culture}/cash-invoices/inline-document
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /{culture}/cash-invoices/inline-document/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{culture}/cash-invoices/mark-viewed
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{culture}/cash-invoices/query-batch
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{culture}/cash-invoices/retry-simple-documents
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{culture}/cash-invoices/simple-document
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /{culture}/cash-invoices/simple-document/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{culture}/cash-invoices/{documentId}/status-key/{statusKey}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /{culture}/cash-invoices/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{culture}/cash-invoices/{id}/payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{culture}/credit-notes/{id}/payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{culture}/debit-notes/{id}/payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{culture}/expenses/{id}/payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{culture}/purchase-orders/inline-document
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /{culture}/purchase-orders/inline-document/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{culture}/purchase-orders/simple-document
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /{culture}/purchase-orders/simple-document/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{culture}/purchase-orders/{documentId}/status-key/{statusKey}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /{culture}/purchase-orders/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{culture}/purchase-orders/{id}/payments
operation_count: 153
overview: 'FlowAccount exposes 153 API operations that an AI agent could call, of which 104 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 49 read, 56 write, and 48 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: FlowAccount
provider_slug: flowaccount
slug: flowaccount-agentic-access
source_filename: flowaccount-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/flowaccount-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 153\n  by_action_class:\n    connected: 49\n    acting: 104\n  by_consequence:\n    read: 49\n    physical: 48\n    write: 56\n  human_in_the_loop_required: 0\noperations:\n- path: /{culture}/cash-invoices/batch-metadata\n  method: get\n  operationId: BatchImport_GenerateBacthIdMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/cash-invoices/batch-import-history\n  method: post\n  operationId: BatchImport_QueryBatchHistory\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/cash-invoices/query-batch\n  method: post\n  operationId: BatchImport_QueryBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/cash-invoices/retry-simple-documents\n  method: post\n  operationId: BatchImport_RetrySimpleDocuments\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n   \
  \   purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/cash-invoices/mark-viewed\n  method: post\n  operationId: BatchImport_MarkViewed\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/cash-invoices/get-presign-for-upload-simpledoc\n  method: post\n  operationId: BatchImport_GetPresign\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /{culture}/cash-invoices/get-batch-import-org-file/{batchId}\n  method: get\n  operationId: BatchImport_GetOrgingalFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/cash-invoices/get-batch-s3-data/{batchId}\n  method: get\n  operationId: BatchImport_GetBatchS3Data\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/cash-invoices/custom-template\n  method: post\n  operationId: BatchImport_UpsertCustomTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /{culture}/cash-invoices/custom-template/{templateId}\n  method: get\n  operationId: BatchImport_GetCustomTemplate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/cash-invoices/custom-template/{templateId}\n  method: delete\n  operationId: BatchImport_DeleteCustomTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/{culture}/contacts/search\n  method: get\n  operationId: Contact_Search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/{culture}/contacts\n\
  \  method: get\n  operationId: Contact_GetContactList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/{culture}/contacts\n  method: post\n  operationId: Contact_Create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/{culture}/contacts/{id}\n  method: get\n  operationId: Contact_GetContactList2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/{culture}/contacts/{id}\n  method: put\n  operationId: Contact_Update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/{culture}/contacts/{id}\n  method: delete\n  operationId: Contact_RemoveContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/{culture}/contacts/{contactId}/update-contact-qrcode\n  method: post\n  operationId: Contact_UploadContactQRCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/cash-invoices\n  method: get\n  operationId: CashInvoice_Index\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/cash-invoices/{id}\n  method: get\n  operationId: CashInvoice_Details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/cash-invoices/{id}\n  method: delete\n  operationId: CashInvoice_Delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/cash-invoices/simple-document\n  method: post\n  operationId: CashInvoice_Create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/cash-invoices/inline-document\n  method: post\n  operationId: CashInvoice_Create2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/cash-invoices/simple-document/{id}\n  method: put\n  operationId: CashInvoice_Edit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/cash-invoices/inline-document/{id}\n  method: put\n  operationId: CashInvoice_Edit2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/cash-invoices/{documentId}/status-key/{statusKey}\n  method: post\n  operationId: CashInvoice_ChangeStatusByKey\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/cash-invoices/{id}/payments\n\
  \  method: post\n  operationId: CashInvoice_ReceivePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/billing-notes\n  method: get\n  operationId: BillingNote_Index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/billing-notes/{id}\n  method: get\n  operationId: BillingNote_Details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/billing-notes/{id}\n  method: delete\n  operationId: BillingNote_Delete\n  x-agentic-access:\n    action-class: acting\n   \
  \ consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/billing-notes/simple-document\n  method: post\n  operationId: BillingNote_Create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/billing-notes/inline-document\n  method: post\n  operationId: BillingNote_Create2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/billing-notes/simple-document/{id}\n\
  \  method: put\n  operationId: BillingNote_Edit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/billing-notes/inline-document/{id}\n  method: put\n  operationId: BillingNote_Edit2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/billing-notes/{documentId}/status-key/{statusKey}\n  method: post\n  operationId: BillingNote_ChangeStatusByKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/billing-notes/{id}/payments\n  method: post\n  operationId: BillingNote_ReceivePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/quotations/{id}/partial-manual-payall\n  method: post\n  operationId: Quotation_CreatePartialManualPayall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/quotations/{id}/partial-manual-cancel\n\
  \  method: post\n  operationId: Quotation_PartialManualCancel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/quotations\n  method: get\n  operationId: Quotation_Index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/quotations/{id}\n  method: get\n  operationId: Quotation_Details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/quotations/{id}\n  method: delete\n  operationId: Quotation_Delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/quotations/simple-document\n  method: post\n  operationId: Quotation_Create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/quotations/inline-document\n  method: post\n  operationId: Quotation_Create2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/quotations/simple-document/{id}\n  method: put\n  operationId: Quotation_Edit\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/quotations/inline-document/{id}\n  method: put\n  operationId: Quotation_Edit2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/quotations/{documentId}/status-key/{statusKey}\n  method: post\n  operationId: Quotation_ChangeStatusByKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/quotations/{id}/payments\n  method: post\n  operationId: Quotation_ReceivePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/receipts/categories/business\n  method: get\n  operationId: Receipt_GetBusinessCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/receipts/categories/accounting\n  method: get\n  operationId: Receipt_GetChartOfAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /{culture}/receipts\n  method: get\n  operationId: Receipt_Index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/receipts/{id}\n  method: get\n  operationId: Receipt_Details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/receipts/{id}\n  method: delete\n  operationId: Receipt_Delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/receipts/simple-document\n  method: post\n  operationId: Receipt_Create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/receipts/inline-document\n  method: post\n  operationId: Receipt_Create2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/receipts/simple-document/{id}\n  method: put\n  operationId: Receipt_Edit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/receipts/inline-document/{id}\n  method: put\n  operationId: Receipt_Edit2\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/receipts/{documentId}/status-key/{statusKey}\n  method: post\n  operationId: Receipt_ChangeStatusByKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/receipts/{id}/payments\n  method: post\n  operationId: Receipt_ReceivePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n     \
  \ human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/receivable-invoices\n  method: get\n  operationId: ReceivableInvoice_Index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/receivable-invoices/{id}\n  method: get\n  operationId: ReceivableInvoice_Details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/receivable-invoices/{id}\n  method: delete\n  operationId: ReceivableInvoice_Delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n     \
  \ - high-value\n    audit: required\n- path: /{culture}/receivable-invoices/simple-document\n  method: post\n  operationId: ReceivableInvoice_Create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/receivable-invoices/inline-document\n  method: post\n  operationId: ReceivableInvoice_Create2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/receivable-invoices/simple-document/{id}\n  method: put\n\
  \  operationId: ReceivableInvoice_Edit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/receivable-invoices/inline-document/{id}\n  method: put\n  operationId: ReceivableInvoice_Edit2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/receivable-invoices/{documentId}/status-key/{statusKey}\n  method: post\n  operationId: ReceivableInvoice_ChangeStatusByKey\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/receivable-invoices/{id}/payments\n  method: post\n  operationId: ReceivableInvoice_ReceivePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/tax-invoices/cumulative-references\n  method: get\n  operationId: TaxInvoice_GetCumulativeDocumentReferenceList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /{culture}/tax-invoices\n  method: get\n  operationId: TaxInvoice_Index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/tax-invoices/{id}\n  method: get\n  operationId: TaxInvoice_Details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/tax-invoices/{id}\n  method: delete\n  operationId: TaxInvoice_Delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/tax-invoices/simple-document\n  method: post\n  operationId: TaxInvoice_Create\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/tax-invoices/inline-document\n  method: post\n  operationId: TaxInvoice_Create2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/tax-invoices/simple-document/{id}\n  method: put\n  operationId: TaxInvoice_Edit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n    \
  \  max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/tax-invoices/inline-document/{id}\n  method: put\n  operationId: TaxInvoice_Edit2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/tax-invoices/{documentId}/status-key/{statusKey}\n  method: post\n  operationId: TaxInvoice_ChangeStatusByKey\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/tax-invoices/{id}/payments\n  method: post\n  operationId: TaxInvoice_ReceivePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/credit-notes/cumulative-references\n  method: get\n  operationId: CreditNote_GetCumulativeDocumentReferenceList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/credit-notes\n  method: get\n  operationId: CreditNote_Index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n    \
  \  max-ttl: 3600\n    audit: none\n- path: /{culture}/credit-notes/{id}\n  method: get\n  operationId: CreditNote_Details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/credit-notes/{id}\n  method: delete\n  operationId: CreditNote_Delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/credit-notes/simple-document\n  method: post\n  operationId: CreditNote_Create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /{culture}/credit-notes/inline-document\n  method: post\n  operationId: CreditNote_Create2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/credit-notes/simple-document/{id}\n  method: put\n  operationId: CreditNote_Edit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/credit-notes/inline-document/{id}\n  method: put\n  operationId: CreditNote_Edit2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n    \
  \  max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/credit-notes/{documentId}/status-key/{statusKey}\n  method: post\n  operationId: CreditNote_ChangeStatusByKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/credit-notes/{id}/payments\n  method: post\n  operationId: CreditNote_ReceivePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /{culture}/debit-notes/cumulative-references\n  method: get\n  operationId: DebitNote_GetCumulativeDocumentReferenceList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/debit-notes\n  method: get\n  operationId: DebitNote_Index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/debit-notes/{id}\n  method: get\n  operationId: DebitNote_Details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/debit-notes/{id}\n  method: delete\n  operationId: DebitNote_Delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/debit-notes/simple-document\n  method: post\n  operationId: DebitNote_Create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/debit-notes/inline-document\n  method: post\n  operationId: DebitNote_Create2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{culture}/debit-notes/simple-document/{id}\n  method: put\n  operationId: DebitNote_Edit\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n\n# --- truncated at 32 KB (51 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/flowaccount/refs/heads/main/agentic-access/flowaccount-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flowaccount/refs/heads/main/agentic-access/flowaccount-agentic-access.yml
summary_line: 153 operations · 104 acting
tags:
- Company
- Accounting
- Invoicing
- Payroll
- Point of Sale
- SME
- Finance
- Tax
- Thailand
- Bookkeeping
---
