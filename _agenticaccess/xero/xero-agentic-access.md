---
acting_count: 214
action_class_counts:
  acting: 214
  connected: 252
api_specs:
- filename: xero-accounting-openapi.yml
  format: yaml
  label: Xero Accounting API
  slug: xero-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-accounting-openapi.yml
- filename: xero-assets-openapi.yml
  format: yaml
  label: Xero Assets API
  slug: xero-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-assets-openapi.yml
- filename: xero-bankfeeds-openapi.yml
  format: yaml
  label: Xero Bank Feeds API
  slug: xero-bank-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-bankfeeds-openapi.yml
- filename: xero-finance-openapi.yml
  format: yaml
  label: Xero Finance API
  slug: xero-finance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-finance-openapi.yml
- filename: xero-identity-openapi.yml
  format: yaml
  label: Xero Identity API
  slug: xero-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-identity-openapi.yml
- filename: xero-payroll-au-openapi.yml
  format: yaml
  label: Xero Payroll Australia API
  slug: xero-payroll-australia-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-payroll-au-openapi.yml
- filename: xero-payroll-nz-openapi.yml
  format: yaml
  label: Xero Payroll New Zealand API
  slug: xero-payroll-new-zealand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-payroll-nz-openapi.yml
- filename: xero-payroll-uk-openapi.yml
  format: yaml
  label: Xero Payroll United Kingdom API
  slug: xero-payroll-united-kingdom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-payroll-uk-openapi.yml
- filename: xero-projects-openapi.yml
  format: yaml
  label: Xero Projects API
  slug: xero-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-projects-openapi.yml
- filename: xero-files-openapi.yml
  format: yaml
  label: Xero Files API
  slug: xero-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-files-openapi.yml
consequence_counts:
  physical: 41
  read: 252
  write: 173
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Xero Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /BankTransfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /BankTransfers/{BankTransferID}/Attachments/{FileName}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /BankTransfers/{BankTransferID}/Attachments/{FileName}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /BankTransfers/{BankTransferID}/History
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /BatchPayments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /BatchPayments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /BatchPayments/{BatchPaymentID}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /BatchPayments/{BatchPaymentID}/History
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /BrandingThemes/{BrandingThemeID}/PaymentServices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /Employees/{EmployeeID}/PaymentMethods
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /Employees/{EmployeeID}/PaymentMethods
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /Invoices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /Invoices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /Invoices/{InvoiceID}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /Invoices/{InvoiceID}/Attachments/{FileName}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /Invoices/{InvoiceID}/Attachments/{FileName}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /Invoices/{InvoiceID}/Email
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /Invoices/{InvoiceID}/History
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /Overpayments/{OverpaymentID}/Allocations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /Overpayments/{OverpaymentID}/Allocations/{AllocationID}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /Overpayments/{OverpaymentID}/History
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /PaymentServices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /Payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /Payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /Payments/{PaymentID}
operation_count: 466
overview: 'Xero exposes 466 API operations that an AI agent could call, of which 214 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 252 read, 173 write, and 41 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Xero
provider_slug: xero
slug: xero-agentic-access
source_filename: xero-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/xero-accounting-openapi.yml, openapi/xero-assets-openapi.yml, openapi/xero-bankfeeds-openapi.yml,\n  openapi/xero-files-openapi.yml, openapi/xero-finance-openapi.yml, openapi/xero-identity-openapi.yml,\n  openapi/xero-payroll-au-openapi.yml, openapi/xero-payroll-nz-openapi.yml, openapi/xero-payroll-uk-openapi.yml,\n  openapi/xero-projects-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 466\n  by_action_class:\n    connected: 252\n    acting: 214\n  by_consequence:\n    read: 252\n    write: 173\n    physical: 41\n  human_in_the_loop_required: 0\noperations:\n- path: /Accounts\n  method: get\n  operationId: getAccounts\n  x-agentic-access:\n    action-class: connected\n \
  \   consequence: read\n    subject: optional\n    scope:\n    - accounting.settings\n    - accounting.settings.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Accounts\n  method: put\n  operationId: createAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounting.settings\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Accounts/{AccountID}\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounting.settings\n    - accounting.settings.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Accounts/{AccountID}\n  method: post\n  operationId: updateAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    scope:\n    - accounting.settings\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Accounts/{AccountID}\n  method: delete\n  operationId: deleteAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounting.settings\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Accounts/{AccountID}/Attachments\n  method: get\n  operationId: getAccountAttachments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounting.attachments\n    - accounting.attachments.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Accounts/{AccountID}/Attachments/{AttachmentID}\n  method:\
  \ get\n  operationId: getAccountAttachmentById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounting.attachments\n    - accounting.attachments.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Accounts/{AccountID}/Attachments/{FileName}\n  method: get\n  operationId: getAccountAttachmentByFileName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounting.attachments\n    - accounting.attachments.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Accounts/{AccountID}/Attachments/{FileName}\n  method: post\n  operationId: updateAccountAttachmentByFileName\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounting.attachments\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /Accounts/{AccountID}/Attachments/{FileName}\n  method: put\n  operationId: createAccountAttachmentByFileName\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounting.attachments\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /BatchPayments\n  method: get\n  operationId: getBatchPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounting.transactions\n    - accounting.transactions.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /BatchPayments\n  method: put\n  operationId: createBatchPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - accounting.transactions\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /BatchPayments\n  method: post\n  operationId: deleteBatchPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - accounting.transactions\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /BatchPayments/{BatchPaymentID}\n  method: get\n  operationId: getBatchPayment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounting.transactions\n    - accounting.transactions.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /BatchPayments/{BatchPaymentID}\n\
  \  method: post\n  operationId: deleteBatchPaymentByUrlParam\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - accounting.transactions\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /BatchPayments/{BatchPaymentID}/History\n  method: get\n  operationId: getBatchPaymentHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounting.transactions\n    - accounting.transactions.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /BatchPayments/{BatchPaymentID}/History\n  method: put\n  operationId: createBatchPaymentHistoryRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - accounting.transactions\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /BankTransactions\n  method: get\n  operationId: getBankTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounting.transactions\n    - accounting.transactions.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /BankTransactions\n  method: put\n  operationId: createBankTransactions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounting.transactions\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /BankTransactions\n  method: post\n  operationId: updateOrCreateBankTransactions\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounting.transactions\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /BankTransactions/{BankTransactionID}\n  method: get\n  operationId: getBankTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounting.transactions\n    - accounting.transactions.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /BankTransactions/{BankTransactionID}\n  method: post\n  operationId: updateBankTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounting.transactions\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /BankTransactions/{BankTransactionID}/Attachments\n  method: get\n  operationId: getBankTransactionAttachments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounting.attachments\n    - accounting.attachments.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /BankTransactions/{BankTransactionID}/Attachments/{AttachmentID}\n  method: get\n  operationId: getBankTransactionAttachmentById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounting.attachments\n    - accounting.attachments.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /BankTransactions/{BankTransactionID}/Attachments/{FileName}\n  method: get\n  operationId: getBankTransactionAttachmentByFileName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    scope:\n    - accounting.attachments\n    - accounting.attachments.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /BankTransactions/{BankTransactionID}/Attachments/{FileName}\n  method: post\n  operationId: updateBankTransactionAttachmentByFileName\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounting.attachments\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /BankTransactions/{BankTransactionID}/Attachments/{FileName}\n  method: put\n  operationId: createBankTransactionAttachmentByFileName\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounting.attachments\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n     \
  \ - abnormal\n      - high-value\n    audit: required\n- path: /BankTransactions/{BankTransactionID}/History\n  method: get\n  operationId: getBankTransactionsHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounting.transactions\n    - accounting.transactions.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /BankTransactions/{BankTransactionID}/History\n  method: put\n  operationId: createBankTransactionHistoryRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounting.transactions\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /BankTransfers\n  method: get\n  operationId: getBankTransfers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    scope:\n    - accounting.transactions\n    - accounting.transactions.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /BankTransfers\n  method: put\n  operationId: createBankTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - accounting.transactions\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /BankTransfers/{BankTransferID}\n  method: get\n  operationId: getBankTransfer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounting.transactions\n    - accounting.transactions.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /BankTransfers/{BankTransferID}/Attachments\n  method: get\n  operationId: getBankTransferAttachments\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounting.attachments\n    - accounting.attachments.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /BankTransfers/{BankTransferID}/Attachments/{AttachmentID}\n  method: get\n  operationId: getBankTransferAttachmentById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounting.attachments\n    - accounting.attachments.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /BankTransfers/{BankTransferID}/Attachments/{FileName}\n  method: get\n  operationId: getBankTransferAttachmentByFileName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounting.attachments\n    - accounting.attachments.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /BankTransfers/{BankTransferID}/Attachments/{FileName}\n  method:\
  \ post\n  operationId: updateBankTransferAttachmentByFileName\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - accounting.attachments\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /BankTransfers/{BankTransferID}/Attachments/{FileName}\n  method: put\n  operationId: createBankTransferAttachmentByFileName\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - accounting.attachments\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /BankTransfers/{BankTransferID}/History\n  method:\
  \ get\n  operationId: getBankTransferHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounting.transactions\n    - accounting.transactions.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /BankTransfers/{BankTransferID}/History\n  method: put\n  operationId: createBankTransferHistoryRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - accounting.transactions\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /BrandingThemes\n  method: get\n  operationId: getBrandingThemes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounting.settings\n    - accounting.settings.read\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /BrandingThemes/{BrandingThemeID}\n  method: get\n  operationId: getBrandingTheme\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounting.settings\n    - accounting.settings.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /BrandingThemes/{BrandingThemeID}/PaymentServices\n  method: get\n  operationId: getBrandingThemePaymentServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - paymentservices\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /BrandingThemes/{BrandingThemeID}/PaymentServices\n  method: post\n  operationId: createBrandingThemePaymentServices\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - paymentservices\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n     \
  \ purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Budgets\n  method: get\n  operationId: getBudgets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounting.budgets.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Budgets/{BudgetID}\n  method: get\n  operationId: getBudget\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounting.budgets.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Contacts\n  method: get\n  operationId: getContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounting.contacts\n    - accounting.contacts.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Contacts\n  method: put\n  operationId: createContacts\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounting.contacts\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Contacts\n  method: post\n  operationId: updateOrCreateContacts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounting.contacts\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Contacts/{ContactNumber}\n  method: get\n  operationId: getContactByContactNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounting.contacts\n    - accounting.contacts.read\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /Contacts/{ContactID}\n  method: get\n  operationId: getContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounting.contacts\n    - accounting.contacts.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Contacts/{ContactID}\n  method: post\n  operationId: updateContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounting.contacts\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Contacts/{ContactID}/Attachments\n  method: get\n  operationId: getContactAttachments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounting.attachments\n    - accounting.attachments.read\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /Contacts/{ContactID}/Attachments/{AttachmentID}\n  method: get\n  operationId: getContactAttachmentById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounting.attachments\n    - accounting.attachments.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Contacts/{ContactID}/Attachments/{FileName}\n  method: get\n  operationId: getContactAttachmentByFileName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounting.attachments\n    - accounting.attachments.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Contacts/{ContactID}/Attachments/{FileName}\n  method: post\n  operationId: updateContactAttachmentByFileName\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounting.attachments\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Contacts/{ContactID}/Attachments/{FileName}\n  method: put\n  operationId: createContactAttachmentByFileName\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounting.attachments\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Contacts/{ContactID}/CISSettings\n  method: get\n  operationId: getContactCISSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounting.settings\n    - accounting.settings.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Contacts/{ContactID}/History\n  method: get\n  operationId: getContactHistory\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounting.contacts\n    - accounting.contacts.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Contacts/{ContactID}/History\n  method: put\n  operationId: createContactHistory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounting.contacts\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ContactGroups\n  method: get\n  operationId: getContactGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounting.contacts\n    - accounting.contacts.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ContactGroups\n  method: put\n  operationId: createContactGroup\n  x-agentic-access:\n    action-class: acting\n  \
  \  consequence: write\n    subject: required\n    scope:\n    - accounting.contacts\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ContactGroups/{ContactGroupID}\n  method: get\n  operationId: getContactGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounting.contacts\n    - accounting.contacts.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ContactGroups/{ContactGroupID}\n  method: post\n  operationId: updateContactGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounting.contacts\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ContactGroups/{ContactGroupID}/Contacts\n\
  \  method: put\n  operationId: createContactGroupContacts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounting.contacts\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ContactGroups/{ContactGroupID}/Contacts\n  method: delete\n  operationId: deleteContactGroupContacts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounting.contacts\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ContactGroups/{ContactGroupID}/Contacts/{ContactID}\n  method: delete\n  operationId: deleteContactGroupContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    scope:\n    - accounting.contacts\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /CreditNotes\n  method: get\n  operationId: getCreditNotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounting.transactions\n    - accounting.transactions.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /CreditNotes\n  method: put\n  operationId: createCreditNotes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounting.transactions\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /CreditNotes\n  method: post\n  operationId: updateOrCreateCreditNotes\n \
  \ x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounting.transactions\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /CreditNotes/{CreditNoteID}\n  method: get\n  operationId: getCreditNote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounting.transactions\n    - accounting.transactions.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /CreditNotes/{CreditNoteID}\n  method: post\n  operationId: updateCreditNote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounting.transactions\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /CreditNotes/{CreditNoteID}/Attachments\n  method: get\n  operationId: getCreditNoteAttachments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounting.attachments\n    - accounting.attachments.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /CreditNotes/{CreditNoteID}/Attachments/{AttachmentID}\n  method: get\n  operationId: getCreditNoteAttachmentById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounting.attachments\n    - accounting.attachments.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /CreditNotes/{CreditNoteID}/Attachments/{FileName}\n  method: get\n  operationId: getCreditNoteAttachmentByFileName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounting.attachments\n    - accounting.attachments.read\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /CreditNotes/{CreditNoteID}/Attachments/{FileName}\n  method: post\n  operationId: updateCreditNoteAttachmentByFileName\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounting.attachments\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /CreditNotes/{CreditNoteID}/Attachments/{FileName}\n  method: put\n  operationId: createCreditNoteAttachmentByFileName\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounting.attachments\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /CreditNotes/{CreditNoteID}/pdf\n  method: get\n\
  \  operationId: getCreditNoteAsPdf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounting.transactions\n    - accounting.transactions.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /CreditNotes/{CreditNoteID}/Allocations\n  method: put\n  operationId: createCreditNoteAllocation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounting.transactions\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /CreditNotes/{CreditNoteID}/Allocations/{AllocationID}\n  method: delete\n  operationId: deleteCreditNoteAllocations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounting.transactions\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /CreditNotes/{CreditNoteID}/History\n  method: get\n  operationId: getCreditNoteHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounting.transactions\n    - accounting.transactions.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /CreditNotes/{CreditNoteID}/History\n  method: put\n  operationId: createCreditNoteHistory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounting.transactions\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Currencies\n  method: get\n  operationId: getCurrencies\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    scope:\n    - accounting.settings\n    - accounting.settings.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Currencies\n  method: put\n  operationId: createCurrency\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounting.settings\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Employees\n  method: get\n  operationId: getEmployees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounting.settings\n    - accounting.settings.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Employees\n  method: put\n  operationId: createEmployees\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounting.settings\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Employees\n  method: post\n  operationId: updateOrCreateEmployees\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounting.settings\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Employees/{EmployeeID}\n  method: get\n  operationId: getEmployee\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounting.settings\n    - accounting.settings.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ExpenseClaims\n  method: get\n  operationId: getExpenseClaims\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    scope:\n    - accounting.transactions\n    - accounting.transactions.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ExpenseClaims\n  method: put\n  operationId: createExpenseClaims\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounting.transactions\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ExpenseClaims/{ExpenseClaimID}\n  method: get\n  operationId: getExpenseClaim\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounting.transactions\n    - accounting.transactions.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ExpenseClaims/{ExpenseClaimID}\n  method: post\n  operationId: updateExpenseClaim\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: writ\n\n# --- truncated at 32 KB (155 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/agentic-access/xero-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/agentic-access/xero-agentic-access.yml
summary_line: 466 operations · 214 acting
tags:
- Accounting
- Bank Feeds
- Finance
- Financial Services
- Invoicing
- Payroll
- Small Business
---
