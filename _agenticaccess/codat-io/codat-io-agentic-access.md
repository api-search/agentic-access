---
acting_count: 16
action_class_counts:
  acting: 16
  connected: 36
api_specs:
- filename: codat-io-openapi.yml
  format: yaml
  label: Codat Platform API
  slug: codat-io-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat-io/refs/heads/main/openapi/codat-io-openapi.yml
- filename: codat-io-openapi.yml
  format: yaml
  label: Codat Accounting API
  slug: codat-io-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat-io/refs/heads/main/openapi/codat-io-openapi.yml
- filename: codat-io-openapi.yml
  format: yaml
  label: Codat Banking API
  slug: codat-io-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat-io/refs/heads/main/openapi/codat-io-openapi.yml
- filename: codat-io-openapi.yml
  format: yaml
  label: Codat Commerce API
  slug: codat-io-commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat-io/refs/heads/main/openapi/codat-io-openapi.yml
- filename: codat-io-openapi.yml
  format: yaml
  label: Codat Lending API
  slug: codat-io-lending-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat-io/refs/heads/main/openapi/codat-io-openapi.yml
- filename: codat-io-openapi.yml
  format: yaml
  label: Codat Bank Feeds API
  slug: codat-io-bank-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat-io/refs/heads/main/openapi/codat-io-openapi.yml
- filename: codat-io-openapi.yml
  format: yaml
  label: Codat Sync for Payables API
  slug: codat-io-sync-for-payables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat-io/refs/heads/main/openapi/codat-io-openapi.yml
- filename: codat-io-openapi.yml
  format: yaml
  label: Codat Sync for Expenses API
  slug: codat-io-sync-for-expenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat-io/refs/heads/main/openapi/codat-io-openapi.yml
- filename: codat-io-openapi.yml
  format: yaml
  label: Codat Sync for Commerce API
  slug: codat-io-sync-for-commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat-io/refs/heads/main/openapi/codat-io-openapi.yml
consequence_counts:
  physical: 1
  read: 36
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Codat Io Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /companies/{companyId}/connections/{connectionId}/payables/bills/{billId}/payment
operation_count: 52
overview: 'Codat exposes 52 API operations that an AI agent could call, of which 16 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 36 read, 15 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Codat
provider_slug: codat-io
slug: codat-io-agentic-access
source_filename: codat-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/codat-io-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 52\n  by_action_class:\n    connected: 36\n    acting: 16\n  by_consequence:\n    read: 36\n    write: 15\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /companies\n  method: get\n  operationId: listCompanies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies\n  method: post\n  operationId: createCompany\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{companyId}\n  method: get\n  operationId: getCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyId}\n  method: patch\n  operationId: updateCompany\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{companyId}\n  method: delete\n  operationId: deleteCompany\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /companies/{companyId}/connections\n  method: get\n  operationId: listConnections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyId}/connections\n  method: post\n  operationId: createConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{companyId}/connections/{connectionId}\n  method: get\n  operationId: getConnection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyId}/connections/{connectionId}\n  method: delete\n  operationId: deleteConnection\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{companyId}/connections/{connectionId}\n  method: patch\n  operationId: unlinkConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{companyId}/data/all\n  method: post\n  operationId: refreshAllData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /companies/{companyId}/data/queue/{dataType}\n  method: post\n  operationId: refreshDataType\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{companyId}/dataStatus\n  method: get\n  operationId: getDataStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: get\n  operationId: listWebhookConsumers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: post\n  operationId: createWebhookConsumer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n  \
  \  audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integrations\n  method: get\n  operationId: listIntegrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integrations/{platformKey}\n  method: get\n  operationId: getIntegration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyId}/data/accounts\n  method: get\n  operationId: listAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyId}/data/accounts/{accountId}\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyId}/connections/{connectionId}/data/invoices\n  method: get\n  operationId: listInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyId}/connections/{connectionId}/data/invoices/{invoiceId}\n  method: get\n  operationId: getInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyId}/connections/{connectionId}/data/bills\n  method: get\n  operationId: listBills\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyId}/connections/{connectionId}/data/journalEntries\n  method: get\n  operationId:\
  \ listJournalEntries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyId}/connections/{connectionId}/data/customers\n  method: get\n  operationId: listCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyId}/connections/{connectionId}/data/suppliers\n  method: get\n  operationId: listSuppliers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyId}/connections/{connectionId}/data/financials/balanceSheet\n  method: get\n  operationId: getBalanceSheet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyId}/connections/{connectionId}/data/financials/profitAndLoss\n\
  \  method: get\n  operationId: getProfitAndLoss\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyId}/connections/{connectionId}/data/financials/cashFlowStatement\n  method: get\n  operationId: getCashFlowStatement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyId}/connections/{connectionId}/data/banking-accounts\n  method: get\n  operationId: listBankingAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyId}/connections/{connectionId}/data/banking-transactions\n  method: get\n  operationId: listBankingTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyId}/connections/{connectionId}/data/banking-transactionCategories\n  method: get\n  operationId: listBankingTransactionCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyId}/connections/{connectionId}/data/commerce-customers\n  method: get\n  operationId: listCommerceCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyId}/connections/{connectionId}/data/commerce-orders\n  method: get\n  operationId: listCommerceOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyId}/connections/{connectionId}/data/commerce-payments\n  method:\
  \ get\n  operationId: listCommercePayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyId}/connections/{connectionId}/data/commerce-products\n  method: get\n  operationId: listCommerceProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyId}/reports/enhancedBalanceSheet/accounts\n  method: get\n  operationId: getEnhancedBalanceSheetAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyId}/reports/enhancedProfitAndLoss/accounts\n  method: get\n  operationId: getEnhancedProfitAndLossAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /data/companies/{companyId}/assess/dataTypes/{dataType}/dataIntegrity/status\n  method: get\n  operationId: getDataIntegrityStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyId}/connections/{connectionId}/data/bankAccounts\n  method: get\n  operationId: listBankFeedBankAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyId}/connections/{connectionId}/data/bankAccounts\n  method: put\n  operationId: createBankFeedBankAccounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /companies/{companyId}/connections/{connectionId}/bankFeedAccounts\n  method: get\n  operationId: getBankFeedConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyId}/connections/{connectionId}/payables/bills\n  method: get\n  operationId: listPayablesBills\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyId}/connections/{connectionId}/payables/bills\n  method: post\n  operationId: createPayableBill\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{companyId}/connections/{connectionId}/payables/bills/{billId}/payment\n\
  \  method: post\n  operationId: createBillPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{companyId}/connections/{connectionId}/payables/suppliers\n  method: post\n  operationId: createPayableSupplier\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{companyId}/sync/expenses/expense-transactions\n  method: post\n  operationId: createExpenseTransactions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{companyId}/sync/expenses/syncs/latest/status\n  method: get\n  operationId: getLatestExpenseSyncStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyId}/sync/expenses/mappingOptions\n  method: get\n  operationId: getExpenseMappingOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyId}/sync/commerce/latest\n  method: post\n  operationId: requestCommerceSync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n   \
  \   human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /config/companies/{companyId}/sync/commerce\n  method: get\n  operationId: getCommerceConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /config/companies/{companyId}/sync/commerce\n  method: post\n  operationId: setCommerceConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /meta/companies/{companyId}/sync/commerce/status\n  method: get\n  operationId: getCommerceSyncStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codat-io/refs/heads/main/agentic-access/codat-io-agentic-access.yml
summary_line: 52 operations · 16 acting
tags:
- Business Data
- Accounting
- Banking
- Commerce
- Fintech
- Lending
- Financial Data
---
