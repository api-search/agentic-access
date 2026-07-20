---
acting_count: 27
action_class_counts:
  acting: 27
  connected: 19
api_specs:
- filename: pennylane-openapi.yml
  format: yaml
  label: Pennylane Customer Invoicing API
  slug: pennylane-customer-invoicing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-openapi.yml
- filename: pennylane-openapi.yml
  format: yaml
  label: Pennylane Supplier Invoicing API
  slug: pennylane-supplier-invoicing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-openapi.yml
- filename: pennylane-openapi.yml
  format: yaml
  label: Pennylane Accounting & Ledger API
  slug: pennylane-accounting-ledger-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-openapi.yml
- filename: pennylane-openapi.yml
  format: yaml
  label: Pennylane Accounting Exports API
  slug: pennylane-accounting-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-openapi.yml
- filename: pennylane-openapi.yml
  format: yaml
  label: Pennylane Banking API
  slug: pennylane-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-openapi.yml
- filename: pennylane-openapi.yml
  format: yaml
  label: Pennylane Customers & Suppliers API
  slug: pennylane-customers-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-openapi.yml
- filename: pennylane-openapi.yml
  format: yaml
  label: Pennylane Products Catalog API
  slug: pennylane-products-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-openapi.yml
- filename: pennylane-openapi.yml
  format: yaml
  label: Pennylane Quotes API
  slug: pennylane-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-openapi.yml
- filename: pennylane-openapi.yml
  format: yaml
  label: Pennylane Billing Subscriptions API
  slug: pennylane-billing-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-openapi.yml
- filename: pennylane-openapi.yml
  format: yaml
  label: Pennylane Direct Debit Mandates API
  slug: pennylane-mandates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-openapi.yml
- filename: pennylane-openapi.yml
  format: yaml
  label: Pennylane Change Events API
  slug: pennylane-change-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-openapi.yml
- filename: pennylane-openapi.yml
  format: yaml
  label: Pennylane E-Invoicing (Plateforme Agréée) API
  slug: pennylane-einvoicing-pa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-openapi.yml
consequence_counts:
  read: 19
  write: 27
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. Financial write operations (invoices, transactions, mandates, exports) are treated as high-value and default to human-in-the-loop escalation. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Pennylane Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 46
overview: 'Pennylane exposes 46 API operations that an AI agent could call, of which 27 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read and 27 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Pennylane
provider_slug: pennylane
slug: pennylane-agentic-access
source_filename: pennylane-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: generated\nsource: openapi/pennylane-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. Financial write operations (invoices, transactions, mandates,\n  exports) are treated as high-value and default to human-in-the-loop escalation.\n  See research/curity/agentic-governance/.\nsummary:\n  operations: 46\n  by_action_class:\n    acting: 27\n    connected: 19\n  by_consequence:\n    write: 27\n    read: 19\n  human_in_the_loop_required: 0\noperations:\n- path: /me\n  method: get\n  operationId: getMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /journals\n  method: get\n  operationId: getJournals\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /journals\n  method: post\n  operationId: postJournals\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /journals/{id}\n  method: get\n  operationId: getJournal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ledger_accounts\n  method: get\n  operationId: getLedgerAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ledger_accounts\n  method: post\n  operationId: postLedgerAccounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ledger_accounts/{id}\n  method: get\n  operationId: getLedgerAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ledger_accounts/{id}\n  method: put\n  operationId: updateLedgerAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ledger_entries\n  method: get\n  operationId: getLedgerEntries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /ledger_entries\n  method: post\n  operationId: postLedgerEntries\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ledger_entries/{id}\n  method: get\n  operationId: getLedgerEntry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ledger_entries/{id}\n  method: put\n  operationId: putLedgerEntries\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /trial_balance\n  method: get\n  operationId: getTrialBalance\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fiscal_years\n  method: get\n  operationId: getFiscalYears\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exports/general_ledger\n  method: post\n  operationId: exportGeneralLedger\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /exports/fec\n  method: post\n  operationId: exportFec\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /categories\n  method: get\n  operationId: getCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /categories\n  method: post\n  operationId: postCategories\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /category_groups\n  method: get\n  operationId: getCategoryGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer_invoices\n  method: get\n  operationId: getCustomerInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer_invoices\n  method: post\n  operationId: postCustomerInvoices\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer_invoices/import\n  method: post\n  operationId: importCustomerInvoices\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer_invoices/{id}\n  method: get\n  operationId: getCustomerInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /customer_invoices/{id}\n  method: put\n  operationId: updateCustomerInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer_invoices/{id}/finalize\n  method: put\n  operationId: finalizeCustomerInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - irreversible\n      - high-value\n    audit: required\n- path: /customer_invoices/{id}/mark_as_paid\n  method: put\n  operationId: markAsPaidCustomerInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer_invoices/{id}/send_by_email\n  method: post\n  operationId: sendByEmailCustomerInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - external-communication\n    audit: required\n- path: /customer_invoices/{id}/matched_transactions\n  method: post\n  operationId: postCustomerInvoiceMatchedTransactions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /supplier_invoices\n  method: get\n  operationId: getSupplierInvoices\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /supplier_invoices/import\n  method: post\n  operationId: importSupplierInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /supplier_invoices/{id}\n  method: get\n  operationId: getSupplierInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /supplier_invoices/{id}\n  method: put\n  operationId: putSupplierInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /supplier_invoices/{id}/validate_accounting\n  method: put\n  operationId: validateAccountingSupplierInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - irreversible\n      - high-value\n    audit: required\n- path: /quotes\n  method: get\n  operationId: listQuotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /quotes\n  method: post\n  operationId: postQuotes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /quotes/{id}\n  method: get\n  operationId: getQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing_subscriptions\n  method: get\n  operationId: getBillingSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing_subscriptions\n  method: post\n  operationId: postBillingSubscriptions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /products\n  method: get\n  operationId: getProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /products\n  method: post\n  operationId: postProducts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /products/{id}\n  method: put\n  operationId: putProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers\n  method: get\n  operationId: getCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company_customers\n  method: post\n  operationId: postCompanyCustomer\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /suppliers\n  method: get\n  operationId: getSuppliers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /suppliers\n  method: post\n  operationId: postSupplier\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bank_accounts\n  method: get\n  operationId: getBankAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions\n  method: get\n  operationId: getTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions\n  method: post\n  operationId: createTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transactions/{id}\n  method: put\n  operationId: updateTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sepa_mandates\n  method:\
  \ get\n  operationId: getSepaMandates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sepa_mandates\n  method: post\n  operationId: postSepaMandates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - irreversible\n      - high-value\n    audit: required\n- path: /file_attachments\n  method: post\n  operationId: postFileAttachments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer_invoices/changes\n  method: get\n  operationId: getCustomerInvoicesChanges\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pa_registrations\n  method: get\n  operationId: getPaRegistrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/agentic-access/pennylane-agentic-access.yml
summary_line: 46 operations · 27 acting
tags:
- Accounting
- Invoicing
- Fintech
- Financial Data
- Banking
- France
- SME
---
