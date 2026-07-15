---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 5
api_specs:
- filename: openapi-general-ledger.yaml
  format: yaml
  label: Oracle Financials General Ledger API
  slug: oracle-financials-general-ledger-api
  spec_type: OpenAPI
  url: https://docs.oracle.com/en/cloud/saas/financials/23r3/farfa/openapi-general-ledger.yaml
- filename: openapi-payables.yaml
  format: yaml
  label: Oracle Financials Accounts Payable API
  slug: oracle-financials-accounts-payable-api
  spec_type: OpenAPI
  url: https://docs.oracle.com/en/cloud/saas/financials/23r3/farfa/openapi-payables.yaml
- filename: openapi-receivables.yaml
  format: yaml
  label: Oracle Financials Accounts Receivable API
  slug: oracle-financials-accounts-receivable-api
  spec_type: OpenAPI
  url: https://docs.oracle.com/en/cloud/saas/financials/23r3/farfa/openapi-receivables.yaml
- filename: openapi-cash-management.yaml
  format: yaml
  label: Oracle Financials Cash Management API
  slug: oracle-financials-cash-management-api
  spec_type: OpenAPI
  url: https://docs.oracle.com/en/cloud/saas/financials/23r3/farfa/openapi-cash-management.yaml
- filename: openapi-expenses.yaml
  format: yaml
  label: Oracle Financials Expense Management API
  slug: oracle-financials-expense-management-api
  spec_type: OpenAPI
  url: https://docs.oracle.com/en/cloud/saas/financials/23r3/farfa/openapi-expenses.yaml
- filename: openapi-fixed-assets.yaml
  format: yaml
  label: Oracle Financials Fixed Assets API
  slug: oracle-financials-fixed-assets-api
  spec_type: OpenAPI
  url: https://docs.oracle.com/en/cloud/saas/financials/23r3/farfa/openapi-fixed-assets.yaml
- filename: openapi-reporting.yaml
  format: yaml
  label: Oracle Financial Reporting API
  slug: oracle-financial-reporting-api
  spec_type: OpenAPI
  url: https://docs.oracle.com/en/cloud/saas/financials/23r3/farfa/openapi-reporting.yaml
consequence_counts:
  read: 5
  safety-critical: 1
  write: 3
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
operation_count: 9
overview: 'Oracle Financials exposes 9 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read, 3 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Oracle Financials
provider_slug: oracle-financials
slug: oracle-financials-agentic-access
source_filename: oracle-financials-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/oracle-financials-general-ledger-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 5\n    acting: 4\n  by_consequence:\n    read: 5\n    write: 3\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /fscmRestApi/resources/11.13.18.05/journalBatches\n  method: get\n  operationId: listJournalBatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fscmRestApi/resources/11.13.18.05/journalBatches/{JeBatchId}\n  method: get\n  operationId: getJournalBatch\n  x-agentic-access:\n    action-class: connected\n  \
  \  consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fscmRestApi/resources/11.13.18.05/journalBatches/{JeBatchId}\n  method: patch\n  operationId: updateJournalBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fscmRestApi/resources/11.13.18.05/journalBatches/{JeBatchId}\n  method: delete\n  operationId: deleteJournalBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fscmRestApi/resources/11.13.18.05/ledgerBalances\n  method: get\n  operationId: listLedgerBalances\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fscmRestApi/resources/11.13.18.05/currencyRates\n  method: get\n  operationId: listCurrencyRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fscmRestApi/resources/11.13.18.05/chartOfAccountsFilters\n  method: post\n  operationId: createChartOfAccountsFilter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fscmRestApi/resources/11.13.18.05/budgetaryControlResults\n  method: get\n  operationId: listBudgetaryControlResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fscmRestApi/resources/11.13.18.05/budgetaryControlBudgetTransactions\n  method: post\n  operationId: createBudgetTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-financials/refs/heads/main/agentic-access/oracle-financials-agentic-access.yml
summary_line: 9 operations · 4 acting · 1 human-in-the-loop
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
