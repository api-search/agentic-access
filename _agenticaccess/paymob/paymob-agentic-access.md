---
acting_count: 32
action_class_counts:
  acting: 32
  connected: 10
api_specs:
- filename: paymob-intentions-api-openapi.yml
  format: yaml
  label: Paymob Intentions API
  slug: paymob-intentions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymob/refs/heads/main/openapi/paymob-intentions-api-openapi.yml
- filename: paymob-accept-api-openapi.yml
  format: yaml
  label: Paymob Accept API
  slug: paymob-accept-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymob/refs/heads/main/openapi/paymob-accept-api-openapi.yml
- filename: paymob-subscriptions-api-openapi.yml
  format: yaml
  label: Paymob Subscriptions API
  slug: paymob-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymob/refs/heads/main/openapi/paymob-subscriptions-api-openapi.yml
- filename: paymob-card-tokens-api-openapi.yml
  format: yaml
  label: Paymob Card Tokens API
  slug: paymob-card-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymob/refs/heads/main/openapi/paymob-card-tokens-api-openapi.yml
- filename: paymob-payouts-api-openapi.yml
  format: yaml
  label: Paymob Payouts (Send) API
  slug: paymob-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymob/refs/heads/main/openapi/paymob-payouts-api-openapi.yml
consequence_counts:
  physical: 14
  read: 10
  write: 18
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
  path: /api/acceptance/capture
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/acceptance/payment_keys
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/acceptance/payments/cit
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/acceptance/payments/mit
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
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/intentions/confirm/
operation_count: 42
overview: 'Paymob exposes 42 API operations that an AI agent could call, of which 32 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read, 18 write, and 14 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Paymob
provider_slug: paymob
slug: paymob-agentic-access
source_filename: paymob-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/paymob-accept-api-openapi.yml, openapi/paymob-card-tokens-api-openapi.yml, openapi/paymob-intentions-api-openapi.yml,\n  openapi/paymob-payouts-api-openapi.yml, openapi/paymob-subscriptions-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 42\n  by_action_class:\n    acting: 32\n    connected: 10\n  by_consequence:\n    write: 18\n    physical: 14\n    read: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /api/auth/tokens\n  method: post\n  operationId: createAuthToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/ecommerce/orders\n  method: post\n  operationId: registerOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/acceptance/payment_keys\n  method: post\n  operationId: requestPaymentKey\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/acceptance/payments/pay\n  method: post\n  operationId: payWithPaymentMethod\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/acceptance/capture\n  method: post\n  operationId: captureTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/acceptance/void_refund/void\n  method: post\n  operationId: voidTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/acceptance/void_refund/refund\n  method: post\n  operationId: refundTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/acceptance/transactions/{transaction_id}\n  method: get\n  operationId: retrieveTransactionById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ecommerce/orders/transaction_inquiry\n  method: post\n  operationId: transactionInquiryByOrderId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/ecommerce/payment-links\n  method: post\n  operationId: createPaymentLink\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/ecommerce/payment-links/cancel\n  method: post\n  operationId: cancelPaymentLink\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/acceptance/card_tokens\n  method: get\n  operationId: listCardTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/acceptance/card_tokens/{token_id}\n  method: delete\n  operationId: deleteCardToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/acceptance/payments/cit\n  method: post\n  operationId: customerInitiatedTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/acceptance/payments/mit\n  method: post\n  operationId: merchantInitiatedTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/intention/\n  method: post\n  operationId: createIntention\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/intention/{client_secret}\n  method: put\n  operationId: updateIntention\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/intention/element/{public_key}/{client_secret}/\n  method: get\n  operationId: retrieveIntention\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/intentions/confirm/\n  method: post\n  operationId: confirmIntention\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /unifiedcheckout/\n  method: get\n  operationId: launchUnifiedCheckout\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/auth/token/\n  method: post\n  operationId: generatePayoutsToken\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/token/refresh/\n  method: post\n  operationId: refreshPayoutsToken\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /disburse/api/v1/disburse/instant_cashin/\n\
  \  method: post\n  operationId: instantCashin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /disburse/api/v1/disburse/bulk_transaction/\n  method: post\n  operationId: bulkDisbursement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /disburse/api/v1/budget/inquire/\n  method: get\n  operationId: budgetInquiry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /disburse/api/v1/topup/request/\n  method: post\n  operationId:\
  \ topupRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /disburse/api/v1/topup/inquire/\n  method: post\n  operationId: topupInquiry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /disburse/api/v1/bulk_transaction/inquire/\n  method: post\n  operationId: bulkTransactionInquiry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /disburse/api/v1/bulk_transaction/inquire_by_reference/\n  method: post\n  operationId: bulkTransactionInquiryByReference\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/acceptance/subscription-plans\n  method: post\n  operationId: createSubscriptionPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/acceptance/subscription-plans\n  method: get\n  operationId: listSubscriptionPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n   \
  \ subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/acceptance/subscription-plans/{subscription_plan_id}\n  method: put\n  operationId: updateSubscriptionPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/acceptance/subscription-plans/{subscription_plan_id}/suspend\n  method: post\n  operationId: suspendSubscriptionPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/acceptance/subscription-plans/{subscription_plan_id}/resume\n  method: post\n  operationId: resumeSubscriptionPlan\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/acceptance/subscriptions/{subscription_id}\n  method: get\n  operationId: retrieveSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/acceptance/subscriptions/{subscription_id}\n  method: put\n  operationId: updateSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/acceptance/subscriptions/{subscription_id}/suspend\n  method: post\n \
  \ operationId: suspendSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/acceptance/subscriptions/{subscription_id}/resume\n  method: post\n  operationId: resumeSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/acceptance/subscriptions/{subscription_id}/cancel\n  method: post\n  operationId: cancelSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/acceptance/subscriptions/{subscription_id}/last-transaction\n  method: get\n  operationId: getLastSubscriptionTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/acceptance/subscriptions/{subscription_id}/transactions\n  method: get\n  operationId: listSubscriptionTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/acceptance/subscriptions/{subscription_id}/card-tokens\n  method: get\n  operationId: listSubscriptionCardTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paymob/refs/heads/main/agentic-access/paymob-agentic-access.yml
summary_line: 42 operations · 32 acting
tags:
- Payments
- Payment Gateway
- Fintech
- MENA
- MENAP
- Egypt
- Saudi Arabia
- UAE
- Pakistan
- Oman
- Card Payments
- Mobile Wallets
- BNPL
- Payouts
- Subscriptions
---
