---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 9
api_specs:
- filename: op-version-latest-get.html
  format: yaml
  label: Oracle ERP Cloud REST API
  slug: oracle-erp-cloud-rest-api
  spec_type: OpenAPI
  url: https://docs.oracle.com/en/cloud/saas/financials/24d/farfa/op-version-latest-get.html
consequence_counts:
  physical: 1
  read: 9
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Oracle Financial Applications Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoices
operation_count: 12
overview: 'Oracle Financial Applications exposes 12 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 2 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Oracle Financial Applications
provider_slug: oracle-financial-applications
slug: oracle-financial-applications-agentic-access
source_filename: oracle-financial-applications-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/oracle-financial-applications-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 9\n    acting: 3\n  by_consequence:\n    read: 9\n    write: 2\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /journalBatches\n  method: get\n  operationId: listJournalBatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /journalBatches\n  method: post\n  operationId: createJournalBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /journalBatches/{JournalBatchesUniqID}\n  method: get\n  operationId: getJournalBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /journalBatches/{JournalBatchesUniqID}\n  method: patch\n  operationId: updateJournalBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /currencyRates\n  method: get\n  operationId: listCurrencyRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /currencyRates/{currencyRatesUniqID}\n\
  \  method: get\n  operationId: getCurrencyRate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoices\n  method: get\n  operationId: listInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoices\n  method: post\n  operationId: createInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invoices/{InvoiceId}\n  method: get\n  operationId: getInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /receivablesCustomerTransactions\n  method: get\n  operationId: listReceivablesTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cashCashBalancesUploads\n  method: get\n  operationId: listCashBalanceUploads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fixedAssets\n  method: get\n  operationId: listFixedAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-financial-applications/refs/heads/main/agentic-access/oracle-financial-applications-agentic-access.yml
summary_line: 12 operations · 3 acting
tags:
- Accounting
- Cloud Applications
- Enterprise Performance Management
- Enterprise Resource Planning
- EPM
- ERP
- Financial Management
- Financial Reporting
---
