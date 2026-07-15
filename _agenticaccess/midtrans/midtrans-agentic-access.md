---
acting_count: 21
action_class_counts:
  acting: 21
  connected: 12
api_specs:
- filename: midtrans-openapi.yml
  format: yaml
  label: Midtrans Snap API
  slug: midtrans-snap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/midtrans/refs/heads/main/openapi/midtrans-openapi.yml
- filename: midtrans-openapi.yml
  format: yaml
  label: Midtrans Core API
  slug: midtrans-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/midtrans/refs/heads/main/openapi/midtrans-openapi.yml
- filename: midtrans-openapi.yml
  format: yaml
  label: Midtrans Card Tokenization API
  slug: midtrans-card-tokenization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/midtrans/refs/heads/main/openapi/midtrans-openapi.yml
- filename: midtrans-openapi.yml
  format: yaml
  label: Midtrans GoPay Tokenization API
  slug: midtrans-gopay-tokenization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/midtrans/refs/heads/main/openapi/midtrans-openapi.yml
- filename: midtrans-openapi.yml
  format: yaml
  label: Midtrans Payment Link API
  slug: midtrans-payment-link-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/midtrans/refs/heads/main/openapi/midtrans-openapi.yml
- filename: midtrans-openapi.yml
  format: yaml
  label: Midtrans Subscription API
  slug: midtrans-subscription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/midtrans/refs/heads/main/openapi/midtrans-openapi.yml
- filename: midtrans-openapi.yml
  format: yaml
  label: Midtrans Iris Disbursement API
  slug: midtrans-iris-disbursement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/midtrans/refs/heads/main/openapi/midtrans-openapi.yml
consequence_counts:
  physical: 13
  read: 12
  safety-critical: 1
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Midtrans Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/subscriptions/{subscription_id}/disable
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /iris/api/v1/payouts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /iris/api/v1/payouts/approve
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /iris/api/v1/payouts/reject
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /snap/v1/transactions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/payment-links
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/payment-links/{order_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/charge
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/{order_id}/approve
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/{order_id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/{order_id}/deny
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/{order_id}/expire
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/{order_id}/refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/{order_id}/refund/online/direct
operation_count: 33
overview: 'Midtrans exposes 33 API operations that an AI agent could call, of which 21 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read, 7 write, 13 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Midtrans
provider_slug: midtrans
slug: midtrans-agentic-access
source_filename: midtrans-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/midtrans-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 33\n  by_action_class:\n    acting: 21\n    connected: 12\n  by_consequence:\n    physical: 13\n    read: 12\n    write: 7\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /snap/v1/transactions\n  method: post\n  operationId: createSnapTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/charge\n\
  \  method: post\n  operationId: chargeTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/token\n  method: get\n  operationId: getCardToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/card/register\n  method: get\n  operationId: registerCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/{order_id}/status\n  method: get\n  operationId: getTransactionStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v2/{order_id}/approve\n  method: post\n  operationId: approveTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/{order_id}/deny\n  method: post\n  operationId: denyTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/{order_id}/cancel\n  method: post\n  operationId: cancelTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/{order_id}/expire\n  method: post\n  operationId: expireTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/{order_id}/refund\n  method: post\n  operationId: refundTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/{order_id}/refund/online/direct\n  method: post\n  operationId: directRefundTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/pay/account\n  method: post\n  operationId: createPayAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/pay/account/{account_id}\n  method: get\n  operationId: getPayAccount\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/payment-links\n  method: post\n  operationId: createPaymentLink\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/payment-links/{order_id}\n  method: get\n  operationId: getPaymentLink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/payment-links/{order_id}\n  method: delete\n  operationId: deletePaymentLink\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n  \
  \    purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/subscriptions\n  method: post\n  operationId: createSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/subscriptions/{subscription_id}\n  method: get\n  operationId: getSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/subscriptions/{subscription_id}\n  method: patch\n  operationId: updateSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n   \
  \ escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/subscriptions/{subscription_id}/enable\n  method: post\n  operationId: enableSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/subscriptions/{subscription_id}/disable\n  method: post\n  operationId: disableSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/subscriptions/{subscription_id}/cancel\n  method: post\n  operationId:\
  \ cancelSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iris/api/v1/ping\n  method: get\n  operationId: irisPing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iris/api/v1/beneficiaries\n  method: get\n  operationId: listBeneficiaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iris/api/v1/beneficiaries\n  method: post\n  operationId: createBeneficiary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iris/api/v1/beneficiaries/{alias_name}\n  method: patch\n  operationId: updateBeneficiary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iris/api/v1/payouts\n  method: post\n  operationId: createPayouts\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iris/api/v1/payouts/approve\n  method: post\n  operationId: approvePayouts\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iris/api/v1/payouts/reject\n  method: post\n  operationId: rejectPayouts\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iris/api/v1/payouts/{reference_no}\n  method: get\n  operationId: getPayoutDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iris/api/v1/balance\n  method: get\n  operationId:\
  \ getBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iris/api/v1/bank_accounts\n  method: get\n  operationId: listBankAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iris/api/v1/account_validation\n  method: get\n  operationId: validateBankAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/midtrans/refs/heads/main/agentic-access/midtrans-agentic-access.yml
summary_line: 33 operations · 21 acting · 1 human-in-the-loop
tags:
- Payments
- Payment Gateway
- Indonesia
- Southeast Asia
- Snap
- E-Wallet
- Virtual Account
- Cards
- Bank Transfer
- Fintech
---
