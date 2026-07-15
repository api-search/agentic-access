---
acting_count: 5
action_class_counts:
  acting: 5
api_specs:
- filename: opay-cashier-api-openapi.yml
  format: yaml
  label: OPay Cashier API
  slug: opay-cashier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opay/refs/heads/main/openapi/opay-cashier-api-openapi.yml
consequence_counts:
  physical: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Opay Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /cashier/create
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /cashier/status
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment/create
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment/refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment/refund/status
operation_count: 5
overview: 'OPay exposes 5 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: OPay
provider_slug: opay
slug: opay-agentic-access
source_filename: opay-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/opay-cashier-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    acting: 5\n  by_consequence:\n    physical: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /cashier/create\n  method: post\n  operationId: createCashierPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cashier/status\n  method: post\n  operationId: queryPaymentStatus\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment/create\n  method: post\n  operationId: createPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment/refund\n  method: post\n  operationId: refundPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment/refund/status\n  method: post\n  operationId: queryRefundStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opay/refs/heads/main/agentic-access/opay-agentic-access.yml
summary_line: 5 operations · 5 acting
tags:
- Payments
- Mobile Money
- Fintech
- Super App
- Nigeria
- Africa
- Wallet
- Savings
- BNPL
- Bank Transfer
- Card Payments
- USSD
- Agent Banking
- POS
- Bill Payments
- Airtime
- Cashier
- Checkout
- Merchant Acquiring
---
