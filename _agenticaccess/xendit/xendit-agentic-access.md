---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 10
api_specs:
- filename: xendit-openapi.yml
  format: yaml
  label: Xendit Payment Requests API
  slug: xendit-payment-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xendit/refs/heads/main/openapi/xendit-openapi.yml
- filename: xendit-openapi.yml
  format: yaml
  label: Xendit Payment Tokens API
  slug: xendit-payment-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xendit/refs/heads/main/openapi/xendit-openapi.yml
- filename: xendit-openapi.yml
  format: yaml
  label: Xendit Invoices API
  slug: xendit-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xendit/refs/heads/main/openapi/xendit-openapi.yml
- filename: xendit-openapi.yml
  format: yaml
  label: Xendit Payouts API
  slug: xendit-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xendit/refs/heads/main/openapi/xendit-openapi.yml
- filename: xendit-openapi.yml
  format: yaml
  label: Xendit Balance API
  slug: xendit-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xendit/refs/heads/main/openapi/xendit-openapi.yml
- filename: xendit-openapi.yml
  format: yaml
  label: Xendit Transactions API
  slug: xendit-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xendit/refs/heads/main/openapi/xendit-openapi.yml
- filename: xendit-openapi.yml
  format: yaml
  label: Xendit Customers API
  slug: xendit-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xendit/refs/heads/main/openapi/xendit-openapi.yml
- filename: xendit-openapi.yml
  format: yaml
  label: Xendit Refunds API
  slug: xendit-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xendit/refs/heads/main/openapi/xendit-openapi.yml
consequence_counts:
  physical: 8
  read: 10
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Xendit Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoices/{invoice_id}/expire!
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /refunds
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/invoices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/payment_requests
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/payment_requests/{payment_request_id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/payment_tokens
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/payouts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/payouts/{payout_id}/cancel
operation_count: 20
overview: 'Xendit exposes 20 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read, 2 write, and 8 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Xendit
provider_slug: xendit
slug: xendit-agentic-access
source_filename: xendit-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/xendit-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    acting: 10\n    connected: 10\n  by_consequence:\n    physical: 8\n    read: 10\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /v3/payment_requests\n  method: post\n  operationId: createPaymentRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/payment_requests/{payment_request_id}\n\
  \  method: get\n  operationId: getPaymentRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/payment_requests/{payment_request_id}/cancel\n  method: post\n  operationId: cancelPaymentRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/payment_tokens\n  method: post\n  operationId: createPaymentToken\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v2/invoices\n  method: post\n  operationId: createInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/invoices\n  method: get\n  operationId: getInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/invoices/{invoice_id}\n  method: get\n  operationId: getInvoiceById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoices/{invoice_id}/expire!\n  method: post\n  operationId: expireInvoice\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/payouts\n  method: post\n  operationId: createPayout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/payouts/{payout_id}\n  method: get\n  operationId: getPayoutById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/payouts/{payout_id}/cancel\n  method: post\n  operationId: cancelPayout\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /balance\n  method: get\n  operationId: getBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions\n  method: get\n  operationId: listTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/{transaction_id}\n  method: get\n  operationId: getTransactionById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /customers\n  method: post\n  operationId: createCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers\n  method: get\n  operationId: getCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customer_id}\n  method: get\n  operationId: getCustomerById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customer_id}\n  method: patch\n  operationId: updateCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /refunds\n  method: post\n  operationId: createRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /refunds/{refund_id}\n  method: get\n  operationId: getRefundById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xendit/refs/heads/main/agentic-access/xendit-agentic-access.yml
summary_line: 20 operations · 10 acting
tags:
- Payments
- Fintech
- Payment Gateway
- Southeast Asia
- Indonesia
- Philippines
- Disbursements
- E-Wallet
- Virtual Accounts
- Cards
- Financial Infrastructure
---
