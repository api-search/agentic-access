---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 6
api_specs:
- filename: abacatepay-openapi.yml
  format: yaml
  label: AbacatePay Billing and Charges API
  slug: abacatepay-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abacatepay/refs/heads/main/openapi/abacatepay-openapi.yml
- filename: abacatepay-openapi.yml
  format: yaml
  label: AbacatePay Pix QR Code API
  slug: abacatepay-pix-qrcode-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abacatepay/refs/heads/main/openapi/abacatepay-openapi.yml
- filename: abacatepay-openapi.yml
  format: yaml
  label: AbacatePay Customers API
  slug: abacatepay-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abacatepay/refs/heads/main/openapi/abacatepay-openapi.yml
- filename: abacatepay-openapi.yml
  format: yaml
  label: AbacatePay Coupons API
  slug: abacatepay-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abacatepay/refs/heads/main/openapi/abacatepay-openapi.yml
- filename: abacatepay-openapi.yml
  format: yaml
  label: AbacatePay Withdraw API
  slug: abacatepay-withdraw-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abacatepay/refs/heads/main/openapi/abacatepay-openapi.yml
consequence_counts:
  physical: 2
  read: 6
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Abacatepay Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pixQrCode/simulate-payment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /withdraw/create
operation_count: 12
overview: 'AbacatePay exposes 12 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 4 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AbacatePay
provider_slug: abacatepay
slug: abacatepay-agentic-access
source_filename: abacatepay-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/abacatepay-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    acting: 6\n    connected: 6\n  by_consequence:\n    write: 4\n    read: 6\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /billing/create\n  method: post\n  operationId: createBilling\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/list\n  method: get\n  operationId: listBillings\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pixQrCode/create\n  method: post\n  operationId: createPixQrCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pixQrCode/check\n  method: get\n  operationId: checkPixQrCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pixQrCode/simulate-payment\n  method: post\n  operationId: simulatePixPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer/create\n  method: post\n  operationId: createCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer/list\n  method: get\n  operationId: listCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coupon/create\n  method: post\n  operationId: createCoupon\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /coupon/list\n  method: get\n  operationId: listCoupons\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /withdraw/create\n  method: post\n  operationId: createWithdraw\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /withdraw/get\n  method: get\n  operationId: getWithdraw\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /withdraw/list\n  method: get\n  operationId: listWithdraws\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abacatepay/refs/heads/main/agentic-access/abacatepay-agentic-access.yml
summary_line: 12 operations · 6 acting
tags:
- Payments
- Pix
- Brazil
- FinTech
- Developers
---
