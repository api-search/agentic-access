---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 22
api_specs:
- filename: navan-openapi.yml
  format: yaml
  label: Navan Expense Transactions API
  slug: navan-expense-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navan/refs/heads/main/openapi/navan-openapi.yml
- filename: navan-openapi.yml
  format: yaml
  label: Navan Expense Fees and Adjustments API
  slug: navan-expense-fees-adjustments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navan/refs/heads/main/openapi/navan-openapi.yml
- filename: navan-openapi.yml
  format: yaml
  label: Navan Expense Receipts API
  slug: navan-expense-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navan/refs/heads/main/openapi/navan-openapi.yml
- filename: navan-openapi.yml
  format: yaml
  label: Navan Expense Custom Fields API
  slug: navan-expense-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navan/refs/heads/main/openapi/navan-openapi.yml
- filename: navan-openapi.yml
  format: yaml
  label: Navan Users API
  slug: navan-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navan/refs/heads/main/openapi/navan-openapi.yml
- filename: navan-openapi.yml
  format: yaml
  label: Navan Bookings API
  slug: navan-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navan/refs/heads/main/openapi/navan-openapi.yml
- filename: navan-openapi.yml
  format: yaml
  label: Navan Webhooks API
  slug: navan-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navan/refs/heads/main/openapi/navan-openapi.yml
consequence_counts:
  read: 22
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Navan Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 29
overview: 'Navan exposes 29 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Navan
provider_slug: navan
slug: navan-agentic-access
source_filename: navan-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/navan-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 29\n  by_action_class:\n    connected: 22\n    acting: 7\n  by_consequence:\n    read: 22\n    write: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/expense/transactions\n  method: get\n  operationId: listTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/expense/transactions\n  method: patch\n  operationId: updateTransactions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/expense/transactions/{id}\n  method: get\n  operationId: getTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/expense/card-transactions\n  method: get\n  operationId: listCardTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/expense/connect-transactions\n  method: get\n  operationId: listConnectTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/expense/manual-transactions\n  method: get\n  operationId: listManualTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/expense/repayments\n  method: get\n  operationId: listRepayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/expense/fees\n  method: get\n  operationId: listFees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/expense/adjustments\n  method: get\n  operationId: listAdjustments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/expense/daily-rebates\n  method: get\n  operationId: listDailyRebates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/expense/disputes\n  method: get\n \
  \ operationId: listDisputes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/expense/transactions/{id}/receipt\n  method: get\n  operationId: getTransactionReceipt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/expense/transactions/{id}/receipt/download\n  method: get\n  operationId: downloadTransactionReceipt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/expense/transactions/receipts\n  method: get\n  operationId: listReceipts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/expense/custom-fields\n  method: get\n  operationId: listCustomFields\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/expense/custom-fields/{fieldName}\n  method: get\n  operationId: getCustomField\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/expense/custom-fields/{fieldName}/options\n  method: post\n  operationId: manageCustomFieldOptions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/expense/custom-fields/jobs/{job_id}\n  method: get\n  operationId: getCustomFieldJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /travel/v1/users\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /travel/v1/users\n  method: post\n  operationId: createUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /travel/v1/users/{userId}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /travel/v1/users/{userId}\n  method: patch\n  operationId: updateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /travel/v1/users/{userId}\n  method: delete\n  operationId: deactivateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /travel/v1/bookings\n  method: get\n  operationId: listBookings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /travel/v1/bookings/{bookingId}\n  method: get\n  operationId: getBooking\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/expense/webhooks\n  method: get\n  operationId:\
  \ listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/expense/webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/expense/webhooks/{id}\n  method: get\n  operationId: getWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/expense/webhooks/{id}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/navan/refs/heads/main/agentic-access/navan-agentic-access.yml
summary_line: 29 operations · 7 acting
tags:
- Corporate Travel
- Expense Management
- Corporate Cards
- Spend Management
- T&E
- Fintech
- Business Travel
---
