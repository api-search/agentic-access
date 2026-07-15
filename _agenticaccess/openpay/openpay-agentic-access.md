---
acting_count: 25
action_class_counts:
  acting: 25
  connected: 23
api_specs:
- filename: openpay-openapi.yml
  format: yaml
  label: Openpay Charges API
  slug: openpay-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpay/refs/heads/main/openapi/openpay-openapi.yml
- filename: openpay-openapi.yml
  format: yaml
  label: Openpay Customers and Cards API
  slug: openpay-customers-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpay/refs/heads/main/openapi/openpay-openapi.yml
- filename: openpay-openapi.yml
  format: yaml
  label: Openpay Subscriptions and Plans API
  slug: openpay-subscriptions-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpay/refs/heads/main/openapi/openpay-openapi.yml
- filename: openpay-openapi.yml
  format: yaml
  label: Openpay Payouts and Transfers API
  slug: openpay-payouts-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpay/refs/heads/main/openapi/openpay-openapi.yml
- filename: openpay-openapi.yml
  format: yaml
  label: Openpay Fees API
  slug: openpay-fees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpay/refs/heads/main/openapi/openpay-openapi.yml
- filename: openpay-openapi.yml
  format: yaml
  label: Openpay Webhooks API
  slug: openpay-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpay/refs/heads/main/openapi/openpay-openapi.yml
consequence_counts:
  physical: 7
  read: 23
  write: 18
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Openpay Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{merchant_id}/charges
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{merchant_id}/charges/{transaction_id}/capture
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{merchant_id}/charges/{transaction_id}/refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{merchant_id}/customers/{customer_id}/charges
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{merchant_id}/customers/{customer_id}/payouts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{merchant_id}/customers/{customer_id}/transfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{merchant_id}/fees
operation_count: 48
overview: 'Openpay exposes 48 API operations that an AI agent could call, of which 25 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 23 read, 18 write, and 7 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Openpay
provider_slug: openpay
slug: openpay-agentic-access
source_filename: openpay-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openpay-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 48\n  by_action_class:\n    acting: 25\n    connected: 23\n  by_consequence:\n    physical: 7\n    read: 23\n    write: 18\n  human_in_the_loop_required: 0\noperations:\n- path: /{merchant_id}/charges\n  method: post\n  operationId: createMerchantCharge\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{merchant_id}/charges\n  method:\
  \ get\n  operationId: listMerchantCharges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{merchant_id}/charges/{transaction_id}\n  method: get\n  operationId: getMerchantCharge\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{merchant_id}/charges/{transaction_id}/refund\n  method: post\n  operationId: refundMerchantCharge\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{merchant_id}/charges/{transaction_id}/capture\n  method: post\n  operationId: captureMerchantCharge\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{merchant_id}/customers\n  method: post\n  operationId: createCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{merchant_id}/customers\n  method: get\n  operationId: listCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{merchant_id}/customers/{customer_id}\n  method: get\n  operationId: getCustomer\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{merchant_id}/customers/{customer_id}\n  method: put\n  operationId: updateCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{merchant_id}/customers/{customer_id}\n  method: delete\n  operationId: deleteCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{merchant_id}/customers/{customer_id}/charges\n  method: post\n  operationId: createCustomerCharge\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{merchant_id}/customers/{customer_id}/charges\n  method: get\n  operationId: listCustomerCharges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{merchant_id}/cards\n  method: post\n  operationId: createMerchantCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{merchant_id}/cards\n  method: get\n  operationId: listMerchantCards\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{merchant_id}/cards/{card_id}\n  method: get\n  operationId: getMerchantCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{merchant_id}/cards/{card_id}\n  method: delete\n  operationId: deleteMerchantCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{merchant_id}/customers/{customer_id}/cards\n  method: post\n  operationId: createCustomerCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{merchant_id}/customers/{customer_id}/cards\n  method: get\n  operationId: listCustomerCards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{merchant_id}/customers/{customer_id}/cards/{card_id}\n  method: get\n  operationId: getCustomerCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{merchant_id}/customers/{customer_id}/cards/{card_id}\n  method: delete\n  operationId: deleteCustomerCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /{merchant_id}/tokens\n  method: post\n  operationId: createToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{merchant_id}/tokens/{token_id}\n  method: get\n  operationId: getToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{merchant_id}/plans\n  method: post\n  operationId: createPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{merchant_id}/plans\n  method: get\n  operationId:\
  \ listPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{merchant_id}/plans/{plan_id}\n  method: get\n  operationId: getPlan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{merchant_id}/plans/{plan_id}\n  method: put\n  operationId: updatePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{merchant_id}/plans/{plan_id}\n  method: delete\n  operationId: deletePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{merchant_id}/customers/{customer_id}/subscriptions\n  method: post\n  operationId: createSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{merchant_id}/customers/{customer_id}/subscriptions\n  method: get\n  operationId: listSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{merchant_id}/customers/{customer_id}/subscriptions/{subscription_id}\n  method: get\n  operationId: getSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /{merchant_id}/customers/{customer_id}/subscriptions/{subscription_id}\n  method: put\n  operationId: updateSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{merchant_id}/customers/{customer_id}/subscriptions/{subscription_id}\n  method: delete\n  operationId: cancelSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{merchant_id}/customers/{customer_id}/bankaccounts\n  method: post\n  operationId: createBankAccount\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{merchant_id}/customers/{customer_id}/bankaccounts\n  method: get\n  operationId: listBankAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{merchant_id}/customers/{customer_id}/bankaccounts/{bank_account_id}\n  method: get\n  operationId: getBankAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{merchant_id}/customers/{customer_id}/bankaccounts/{bank_account_id}\n  method: delete\n  operationId: deleteBankAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n \
  \     max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{merchant_id}/customers/{customer_id}/payouts\n  method: post\n  operationId: createPayout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{merchant_id}/customers/{customer_id}/payouts\n  method: get\n  operationId: listPayouts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{merchant_id}/customers/{customer_id}/payouts/{payout_id}\n  method: get\n  operationId: getPayout\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{merchant_id}/customers/{customer_id}/transfers\n  method: post\n  operationId: createTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{merchant_id}/customers/{customer_id}/transfers\n  method: get\n  operationId: listTransfers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{merchant_id}/customers/{customer_id}/transfers/{transfer_id}\n  method: get\n  operationId: getTransfer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /{merchant_id}/fees\n  method: post\n  operationId: createFee\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{merchant_id}/fees\n  method: get\n  operationId: listFees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{merchant_id}/webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /{merchant_id}/webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{merchant_id}/webhooks/{webhook_id}\n  method: get\n  operationId: getWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{merchant_id}/webhooks/{webhook_id}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openpay/refs/heads/main/agentic-access/openpay-agentic-access.yml
summary_line: 48 operations · 25 acting
tags:
- Payments
- Fintech
- Cards
- SPEI
- Subscriptions
---
