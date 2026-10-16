---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 3
api_specs:
- filename: concur-expense-reports-api-openapi.yml
  format: yaml
  label: SAP Concur Expense Reports API
  slug: concur-expense-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/concur-expense-reports-api-openapi.yml
- filename: concur-expenses-api-openapi.yml
  format: yaml
  label: SAP Concur Expenses API
  slug: concur-expenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/concur-expenses-api-openapi.yml
- filename: sap-concur-allocations-api-openapi.yml
  format: yaml
  label: SAP Concur Allocations API
  slug: sap-concur-allocations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/sap-concur-allocations-api-openapi.yml
- filename: sap-concur-comments-api-openapi.yml
  format: yaml
  label: SAP Concur Comments API
  slug: sap-concur-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/sap-concur-comments-api-openapi.yml
- filename: sap-concur-expenses-api-openapi.yml
  format: yaml
  label: SAP Concur Expenses API
  slug: sap-concur-expenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/sap-concur-expenses-api-openapi.yml
- filename: sap-concur-reports-api-openapi.yml
  format: yaml
  label: SAP Concur Reports API
  slug: sap-concur-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/sap-concur-reports-api-openapi.yml
- filename: sap-concur-workflows-api-openapi.yml
  format: yaml
  label: SAP Concur Workflows API
  slug: sap-concur-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/sap-concur-workflows-api-openapi.yml
- filename: sap-concur-expense-allocations-api-openapi.yml
  format: yaml
  label: SAP Concur Expense Allocations API
  slug: sap-concur-expense-allocations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/sap-concur-expense-allocations-api-openapi.yml
- filename: sap-concur-expense-expense-entries-api-openapi.yml
  format: yaml
  label: SAP Concur Expense Entries API
  slug: sap-concur-expense-expense-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/sap-concur-expense-expense-entries-api-openapi.yml
- filename: sap-concur-expense-expense-reports-api-openapi.yml
  format: yaml
  label: SAP Concur Expense Reports API
  slug: sap-concur-expense-expense-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/sap-concur-expense-expense-reports-api-openapi.yml
- filename: sap-concur-expense-group-configurations-api-openapi.yml
  format: yaml
  label: SAP Concur Expense Group Configurations API
  slug: sap-concur-expense-group-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/sap-concur-expense-group-configurations-api-openapi.yml
- filename: sap-concur-expense-payment-batches-api-openapi.yml
  format: yaml
  label: SAP Concur Expense Payment Batches API
  slug: sap-concur-expense-payment-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/sap-concur-expense-payment-batches-api-openapi.yml
- filename: sap-concur-expense-quick-expenses-api-openapi.yml
  format: yaml
  label: SAP Concur Expense Quick Expenses API
  slug: sap-concur-expense-quick-expenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/sap-concur-expense-quick-expenses-api-openapi.yml
- filename: sap-concur-expense-receipt-images-api-openapi.yml
  format: yaml
  label: SAP Concur Expense Receipt Images API
  slug: sap-concur-expense-receipt-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/sap-concur-expense-receipt-images-api-openapi.yml
consequence_counts:
  read: 3
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Concur Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'SAP Concur exposes 5 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SAP Concur
provider_slug: concur
slug: concur-agentic-access
source_filename: concur-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/concur-expense-api.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 3\n    acting: 2\n  by_consequence:\n    read: 3\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /expensereports/v4/users/{userId}/context/{contextType}/reports\n  method: get\n  operationId: getExpenseReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expensereports/v4/users/{userId}/context/{contextType}/reports\n  method: post\n  operationId: createExpenseReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /expensereports/v4/reports/{reportId}\n  method: get\n  operationId: getExpenseReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expensereports/v4/reports/{reportId}/expenses\n  method: get\n  operationId: getExpenses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expensereports/v4/reports/{reportId}/expenses\n  method: post\n  operationId: createExpense\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/agentic-access/concur-agentic-access.yml
summary_line: 5 operations · 2 acting
tags:
- Expense Management
- Finance
- Invoices
- SAP
- Travel
- Business Travel
- Financial Services
- Invoice Management
- Travel Management
- Financial Management
- Receipts
- Reimbursement
- Reporting
---
