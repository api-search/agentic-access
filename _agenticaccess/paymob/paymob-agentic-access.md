---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 2
api_specs:
- filename: paymob-accounts-api-openapi.yml
  format: yaml
  label: Paymob Accounts API
  slug: paymob-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymob/refs/heads/main/openapi/paymob-accounts-api-openapi.yml
- filename: paymob-authentication-api-openapi.yml
  format: yaml
  label: Paymob Authentication API
  slug: paymob-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymob/refs/heads/main/openapi/paymob-authentication-api-openapi.yml
- filename: paymob-capture-api-openapi.yml
  format: yaml
  label: Paymob Capture API
  slug: paymob-capture-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymob/refs/heads/main/openapi/paymob-capture-api-openapi.yml
- filename: paymob-disbursement-api-openapi.yml
  format: yaml
  label: Paymob Disbursement API
  slug: paymob-disbursement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymob/refs/heads/main/openapi/paymob-disbursement-api-openapi.yml
- filename: paymob-orders-api-openapi.yml
  format: yaml
  label: Paymob Orders API
  slug: paymob-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymob/refs/heads/main/openapi/paymob-orders-api-openapi.yml
- filename: paymob-payment-keys-api-openapi.yml
  format: yaml
  label: Paymob Payment Keys API
  slug: paymob-payment-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymob/refs/heads/main/openapi/paymob-payment-keys-api-openapi.yml
- filename: paymob-payment-links-api-openapi.yml
  format: yaml
  label: Paymob Payment Links API
  slug: paymob-payment-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymob/refs/heads/main/openapi/paymob-payment-links-api-openapi.yml
- filename: paymob-payments-api-openapi.yml
  format: yaml
  label: Paymob Payments API
  slug: paymob-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymob/refs/heads/main/openapi/paymob-payments-api-openapi.yml
- filename: paymob-transactions-api-openapi.yml
  format: yaml
  label: Paymob Transactions API
  slug: paymob-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymob/refs/heads/main/openapi/paymob-transactions-api-openapi.yml
- filename: paymob-top-up-api-openapi.yml
  format: yaml
  label: Paymob Top Up API
  slug: paymob-top-up-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymob/refs/heads/main/openapi/paymob-top-up-api-openapi.yml
consequence_counts:
  physical: 10
  read: 2
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Paymob Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/acceptance/payment_keys
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/acceptance/payments/pay
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/acceptance/void_refund/refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/acceptance/void_refund/void
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/auth/token/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/auth/token/refresh/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/ecommerce/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/ecommerce/orders/transaction_inquiry
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/ecommerce/payment-links
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/ecommerce/payment-links/cancel
operation_count: 20
overview: 'Paymob exposes 20 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read, 8 write, and 10 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Paymob
provider_slug: paymob
slug: paymob-agentic-access
source_filename: paymob-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: generated\nsource: openapi/paymob-accounts-api-openapi.yml, openapi/paymob-authentication-api-openapi.yml,\n  openapi/paymob-capture-api-openapi.yml, openapi/paymob-disbursement-api-openapi.yml, openapi/paymob-orders-api-openapi.yml,\n  openapi/paymob-payment-keys-api-openapi.yml, openapi/paymob-payment-links-api-openapi.yml,\n  openapi/paymob-payments-api-openapi.yml, openapi/paymob-top-up-api-openapi.yml, openapi/paymob-transactions-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    connected: 2\n    acting: 18\n  by_consequence:\n    read: 2\n    write: 8\n    physical: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /disburse/api/v1/budget/inquire/\n  method:\
  \ get\n  operationId: budgetInquiry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/auth/tokens\n  method: post\n  operationId: createAuthToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/token/\n  method: post\n  operationId: generatePayoutsToken\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/token/refresh/\n  method: post\n  operationId:\
  \ refreshPayoutsToken\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/acceptance/capture\n  method: post\n  operationId: captureTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/acceptance/void_refund/void\n  method: post\n  operationId: voidTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/acceptance/void_refund/refund\n  method: post\n  operationId: refundTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /disburse/api/v1/disburse/instant_cashin/\n  method: post\n  operationId: instantCashin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /disburse/api/v1/disburse/bulk_transaction/\n  method:\
  \ post\n  operationId: bulkDisbursement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /disburse/api/v1/bulk_transaction/inquire/\n  method: post\n  operationId: bulkTransactionInquiry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /disburse/api/v1/bulk_transaction/inquire_by_reference/\n  method: post\n  operationId: bulkTransactionInquiryByReference\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n   \
  \   human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/ecommerce/orders\n  method: post\n  operationId: registerOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/acceptance/payment_keys\n  method: post\n  operationId: requestPaymentKey\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/ecommerce/payment-links\n  method: post\n  operationId:\
  \ createPaymentLink\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/ecommerce/payment-links/cancel\n  method: post\n  operationId: cancelPaymentLink\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/acceptance/payments/pay\n  method: post\n  operationId: payWithPaymentMethod\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /disburse/api/v1/topup/request/\n  method: post\n  operationId: topupRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /disburse/api/v1/topup/inquire/\n  method: post\n  operationId: topupInquiry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/acceptance/transactions/{transaction_id}\n  method: get\n\
  \  operationId: retrieveTransactionById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ecommerce/orders/transaction_inquiry\n  method: post\n  operationId: transactionInquiryByOrderId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paymob/refs/heads/main/agentic-access/paymob-agentic-access.yml
summary_line: 20 operations · 18 acting
tags:
- Payments
- Payment Gateway
- Fintech
- MENA
- MENAP
- Egypt
- Saudi Arabia
- United Arab Emirates
- Pakistan
- Oman
- Card Payments
- Mobile Wallets
- Buy Now Pay Later
- Payouts
- Subscription
---
