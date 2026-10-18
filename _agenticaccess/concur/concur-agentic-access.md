---
acting_count: 28
action_class_counts:
  acting: 28
  connected: 27
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
- filename: concur-allocations-api-openapi.yml
  format: yaml
  label: SAP Concur Allocations API
  slug: concur-allocations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/concur-allocations-api-openapi.yml
- filename: concur-comments-api-openapi.yml
  format: yaml
  label: SAP Concur Comments API
  slug: concur-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/concur-comments-api-openapi.yml
- filename: concur-expense-entries-api-openapi.yml
  format: yaml
  label: SAP Concur Expense Entries API
  slug: concur-expense-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/concur-expense-entries-api-openapi.yml
- filename: concur-group-configurations-api-openapi.yml
  format: yaml
  label: SAP Concur Group Configurations API
  slug: concur-group-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/concur-group-configurations-api-openapi.yml
- filename: concur-payment-batches-api-openapi.yml
  format: yaml
  label: SAP Concur Payment Batches API
  slug: concur-payment-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/concur-payment-batches-api-openapi.yml
- filename: concur-quick-expenses-api-openapi.yml
  format: yaml
  label: SAP Concur Quick Expenses API
  slug: concur-quick-expenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/concur-quick-expenses-api-openapi.yml
- filename: concur-receipt-images-api-openapi.yml
  format: yaml
  label: SAP Concur Receipt Images API
  slug: concur-receipt-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/concur-receipt-images-api-openapi.yml
- filename: concur-reports-api-openapi.yml
  format: yaml
  label: SAP Concur Reports API
  slug: concur-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/concur-reports-api-openapi.yml
- filename: concur-workflows-api-openapi.yml
  format: yaml
  label: SAP Concur Workflows API
  slug: concur-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/openapi/concur-workflows-api-openapi.yml
consequence_counts:
  physical: 1
  read: 27
  write: 27
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Concur Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /expensereports/v4/users/{userID}/context/{contextType}/reports/{reportId}/sendBack
operation_count: 55
overview: 'SAP Concur exposes 55 API operations that an AI agent could call, of which 28 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 27 read, 27 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SAP Concur
provider_slug: concur
slug: concur-agentic-access
source_filename: concur-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-17'\nmethod: generated\nsource: openapi/concur-allocations-api-openapi.yml, openapi/concur-comments-api-openapi.yml,\n  openapi/concur-expense-entries-api-openapi.yml, openapi/concur-expense-reports-api-openapi.yml,\n  openapi/concur-expenses-api-openapi.yml, openapi/concur-group-configurations-api-openapi.yml,\n  openapi/concur-payment-batches-api-openapi.yml, openapi/concur-quick-expenses-api-openapi.yml,\n  openapi/concur-receipt-images-api-openapi.yml, openapi/concur-reports-api-openapi.yml, openapi/concur-workflows-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 55\n  by_action_class:\n    connected: 27\n    acting: 28\n  by_consequence:\n    read: 27\n    write: 27\n    physical: 1\n  human_in_the_loop_required:\
  \ 0\noperations:\n- path: /expensereports/v4/users/{userID}/context/{contextType}/reports/{reportId}/expenses/{expenseId}/allocations\n  method: get\n  operationId: getAllocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expensereports/v4/users/{userID}/context/{contextType}/reports/{reportId}/allocations/{allocationId}\n  method: get\n  operationId: getAllocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expensereports/v4/users/{userID}/context/{contextType}/reports/{reportId}/allocations/{allocationId}\n  method: patch\n  operationId: updateAllocation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /expense/allocations\n  method: get\n  operationId: listAllocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - expense.report.read\n    - expense.report.write\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expensereports/v4/users/{userID}/context/{contextType}/reports/{reportId}/comments\n  method: get\n  operationId: getReportComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expensereports/v4/users/{userID}/context/{contextType}/reports/{reportId}/comments\n  method: post\n  operationId: createReportComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /expensereports/v4/users/{userID}/context/{contextType}/reports/{reportId}/comments\n  method: put\n  operationId: updateReportComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /expensereports/v4/users/{userID}/context/{contextType}/reports/{reportId}/comments\n  method: delete\n  operationId: deleteReportComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /expensereports/v4/users/{userID}/context/{contextType}/reports/{reportId}/expenses/{expenseId}/comments\n\
  \  method: get\n  operationId: getExpenseComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expensereports/v4/users/{userID}/context/{contextType}/reports/{reportId}/expenses/{expenseId}/comments\n  method: post\n  operationId: createExpenseComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /expense/entries\n  method: get\n  operationId: listExpenseEntries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - expense.report.read\n    - expense.report.write\n- path: /expense/entries\n  method: post\n  operationId: createExpenseEntry\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - expense.report.read\n    - expense.report.write\n- path: /expense/entries/{id}\n  method: get\n  operationId: getExpenseEntry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - expense.report.read\n    - expense.report.write\n- path: /expense/entries/{id}\n  method: put\n  operationId: updateExpenseEntry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n\
  \    - expense.report.read\n    - expense.report.write\n- path: /expense/entries/{id}\n  method: delete\n  operationId: deleteExpenseEntry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - expense.report.read\n    - expense.report.write\n- path: /expensereports/v4/users/{userId}/context/{contextType}/reports\n  method: get\n  operationId: getExpenseReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expensereports/v4/users/{userId}/context/{contextType}/reports\n  method: post\n  operationId: createExpenseReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /expensereports/v4/reports/{reportId}\n  method: get\n  operationId: getExpenseReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expense/reports\n  method: get\n  operationId: listExpenseReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - expense.report.read\n    - expense.report.write\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expense/reports\n  method: post\n  operationId: postExpenseReports\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - expense.report.read\n    - expense.report.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /expense/reports/{id}\n  method: get\n  operationId: getExpenseReportsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - expense.report.read\n    - expense.report.write\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expense/reports/{id}\n  method: put\n  operationId: updateExpenseReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - expense.report.read\n    - expense.report.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /expense/reports/{id}\n  method: delete\n  operationId: deleteExpenseReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n\
  \    - expense.report.read\n    - expense.report.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /expensereports/v4/reports/{reportId}/expenses\n  method: get\n  operationId: getExpenses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expensereports/v4/reports/{reportId}/expenses\n  method: post\n  operationId: createExpense\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /expensereports/v4/users/{userID}/context/{contextType}/reports/{reportId}/expenses\n  method: get\n  operationId: getExpensereportsV4UsersByUserIDContextByContextTypeReportsByReportIdExpenses\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expensereports/v4/users/{userID}/context/{contextType}/reports/{reportId}/expenses/{expenseId}\n  method: get\n  operationId: getExpense\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expensereports/v4/users/{userID}/context/{contextType}/reports/{reportId}/expenses/{expenseId}/itemizations\n  method: get\n  operationId: getExpenseItemizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expensereports/v4/reports/{reportId}/expenses/{expenseId}\n  method: patch\n  operationId: updateSubmittedExpense\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /expensereports/v4/reports/{reportId}/expenses/{expenseId}\n  method: delete\n  operationId: deleteExpense\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /expensereports/v4/reports/{reportId}/expenses/{expenseId}/formFields\n  method: get\n  operationId: getExpenseFormFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expense/expensegroupconfigurations\n  method: get\n  operationId: listExpenseGroupConfigurations\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - expense.report.read\n    - expense.report.write\n- path: /expense/expensegroupconfigurations/{id}\n  method: get\n  operationId: getExpenseGroupConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - expense.report.read\n    - expense.report.write\n- path: /expense/paymentbatches\n  method: get\n  operationId: listPaymentBatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - expense.report.read\n    - expense.report.write\n- path: /expense/quickexpenses\n  method: get\n  operationId: listQuickExpenses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n\
  \    - expense.report.read\n    - expense.report.write\n- path: /expense/quickexpenses\n  method: post\n  operationId: createQuickExpense\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - expense.report.read\n    - expense.report.write\n- path: /expense/quickexpenses/{id}\n  method: get\n  operationId: getQuickExpense\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - expense.report.read\n    - expense.report.write\n- path: /expense/quickexpenses/{id}\n  method: put\n  operationId: updateQuickExpense\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - expense.report.read\n    - expense.report.write\n- path: /expense/quickexpenses/{id}\n  method: delete\n  operationId: deleteQuickExpense\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - expense.report.read\n    - expense.report.write\n- path: /expense/receiptimages\n  method: get\n  operationId: listReceiptImages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - expense.report.read\n    - expense.report.write\n- path: /expense/receiptimages\n  method: post\n  operationId: createReceiptImage\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - expense.report.read\n    - expense.report.write\n- path: /expense/receiptimages/{id}\n  method: get\n  operationId: getReceiptImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - expense.report.read\n    - expense.report.write\n- path: /expense/receiptimages/{id}\n  method: delete\n  operationId: deleteReceiptImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  \    scope:\n    - expense.report.read\n    - expense.report.write\n- path: /expensereports/v4/users/{userID}/context/{contextType}/reports\n  method: post\n  operationId: createReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /expensereports/v4/users/{userID}/context/{contextType}/reports/{reportId}\n  method: get\n  operationId: getReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expensereports/v4/users/{userID}/context/{contextType}/reports/{reportId}\n  method: patch\n  operationId: updateReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /expensereports/v4/reports/{reportId}\n  method: patch\n  operationId: updateSubmittedReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /expensereports/v4/reports/{reportId}\n  method: delete\n  operationId: deleteReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /expensereports/v4/reports/{reportId}/formFields\n  method: get\n  operationId: getReportFormFields\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expensereports/v4/users/{userId}/context/{contextType}/reportsToApprove\n  method: get\n  operationId: getReportsToApprove\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expensereports/v4/users/{userId}/reports/{reportId}/submit\n  method: patch\n  operationId: submitReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /expensereports/v4/users/{userID}/context/{contextType}/reports/{reportId}/approve\n  method: patch\n  operationId: approveReport\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /expensereports/v4/users/{userID}/context/{contextType}/reports/{reportId}/sendBack\n  method: patch\n  operationId: sendBackReport\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /expensereports/v4/users/{userID}/context/{contextType}/reports/{reportId}/recall\n  method: patch\n  operationId: recallReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /expensereports/v4/users/{userId}/reports/{reportId}/costObjectsForApprover\n  method: get\n  operationId: getCostObjectsForApprover\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/concur/refs/heads/main/agentic-access/concur-agentic-access.yml
summary_line: 55 operations · 28 acting
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
