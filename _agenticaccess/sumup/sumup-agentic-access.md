---
acting_count: 19
action_class_counts:
  acting: 19
  connected: 20
api_specs:
- filename: openapi.yaml
  format: yaml
  label: SumUp REST API
  slug: sumup-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/sumup/sumup-openapi/main/openapi.yaml
consequence_counts:
  physical: 7
  read: 20
  safety-critical: 1
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Sumup Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v0.1/merchants/{merchant_code}/readers/{reader_id}/terminate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v0.1/checkouts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v0.1/checkouts/{checkout_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v0.1/checkouts/{checkout_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v0.1/customers/{customer_id}/payment-instruments/{token}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v0.1/merchants/{merchant_code}/readers/{reader_id}/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v0.2/checkouts/{checkout_id}/apple-pay-session
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1.0/merchants/{merchant_code}/payments/{transaction_id}/refunds
operation_count: 39
overview: 'SumUp exposes 39 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 read, 11 write, 7 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SumUp
provider_slug: sumup
slug: sumup-agentic-access
source_filename: sumup-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 39\n  by_action_class:\n    connected: 20\n    acting: 19\n  by_consequence:\n    read: 20\n    physical: 7\n    write: 11\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /v0.1/merchants/{merchant_code}/payment-methods\n  method: get\n  operationId: GetPaymentMethods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/checkouts\n  method: post\n  operationId: CreateCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n  \
  \  - payments\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.1/checkouts\n  method: get\n  operationId: ListCheckouts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - payments\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/checkouts/{checkout_id}\n  method: get\n  operationId: GetCheckout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - payments\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/checkouts/{checkout_id}\n  method: put\n  operationId: ProcessCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.1/checkouts/{checkout_id}\n  method: delete\n  operationId: DeactivateCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - payments\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.2/checkouts/{checkout_id}/apple-pay-session\n  method: put\n  operationId: CreateApplePaySession\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v0.1/customers\n  method: post\n  operationId: CreateCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - payment_instruments\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.1/customers/{customer_id}\n  method: get\n  operationId: GetCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - payment_instruments\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/customers/{customer_id}\n  method: put\n  operationId: UpdateCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - payment_instruments\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.1/customers/{customer_id}/payment-instruments\n  method: get\n  operationId: ListPaymentInstruments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - payment_instruments\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/customers/{customer_id}/payment-instruments/{token}\n  method: delete\n  operationId: DeactivatePaymentInstrument\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - payment_instruments\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1.0/merchants/{merchant_code}/payments/{transaction_id}/refunds\n  method: post\n\
  \  operationId: RefundTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - payments\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2.1/merchants/{merchant_code}/transactions\n  method: get\n  operationId: GetTransactionV2.1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - transactions.history\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2.1/merchants/{merchant_code}/transactions/history\n  method: get\n  operationId: ListTransactionsV2.1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - transactions.history\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.0/merchants/{merchant_code}/payouts\n\
  \  method: get\n  operationId: ListPayoutsV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user.profile\n    - user.profile_readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/receipts/{transaction_id}\n  method: get\n  operationId: GetReceipt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/memberships\n  method: get\n  operationId: ListMemberships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/merchants/{merchant_code}/members\n  method: get\n  operationId: ListMerchantMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/merchants/{merchant_code}/members\n  method:\
  \ post\n  operationId: CreateMerchantMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.1/merchants/{merchant_code}/members/{member_id}\n  method: get\n  operationId: GetMerchantMember\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/merchants/{merchant_code}/members/{member_id}\n  method: put\n  operationId: UpdateMerchantMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.1/merchants/{merchant_code}/members/{member_id}\n\
  \  method: delete\n  operationId: DeleteMerchantMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.1/merchants/{merchant_code}/roles\n  method: get\n  operationId: ListMerchantRoles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/merchants/{merchant_code}/roles\n  method: post\n  operationId: CreateMerchantRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.1/merchants/{merchant_code}/roles/{role_id}\n\
  \  method: get\n  operationId: GetMerchantRole\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/merchants/{merchant_code}/roles/{role_id}\n  method: delete\n  operationId: DeleteMerchantRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.1/merchants/{merchant_code}/roles/{role_id}\n  method: patch\n  operationId: UpdateMerchantRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/merchants/{merchant_code}\n\
  \  method: get\n  operationId: GetMerchant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user.profile\n    - user.profile_readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/merchants/{merchant_code}/persons\n  method: get\n  operationId: ListPersons\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user.profile\n    - user.profile_readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/merchants/{merchant_code}/persons/{person_id}\n  method: get\n  operationId: GetPerson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user.profile\n    - user.profile_readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/merchants/{merchant_code}/readers\n  method: get\n  operationId: ListReaders\n  x-agentic-access:\n    action-class: connected\n  \
  \  consequence: read\n    subject: optional\n    scope:\n    - readers.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/merchants/{merchant_code}/readers\n  method: post\n  operationId: CreateReader\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - readers.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.1/merchants/{merchant_code}/readers/{reader_id}\n  method: get\n  operationId: GetReader\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - readers.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/merchants/{merchant_code}/readers/{reader_id}\n  method: delete\n  operationId: DeleteReader\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    scope:\n    - readers.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.1/merchants/{merchant_code}/readers/{reader_id}\n  method: patch\n  operationId: UpdateReader\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - readers.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.1/merchants/{merchant_code}/readers/{reader_id}/checkout\n  method: post\n  operationId: CreateReaderCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - readers.write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.1/merchants/{merchant_code}/readers/{reader_id}/status\n  method: get\n  operationId: GetReaderStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - readers.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/merchants/{merchant_code}/readers/{reader_id}/terminate\n  method: post\n  operationId: CreateReaderTerminate\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - readers.write\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sumup/refs/heads/main/agentic-access/sumup-agentic-access.yml
summary_line: 39 operations · 19 acting · 1 human-in-the-loop
tags:
- Payments
- POS
- Point of Sale
- Card Readers
- Checkout
- Fintech
- Mobile Payments
- Online Payments
---
