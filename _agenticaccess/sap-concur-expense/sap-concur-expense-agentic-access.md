---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 12
api_specs:
- filename: sap-concur-expense-report-openapi.yml
  format: yaml
  label: Expense Report v3 API
  slug: expense-report-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-concur-expense/refs/heads/main/openapi/sap-concur-expense-report-openapi.yml
- filename: sap-concur-expense-report-openapi.yml
  format: yaml
  label: Expense Entry v3 API
  slug: expense-entry-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-concur-expense/refs/heads/main/openapi/sap-concur-expense-report-openapi.yml
- filename: sap-concur-expense-report-openapi.yml
  format: yaml
  label: Quick Expense v3 API
  slug: quick-expense-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-concur-expense/refs/heads/main/openapi/sap-concur-expense-report-openapi.yml
- filename: sap-concur-expense-report-openapi.yml
  format: yaml
  label: Receipt Image v3 API
  slug: receipt-image-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-concur-expense/refs/heads/main/openapi/sap-concur-expense-report-openapi.yml
consequence_counts:
  read: 12
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sap Concur Expense Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 23
overview: 'SAP Concur Expense exposes 23 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read and 11 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SAP Concur Expense
provider_slug: sap-concur-expense
slug: sap-concur-expense-agentic-access
source_filename: sap-concur-expense-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/sap-concur-expense-report-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 12\n    acting: 11\n  by_consequence:\n    read: 12\n    write: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /expense/reports\n  method: get\n  operationId: listExpenseReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - expense.report.read\n    - expense.report.write\n- path: /expense/reports\n  method: post\n  operationId: createExpenseReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - expense.report.read\n    - expense.report.write\n- path: /expense/reports/{id}\n  method: get\n  operationId: getExpenseReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - expense.report.read\n    - expense.report.write\n- path: /expense/reports/{id}\n  method: put\n  operationId: updateExpenseReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - expense.report.read\n    - expense.report.write\n- path: /expense/reports/{id}\n\
  \  method: delete\n  operationId: deleteExpenseReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - expense.report.read\n    - expense.report.write\n- path: /expense/entries\n  method: get\n  operationId: listExpenseEntries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - expense.report.read\n    - expense.report.write\n- path: /expense/entries\n  method: post\n  operationId: createExpenseEntry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n    scope:\n    - expense.report.read\n    - expense.report.write\n- path: /expense/entries/{id}\n  method: get\n  operationId: getExpenseEntry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - expense.report.read\n    - expense.report.write\n- path: /expense/entries/{id}\n  method: put\n  operationId: updateExpenseEntry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - expense.report.read\n    - expense.report.write\n- path: /expense/entries/{id}\n  method: delete\n  operationId: deleteExpenseEntry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - expense.report.read\n    - expense.report.write\n- path: /expense/quickexpenses\n  method: get\n  operationId: listQuickExpenses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - expense.report.read\n    - expense.report.write\n- path: /expense/quickexpenses\n  method: post\n  operationId: createQuickExpense\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - expense.report.read\n    - expense.report.write\n- path: /expense/quickexpenses/{id}\n\
  \  method: get\n  operationId: getQuickExpense\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - expense.report.read\n    - expense.report.write\n- path: /expense/quickexpenses/{id}\n  method: put\n  operationId: updateQuickExpense\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - expense.report.read\n    - expense.report.write\n- path: /expense/quickexpenses/{id}\n  method: delete\n  operationId: deleteQuickExpense\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - expense.report.read\n    - expense.report.write\n- path: /expense/receiptimages\n  method: get\n  operationId: listReceiptImages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - expense.report.read\n    - expense.report.write\n- path: /expense/receiptimages\n  method: post\n  operationId: createReceiptImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - expense.report.read\n    - expense.report.write\n- path: /expense/receiptimages/{id}\n  method: get\n  operationId: getReceiptImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - expense.report.read\n    - expense.report.write\n- path: /expense/receiptimages/{id}\n  method: delete\n  operationId: deleteReceiptImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - expense.report.read\n    - expense.report.write\n- path: /expense/allocations\n  method: get\n  operationId: listAllocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - expense.report.read\n    - expense.report.write\n- path: /expense/expensegroupconfigurations\n  method: get\n  operationId: listExpenseGroupConfigurations\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - expense.report.read\n    - expense.report.write\n- path: /expense/expensegroupconfigurations/{id}\n  method: get\n  operationId: getExpenseGroupConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - expense.report.read\n    - expense.report.write\n- path: /expense/paymentbatches\n  method: get\n  operationId: listPaymentBatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - expense.report.read\n    - expense.report.write\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-concur-expense/refs/heads/main/agentic-access/sap-concur-expense-agentic-access.yml
summary_line: 23 operations · 11 acting
tags:
- Expense Management
- Financial Management
- Receipts
- Reimbursement
- Reporting
- SAP
- Travel
---
