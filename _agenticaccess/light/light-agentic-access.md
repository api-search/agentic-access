---
acting_count: 120
action_class_counts:
  acting: 120
  connected: 63
api_specs:
- filename: light-openapi-original.json
  format: json
  label: Light API
  slug: light-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/light/refs/heads/main/openapi/light-openapi-original.json
consequence_counts:
  physical: 45
  read: 63
  safety-critical: 5
  write: 70
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 5
kind: agentic-access
layout: agentic-access
method: generated
name: Light Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/card-transactions/{transactionId}/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/contracts/{contractId}/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/contracts/{contractId}/terminate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/invoice-receivables/{invoiceReceivableId}/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/purchase-orders/{purchaseOrderId}/reset
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/credit-notes/create-from-invoice-payable/{invoicePayableId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/credit-notes/{creditNoteId}/invoice-payables/{invoicePayableId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/credit-notes/{creditNoteId}/invoice-payables/{invoicePayableId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/credit-notes/{creditNoteId}/invoice-payables/{invoicePayableId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/customer-credits/{customerCreditId}/invoice-receivables/{invoiceReceivableId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/customer-credits/{customerCreditId}/invoice-receivables/{invoiceReceivableId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/customer-credits/{customerCreditId}/invoice-receivables/{invoiceReceivableId}/link
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/customer-credits/{customerCreditId}/invoice-receivables/{invoiceReceivableId}/unlink
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/customer-credits/{customerCreditId}/post-and-send-email
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/customer-credits/{customerCreditId}/submit-einvoice
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/invoice-payables
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/invoice-payables/{invoicePayableId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/invoice-payables/{invoicePayableId}/approve
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/invoice-payables/{invoicePayableId}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/invoice-payables/{invoicePayableId}/custom-properties
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/invoice-payables/{invoicePayableId}/decline
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/invoice-payables/{invoicePayableId}/document/upload-url
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/invoice-payables/{invoicePayableId}/line-items
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/invoice-payables/{invoicePayableId}/line-items/{lineItemId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/invoice-payables/{invoicePayableId}/line-items/{lineItemId}
operation_count: 183
overview: 'Light exposes 183 API operations that an AI agent could call, of which 120 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 63 read, 70 write, 45 physical, and 5 safety-critical.


  5 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Light
provider_slug: light
slug: light-agentic-access
source_filename: light-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/light-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 183\n  by_action_class:\n    acting: 120\n    connected: 63\n  by_consequence:\n    write: 70\n    read: 63\n    safety-critical: 5\n    physical: 45\n  human_in_the_loop_required: 5\noperations:\n- path: /oauth/token\n  method: post\n  operationId: getOAuthToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/authorize\n  method: get\n  operationId: startOAuthAuthorizationFlow\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounting-documents/accounting-documents\n  method: get\n  operationId: listAccountingDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/attachments\n  method: get\n  operationId: getAttachments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/attachments\n  method: post\n  operationId: createAttachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/attachments/upload-url\n\
  \  method: post\n  operationId: createAttachmentUploadUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/attachments/{attachmentId}\n  method: delete\n  operationId: deleteAttachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/attachments/{attachmentId}/document\n  method: get\n  operationId: getAttachmentDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/attachments/{attachmentId}/document\n\
  \  method: options\n  operationId: getAttachmentDocumentOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/bank-accounts\n  method: get\n  operationId: getBankAccountsForCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/bank-accounts\n  method: post\n  operationId: createBankAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/bank-accounts/{bankAccountId}/bank-transactions\n  method: get\n  operationId: listBankTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/bank-accounts/{bankAccountId}/bank-transactions\n  method: post\n  operationId: createBankTransactions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/bank-accounts/{bankAccountId}/balance\n  method: get\n  operationId: getBankAccountBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/bank-accounts/{bankAccountId}/balance\n  method: put\n  operationId: upsertBankAccountBalance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/bank-accounts/{bankAccountId}/bank-transactions/{bankTransactionId}\n  method: get\n  operationId: getBankTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/bff/invoice-payables\n  method: get\n  operationId: listInvoicePayables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/card-balance-accounts/{accountId}/statement\n  method: get\n  operationId: generateCardBalanceAccountStatement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/card-balance-accounts/{accountId}\n  method: get\n  operationId: getCardBalanceAccount\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/card-balance-accounts\n  method: get\n  operationId: listCardBalanceAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/card-balance-accounts/{accountId}/total-spend\n  method: get\n  operationId: getCardBalanceAccountTotalSpend\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/card-customers/public-key\n  method: get\n  operationId: getPublicKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/card-transactions/batch-update\n  method: patch\n  operationId: batchUpdateCardTransactions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/card-transactions/{cardTransactionId}/receipt-upload-url\n  method: post\n  operationId: generateUploadUrlForCardTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/card-transactions/{cardTransactionId}\n  method: get\n  operationId: getCardTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/card-transactions/{transactionId}/receipt\n  method: get\n  operationId: getAttachedCardTransactionReceiptDocument\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/card-transactions/{transactionId}/receipt\n  method: delete\n  operationId: removeReceipt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/card-transactions/{transactionId}/receipt\n  method: options\n  operationId: getCardTransactionReceiptOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/card-transactions\n  method: get\n  operationId: listCardTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/card-transactions/{transactionId}/post\n  method: post\n  operationId: postCardTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/card-transactions/{transactionId}/reset\n  method: post\n  operationId: resetCardTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/card-transactions/{transactionId}\n  method: patch\n  operationId: updateCardTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n  \
  \  audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/card-transactions/{transactionId}/lines/{transactionLineId}\n  method: patch\n  operationId: updateCardTransactionLine\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/cards\n  method: get\n  operationId: listCards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cards\n  method: post\n  operationId: createCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/cards/{cardId}/freeze\n  method: post\n  operationId: freezeCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/cards/{cardId}\n  method: get\n  operationId: getCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cards/{cardId}/unfreeze\n  method: post\n  operationId: unfreezeCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/entities\n  method: get\n  operationId: getCompanyEntities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/current\n  method: get\n  operationId: getCurrentCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/contracts/{contractId}/cancel-termination\n  method: post\n  operationId: cancelContractTermination\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/contracts\n  method: get\n  operationId: listContracts\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/contracts\n  method: post\n  operationId: createContract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/contracts/{contractId}/lines\n  method: post\n  operationId: createContractLine\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/contracts/{contractId}\n  method: get\n  operationId: getContract\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/contracts/{contractId}\n  method: delete\n  operationId: deleteContract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/contracts/{contractId}\n  method: patch\n  operationId: updateContract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/contracts/{contractId}/lines/{lineId}\n  method: delete\n  operationId: deleteContractLine\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/contracts/{contractId}/lines/{lineId}\n  method: patch\n  operationId: updateContractLine\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/contracts/{contractId}/generate-document-upload-url\n  method: post\n  operationId: generateContractDocumentUploadUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/contracts/{contractId}/publish\n  method: post\n\
  \  operationId: publishContract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/contracts/{contractId}/renew\n  method: post\n  operationId: renewContract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/contracts/{contractId}/reset\n  method: post\n  operationId: resetContract\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n\
  \    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/contracts/{contractId}/terminate\n  method: post\n  operationId: terminateContract\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/credit-notes/{creditNoteId}/archive\n  method: post\n  operationId: archiveCreditNote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/credit-notes\n  method: get\n  operationId: listCreditNotes\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/credit-notes\n  method: post\n  operationId: createCreditNote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/credit-notes/{creditNoteId}/lines\n  method: post\n  operationId: createCreditNoteLine\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/credit-notes/create-from-invoice-payable/{invoicePayableId}\n  method: post\n  operationId: createCreditNoteFromInvoicePayable\n  x-agentic-access:\n    action-class: acting\n  \
  \  consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/credit-notes/{creditNoteId}/lines/{lineId}\n  method: delete\n  operationId: deleteCreditNoteLine\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/credit-notes/{creditNoteId}/lines/{lineId}\n  method: patch\n  operationId: updateCreditNoteLine\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/credit-notes/{creditNoteId}\n  method: get\n  operationId: getCreditNote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/credit-notes/{creditNoteId}\n  method: patch\n  operationId: updateCreditNote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/credit-notes/{creditNoteId}/document\n  method: get\n  operationId: getAttachedDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/credit-notes/{creditNoteId}/invoice-payables\n  method: get\n  operationId: getLinkedInvoicePayables\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/credit-notes/{creditNoteId}/invoice-payables/{invoicePayableId}\n  method: post\n  operationId: linkCreditNoteToInvoicePayable\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/credit-notes/{creditNoteId}/invoice-payables/{invoicePayableId}\n  method: delete\n  operationId: unlinkFromInvoicePayable\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/credit-notes/{creditNoteId}/invoice-payables/{invoicePayableId}\n  method: patch\n  operationId: updateLinkedInvoicePayable\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/credit-notes/{creditNoteId}/post\n  method: post\n  operationId: postCreditNote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/custom-properties/groups/{groupId}/values\n  method: get\n  operationId:\
  \ listPaginatedCustomPropertyValues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/custom-properties/groups/{groupId}/values\n  method: post\n  operationId: createCustomPropertyValue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/custom-properties/groups/{groupId}/values/{valueId}\n  method: get\n  operationId: getCustomPropertyValueById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/custom-properties/groups/{groupId}/values/{valueId}\n  method: delete\n  operationId: deleteCustomPropertyValue\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/custom-properties/groups/{groupId}/values/{valueId}\n  method: patch\n  operationId: updateCustomPropertyValue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/custom-properties/groups/{groupId}\n  method: get\n  operationId: getCustomPropertyGroupById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/custom-properties/groups\n  method: get\n  operationId: listPaginatedCustomPropertyGroups\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customer-credits/{customerCreditId}/archive\n  method: post\n  operationId: archiveCustomerCredit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customer-credits\n  method: get\n  operationId: listCustomerCredits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customer-credits\n  method: post\n  operationId: createCustomerCredit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customer-credits/{customerCreditId}/lines\n  method: post\n  operationId: createCustomerCreditLine\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customer-credits/{customerCreditId}/lines/{lineId}\n  method: delete\n  operationId: deleteCustomerCreditLine\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customer-credits/{customerCreditId}/lines/{lineId}\n  method: patch\n  operationId: updateCustomerCreditLine\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customer-credits/{customerCreditId}\n  method: get\n  operationId: getCustomerCredit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customer-credits/{customerCreditId}\n  method: patch\n  operationId: updateCustomerCredit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customer-credits/{customerCreditId}/invoice-receivables/{invoiceReceivableId}/link\n \
  \ method: post\n  operationId: linkCustomerCreditToInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customer-credits/{customerCreditId}/invoice-receivables/{invoiceReceivableId}\n  method: post\n  operationId: linkCustomerCredit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customer-credits/{customerCreditId}/invoice-receivables/{invoiceReceivableId}\n  method: delete\n  operationId: unlinkCustomerCredit\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customer-credits/{customerCreditId}/post-and-send-email\n  method: post\n  operationId: postAndSendCustomerCredit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customer-credits/{customerCreditId}/post\n  method: post\n  operationId: postCustomerCredit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customer-credits/{customerCreditId}/submit-einvoice\n  method: post\n  operationId: submitCustomerCreditEInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customer-credits/{customerCreditId}/unarchive\n  method: post\n  operationId: unarchiveCustomerCredit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/customer-credits/{customerCreditId}/invoice-receivables/{invoiceReceivableId}/unlink\n  method: post\n  operationId: unlinkCustomerCreditFromInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customers/{customerId}/activate\n  method: post\n  operationId: activateCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customers/{customerId}/archive\n  method: post\n  operationId: archiveCustomer\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customers\n  method: get\n  operationId: listCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customers\n  method: post\n  operationId: createCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customers/{customerId}\n  method: get\n  operationId: getCustomerById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customers/{customerId}\n  method: patch\n  operationId: updateCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/exchange/rates/{base}/{target}\n  method: get\n  operationId: getRate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/exchange/rates/{currency}\n  method: get\n  operationId: getRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/expenses/{expenseId}/cancel\n  method: post\n  operationId: cancelExpense\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: write\n    subject: required\n    audience: null\n    to\n\n# --- truncated at 32 KB (60 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/light/refs/heads/main/agentic-access/light-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/light/refs/heads/main/agentic-access/light-agentic-access.yml
summary_line: 183 operations · 120 acting · 5 human-in-the-loop
tags:
- Accounting
- Finance
- ERP
- Accounts Payable
- Accounts Receivable
- General Ledger
- Spend Management
- Invoicing
- Corporate Cards
- Expense Management
- Financial Operations
- Agents
- Company
---
