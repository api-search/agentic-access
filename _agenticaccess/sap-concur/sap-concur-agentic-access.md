---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 12
api_specs:
- filename: expense-report.json
  format: json
  label: Concur Expense API
  slug: concur-expense-api
  spec_type: OpenAPI
  url: https://developer.concur.com/api-reference/expense/expense-report/expense-report.json
- filename: itinerary.json
  format: json
  label: Concur Travel API
  slug: concur-travel-api
  spec_type: OpenAPI
  url: https://developer.concur.com/api-reference/travel/itinerary/itinerary.json
- filename: v3.invoice.json
  format: json
  label: Concur Invoice API
  slug: concur-invoice-api
  spec_type: OpenAPI
  url: https://developer.concur.com/api-reference/invoice/v3.invoice.json
- filename: v4.request.json
  format: json
  label: Concur Request API
  slug: concur-request-api
  spec_type: OpenAPI
  url: https://developer.concur.com/api-reference/request/v4.request.json
consequence_counts:
  physical: 1
  read: 12
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sap Concur Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /expensereports/v4/users/{userID}/context/{contextType}/reports/{reportId}/sendBack
operation_count: 27
overview: 'SAP Concur exposes 27 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read, 14 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SAP Concur
provider_slug: sap-concur
slug: sap-concur-agentic-access
source_filename: sap-concur-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/sap-concur-expense-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 27\n  by_action_class:\n    acting: 15\n    connected: 12\n  by_consequence:\n    write: 14\n    read: 12\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /expensereports/v4/users/{userID}/context/{contextType}/reports\n  method: post\n  operationId: createReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /expensereports/v4/users/{userID}/context/{contextType}/reports/{reportId}\n\
  \  method: get\n  operationId: getReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expensereports/v4/users/{userID}/context/{contextType}/reports/{reportId}\n  method: patch\n  operationId: updateReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /expensereports/v4/reports/{reportId}\n  method: patch\n  operationId: updateSubmittedReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /expensereports/v4/reports/{reportId}\n\
  \  method: delete\n  operationId: deleteReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /expensereports/v4/reports/{reportId}/formFields\n  method: get\n  operationId: getReportFormFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expensereports/v4/users/{userId}/context/{contextType}/reportsToApprove\n  method: get\n  operationId: getReportsToApprove\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expensereports/v4/users/{userID}/context/{contextType}/reports/{reportId}/expenses\n  method: get\n  operationId: getExpenses\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expensereports/v4/users/{userID}/context/{contextType}/reports/{reportId}/expenses/{expenseId}\n  method: get\n  operationId: getExpense\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expensereports/v4/users/{userID}/context/{contextType}/reports/{reportId}/expenses/{expenseId}/itemizations\n  method: get\n  operationId: getExpenseItemizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expensereports/v4/reports/{reportId}/expenses/{expenseId}\n  method: patch\n  operationId: updateSubmittedExpense\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /expensereports/v4/reports/{reportId}/expenses/{expenseId}\n  method: delete\n  operationId: deleteExpense\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /expensereports/v4/reports/{reportId}/expenses/{expenseId}/formFields\n  method: get\n  operationId: getExpenseFormFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expensereports/v4/users/{userID}/context/{contextType}/reports/{reportId}/expenses/{expenseId}/allocations\n  method: get\n  operationId: getAllocations\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expensereports/v4/users/{userID}/context/{contextType}/reports/{reportId}/allocations/{allocationId}\n  method: get\n  operationId: getAllocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expensereports/v4/users/{userID}/context/{contextType}/reports/{reportId}/allocations/{allocationId}\n  method: patch\n  operationId: updateAllocation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /expensereports/v4/users/{userID}/context/{contextType}/reports/{reportId}/comments\n  method: get\n  operationId: getReportComments\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expensereports/v4/users/{userID}/context/{contextType}/reports/{reportId}/comments\n  method: post\n  operationId: createReportComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /expensereports/v4/users/{userID}/context/{contextType}/reports/{reportId}/comments\n  method: put\n  operationId: updateReportComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /expensereports/v4/users/{userID}/context/{contextType}/reports/{reportId}/comments\n\
  \  method: delete\n  operationId: deleteReportComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /expensereports/v4/users/{userID}/context/{contextType}/reports/{reportId}/expenses/{expenseId}/comments\n  method: get\n  operationId: getExpenseComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expensereports/v4/users/{userID}/context/{contextType}/reports/{reportId}/expenses/{expenseId}/comments\n  method: post\n  operationId: createExpenseComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /expensereports/v4/users/{userId}/reports/{reportId}/submit\n  method: patch\n  operationId: submitReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /expensereports/v4/users/{userID}/context/{contextType}/reports/{reportId}/approve\n  method: patch\n  operationId: approveReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /expensereports/v4/users/{userID}/context/{contextType}/reports/{reportId}/sendBack\n  method: patch\n  operationId:\
  \ sendBackReport\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /expensereports/v4/users/{userID}/context/{contextType}/reports/{reportId}/recall\n  method: patch\n  operationId: recallReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /expensereports/v4/users/{userId}/reports/{reportId}/costObjectsForApprover\n  method: get\n  operationId: getCostObjectsForApprover\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-concur/refs/heads/main/agentic-access/sap-concur-agentic-access.yml
summary_line: 27 operations · 15 acting
tags:
- Business Travel
- Expense Management
- Financial Services
- Invoice Management
- Travel Management
---
