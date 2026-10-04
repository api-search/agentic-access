---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 21
api_specs:
- filename: oracle-financials-budgetary-control-api-openapi.yml
  format: yaml
  label: Oracle Financials Budgetary Control API
  slug: oracle-financials-budgetary-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-financials/refs/heads/main/openapi/oracle-financials-budgetary-control-api-openapi.yml
- filename: oracle-financials-chart-of-accounts-api-openapi.yml
  format: yaml
  label: Oracle Financials Chart of Accounts API
  slug: oracle-financials-chart-of-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-financials/refs/heads/main/openapi/oracle-financials-chart-of-accounts-api-openapi.yml
- filename: oracle-financials-currency-rates-api-openapi.yml
  format: yaml
  label: Oracle Financials Currency Rates API
  slug: oracle-financials-currency-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-financials/refs/heads/main/openapi/oracle-financials-currency-rates-api-openapi.yml
- filename: oracle-financials-journal-batches-api-openapi.yml
  format: yaml
  label: Oracle Financials Journal Batches API
  slug: oracle-financials-journal-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-financials/refs/heads/main/openapi/oracle-financials-journal-batches-api-openapi.yml
- filename: oracle-financials-ledger-balances-api-openapi.yml
  format: yaml
  label: Oracle Financials Ledger Balances API
  slug: oracle-financials-ledger-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-financials/refs/heads/main/openapi/oracle-financials-ledger-balances-api-openapi.yml
- filename: oracle-financials-accounting-periods-api-openapi.yml
  format: yaml
  label: Oracle Financials Accounting Periods API
  slug: oracle-financials-accounting-periods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-financials/refs/heads/main/openapi/oracle-financials-accounting-periods-api-openapi.yml
- filename: oracle-financials-cash-management-api-openapi.yml
  format: yaml
  label: Oracle Financials Cash Management API
  slug: oracle-financials-cash-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-financials/refs/heads/main/openapi/oracle-financials-cash-management-api-openapi.yml
- filename: oracle-financials-erp-integrations-api-openapi.yml
  format: yaml
  label: Oracle Financials ERP Integrations API
  slug: oracle-financials-erp-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-financials/refs/heads/main/openapi/oracle-financials-erp-integrations-api-openapi.yml
- filename: oracle-financials-fixed-assets-api-openapi.yml
  format: yaml
  label: Oracle Financials Fixed Assets API
  slug: oracle-financials-fixed-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-financials/refs/heads/main/openapi/oracle-financials-fixed-assets-api-openapi.yml
- filename: oracle-financials-general-ledger-api-openapi.yml
  format: yaml
  label: Oracle Financials General Ledger API
  slug: oracle-financials-general-ledger-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-financials/refs/heads/main/openapi/oracle-financials-general-ledger-api-openapi.yml
- filename: oracle-financials-intercompany-api-openapi.yml
  format: yaml
  label: Oracle Financials Intercompany API
  slug: oracle-financials-intercompany-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-financials/refs/heads/main/openapi/oracle-financials-intercompany-api-openapi.yml
- filename: oracle-financials-ledger-options-api-openapi.yml
  format: yaml
  label: Oracle Financials Ledger Options API
  slug: oracle-financials-ledger-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-financials/refs/heads/main/openapi/oracle-financials-ledger-options-api-openapi.yml
- filename: oracle-financials-payables-api-openapi.yml
  format: yaml
  label: Oracle Financials Payables API
  slug: oracle-financials-payables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-financials/refs/heads/main/openapi/oracle-financials-payables-api-openapi.yml
- filename: oracle-financials-receivables-api-openapi.yml
  format: yaml
  label: Oracle Financials Receivables API
  slug: oracle-financials-receivables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-financials/refs/heads/main/openapi/oracle-financials-receivables-api-openapi.yml
consequence_counts:
  physical: 1
  read: 21
  safety-critical: 1
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Oracle Financials Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /fscmRestApi/resources/11.13.18.05/budgetaryControlBudgetTransactions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoices
operation_count: 32
overview: 'Oracle Financials exposes 32 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read, 9 write, 1 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Oracle Financials
provider_slug: oracle-financials
slug: oracle-financials-agentic-access
source_filename: oracle-financials-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-24'\nmethod: generated\nsource: openapi/oracle-financial-applications-cash-management-api-openapi.yml, openapi/oracle-financial-applications-fixed-assets-api-openapi.yml,\n  openapi/oracle-financial-applications-general-ledger-api-openapi.yml, openapi/oracle-financial-applications-payables-api-openapi.yml,\n  openapi/oracle-financial-applications-receivables-api-openapi.yml, openapi/oracle-financials-budgetary-control-api-openapi.yml,\n  openapi/oracle-financials-chart-of-accounts-api-openapi.yml, openapi/oracle-financials-currency-rates-api-openapi.yml,\n  openapi/oracle-financials-journal-batches-api-openapi.yml, openapi/oracle-financials-ledger-balances-api-openapi.yml,\n  openapi/oracle-general-ledger-accounting-periods-api-openapi.yml, openapi/oracle-general-ledger-budgetary-control-api-openapi.yml,\n  openapi/oracle-general-ledger-erp-integrations-api-openapi.yml, openapi/oracle-general-ledger-intercompany-api-openapi.yml,\n  openapi/oracle-general-ledger-journal-batches-api-openapi.yml,\
  \ openapi/oracle-general-ledger-ledger-balances-api-openapi.yml,\n  openapi/oracle-general-ledger-ledger-options-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 32\n  by_action_class:\n    connected: 21\n    acting: 11\n  by_consequence:\n    read: 21\n    write: 9\n    physical: 1\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /cashCashBalancesUploads\n  method: get\n  operationId: listCashBalanceUploads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fixedAssets\n  method: get\n  operationId: listFixedAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /journalBatches\n  method: get\n  operationId: listJournalBatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /journalBatches\n  method: post\n  operationId: createJournalBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /journalBatches/{JournalBatchesUniqID}\n  method: get\n  operationId: getJournalBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /journalBatches/{JournalBatchesUniqID}\n  method: patch\n  operationId: updateJournalBatch\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /currencyRates\n  method: get\n  operationId: listCurrencyRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /currencyRates/{currencyRatesUniqID}\n  method: get\n  operationId: getCurrencyRate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoices\n  method: get\n  operationId: listInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoices\n  method: post\n  operationId: createInvoice\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invoices/{InvoiceId}\n  method: get\n  operationId: getInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /receivablesCustomerTransactions\n  method: get\n  operationId: listReceivablesTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fscmRestApi/resources/11.13.18.05/budgetaryControlResults\n  method: get\n  operationId: listBudgetaryControlResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /fscmRestApi/resources/11.13.18.05/budgetaryControlBudgetTransactions\n  method: post\n  operationId: createBudgetTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /fscmRestApi/resources/11.13.18.05/chartOfAccountsFilters\n  method: post\n  operationId: createChartOfAccountsFilter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fscmRestApi/resources/11.13.18.05/currencyRates\n  method: get\n  operationId: listCurrencyRates\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fscmRestApi/resources/11.13.18.05/journalBatches\n  method: get\n  operationId: listJournalBatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fscmRestApi/resources/11.13.18.05/journalBatches/{JeBatchId}\n  method: get\n  operationId: getJournalBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fscmRestApi/resources/11.13.18.05/journalBatches/{JeBatchId}\n  method: patch\n  operationId: updateJournalBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /fscmRestApi/resources/11.13.18.05/journalBatches/{JeBatchId}\n  method: delete\n  operationId: deleteJournalBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fscmRestApi/resources/11.13.18.05/ledgerBalances\n  method: get\n  operationId: listLedgerBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accountingPeriodStatusLOV\n  method: get\n  operationId: listAccountingPeriodStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fedBudgetExecutionControls\n  method: get\n  operationId:\
  \ listBudgetExecutionControls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /erpintegrations\n  method: post\n  operationId: submitErpIntegration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /intercompanyTransactions\n  method: get\n  operationId: listIntercompanyTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /intercompanyTransactions\n  method: post\n  operationId: createIntercompanyTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n  \
  \    max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /journalBatches\n  method: get\n  operationId: listJournalBatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /journalBatches/{JournalBatchesUniqID}\n  method: get\n  operationId: getJournalBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /journalBatches/{JournalBatchesUniqID}\n  method: patch\n  operationId: updateJournalBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /journalBatches/{JournalBatchesUniqID}\n\
  \  method: delete\n  operationId: deleteJournalBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ledgerBalances\n  method: get\n  operationId: listLedgerBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fedLedgerOptions\n  method: get\n  operationId: listLedgerOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-financials/refs/heads/main/agentic-access/oracle-financials-agentic-access.yml
summary_line: 32 operations · 11 acting · 1 human-in-the-loop
tags:
- Accounting
- Accounts Payable
- Accounts Receivable
- Cash Management
- ERP
- Expense Management
- Financial Management
- General Ledger
---
