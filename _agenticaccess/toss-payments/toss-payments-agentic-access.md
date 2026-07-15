---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 6
api_specs:
- filename: toss-payments-openapi.yml
  format: yaml
  label: Toss Payments Payments API
  slug: toss-payments-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toss-payments/refs/heads/main/openapi/toss-payments-openapi.yml
- filename: toss-payments-openapi.yml
  format: yaml
  label: Toss Payments Billing API
  slug: toss-payments-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toss-payments/refs/heads/main/openapi/toss-payments-openapi.yml
- filename: toss-payments-openapi.yml
  format: yaml
  label: Toss Payments Virtual Accounts API
  slug: toss-payments-virtual-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toss-payments/refs/heads/main/openapi/toss-payments-openapi.yml
- filename: toss-payments-openapi.yml
  format: yaml
  label: Toss Payments Cash Receipts API
  slug: toss-payments-cash-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toss-payments/refs/heads/main/openapi/toss-payments-openapi.yml
- filename: toss-payments-openapi.yml
  format: yaml
  label: Toss Payments Transactions API
  slug: toss-payments-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toss-payments/refs/heads/main/openapi/toss-payments-openapi.yml
- filename: toss-payments-openapi.yml
  format: yaml
  label: Toss Payments Settlements API
  slug: toss-payments-settlements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toss-payments/refs/heads/main/openapi/toss-payments-openapi.yml
- filename: toss-payments-openapi.yml
  format: yaml
  label: Toss Payments Payouts API
  slug: toss-payments-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toss-payments/refs/heads/main/openapi/toss-payments-openapi.yml
consequence_counts:
  physical: 5
  read: 6
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Toss Payments Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/billing/{billingKey}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/payments/confirm
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/payments/key-in
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/payments/{paymentKey}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/payouts
operation_count: 17
overview: 'Toss Payments exposes 17 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 6 write, and 5 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Toss Payments
provider_slug: toss-payments
slug: toss-payments-agentic-access
source_filename: toss-payments-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/toss-payments-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    acting: 11\n    connected: 6\n  by_consequence:\n    physical: 5\n    read: 6\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/payments/confirm\n  method: post\n  operationId: confirmPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/payments/key-in\n  method: post\n\
  \  operationId: keyInPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/payments/{paymentKey}\n  method: get\n  operationId: getPayment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/payments/orders/{orderId}\n  method: get\n  operationId: getPaymentByOrderId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/payments/{paymentKey}/cancel\n  method: post\n  operationId: cancelPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/authorizations/issue\n  method: post\n  operationId: issueBillingKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/authorizations/card\n  method: post\n  operationId: issueBillingKeyFromCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/{billingKey}\n\
  \  method: post\n  operationId: payWithBillingKey\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/virtual-accounts\n  method: post\n  operationId: createVirtualAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/cash-receipts\n  method: post\n  operationId: issueCashReceipt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/cash-receipts\n  method: get\n  operationId: listCashReceipts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cash-receipts/{receiptKey}/cancel\n  method: post\n  operationId: cancelCashReceipt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transactions\n  method: get\n  operationId: listTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/settlements\n  method: get\n  operationId: listSettlements\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/settlements\n  method: post\n  operationId: requestSettlement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/balances\n  method: get\n  operationId: getPayoutBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/payouts\n  method: post\n  operationId: requestPayouts\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toss-payments/refs/heads/main/agentic-access/toss-payments-agentic-access.yml
summary_line: 17 operations · 11 acting
tags:
- Payments
- Payment Gateway
- South Korea
- Cards
- Easy Pay
- Virtual Account
- Billing
- Checkout
- Fintech
---
