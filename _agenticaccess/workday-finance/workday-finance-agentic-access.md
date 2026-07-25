---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 13
api_specs:
- filename: workday-finance-accounts-api-openapi.yml
  format: yaml
  label: Workday Finance Accounts API
  slug: workday-finance-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-finance/refs/heads/main/openapi/workday-finance-accounts-api-openapi.yml
- filename: workday-finance-cost-centers-api-openapi.yml
  format: yaml
  label: Workday Finance Cost Centers API
  slug: workday-finance-cost-centers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-finance/refs/heads/main/openapi/workday-finance-cost-centers-api-openapi.yml
- filename: workday-finance-financial-periods-api-openapi.yml
  format: yaml
  label: Workday Finance Financial Periods API
  slug: workday-finance-financial-periods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-finance/refs/heads/main/openapi/workday-finance-financial-periods-api-openapi.yml
- filename: workday-finance-journal-entries-api-openapi.yml
  format: yaml
  label: Workday Finance Journal Entries API
  slug: workday-finance-journal-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-finance/refs/heads/main/openapi/workday-finance-journal-entries-api-openapi.yml
- filename: workday-finance-purchase-orders-api-openapi.yml
  format: yaml
  label: Workday Finance Purchase Orders API
  slug: workday-finance-purchase-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-finance/refs/heads/main/openapi/workday-finance-purchase-orders-api-openapi.yml
- filename: workday-finance-requisitions-api-openapi.yml
  format: yaml
  label: Workday Finance Requisitions API
  slug: workday-finance-requisitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-finance/refs/heads/main/openapi/workday-finance-requisitions-api-openapi.yml
- filename: workday-finance-supplier-invoices-api-openapi.yml
  format: yaml
  label: Workday Finance Supplier Invoices API
  slug: workday-finance-supplier-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-finance/refs/heads/main/openapi/workday-finance-supplier-invoices-api-openapi.yml
- filename: workday-finance-suppliers-api-openapi.yml
  format: yaml
  label: Workday Finance Suppliers API
  slug: workday-finance-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-finance/refs/heads/main/openapi/workday-finance-suppliers-api-openapi.yml
- filename: workday-finance-worktags-api-openapi.yml
  format: yaml
  label: Workday Finance Worktags API
  slug: workday-finance-worktags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-finance/refs/heads/main/openapi/workday-finance-worktags-api-openapi.yml
consequence_counts:
  physical: 2
  read: 13
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Workday Finance Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /purchaseOrders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /supplierInvoices
operation_count: 16
overview: 'Workday Finance exposes 16 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read, 1 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Workday Finance
provider_slug: workday-finance
slug: workday-finance-agentic-access
source_filename: workday-finance-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/workday-finance-financial-management-openapi.yml, openapi/workday-finance-procurement-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 13\n    acting: 3\n  by_consequence:\n    read: 13\n    write: 1\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /accounts\n  method: get\n  operationId: listAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /journalEntries\n  method: get\n  operationId: listJournalEntries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /journalEntries\n  method: post\n  operationId: createJournalEntry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /journalEntries/{journalEntryId}\n  method: get\n  operationId: getJournalEntry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /costCenters\n  method: get\n  operationId: listCostCenters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /worktags\n  method: get\n  operationId: listWorktags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /financialPeriods\n  method: get\n  operationId: listFinancialPeriods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /suppliers\n  method: get\n  operationId: listSuppliers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /suppliers/{supplierId}\n  method: get\n  operationId: getSupplier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /purchaseOrders\n  method: get\n  operationId: listPurchaseOrders\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /purchaseOrders\n  method: post\n  operationId: createPurchaseOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /purchaseOrders/{purchaseOrderId}\n  method: get\n  operationId: getPurchaseOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /supplierInvoices\n  method: get\n  operationId: listSupplierInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /supplierInvoices\n  method: post\n  operationId: createSupplierInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /requisitions\n  method: get\n  operationId: listRequisitions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-finance/refs/heads/main/agentic-access/workday-finance-agentic-access.yml
summary_line: 16 operations · 3 acting
tags:
- Accounting
- Cloud
- Enterprise
- ERP
- Finance
- Financial Management
---
