---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 2
api_specs:
- filename: fawrypay-server-api-openapi.yml
  format: yaml
  label: FawryPay Server API
  slug: fawrypay-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fawry/refs/heads/main/openapi/fawrypay-server-api-openapi.yml
consequence_counts:
  physical: 3
  read: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Fawry Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ECommerceWeb/Fawry/payments/charge
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ECommerceWeb/Fawry/payments/refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ECommerceWeb/api/orders/cancel-unpaid-order
operation_count: 5
overview: 'Fawry exposes 5 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Fawry
provider_slug: fawry
slug: fawry-agentic-access
source_filename: fawry-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/fawrypay-server-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    acting: 3\n    connected: 2\n  by_consequence:\n    physical: 3\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /ECommerceWeb/Fawry/payments/charge\n  method: post\n  operationId: createCharge\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ECommerceWeb/Fawry/payments/refund\n\
  \  method: post\n  operationId: refundCharge\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ECommerceWeb/api/orders/cancel-unpaid-order\n  method: post\n  operationId: cancelUnpaidOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ECommerceWeb/Fawry/payments/status/v2\n  method: get\n  operationId: getPaymentStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /ECommerceWeb/api/merchant/installment-plans\n  method: get\n  operationId: listInstallmentPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fawry/refs/heads/main/agentic-access/fawry-agentic-access.yml
summary_line: 5 operations · 3 acting
tags:
- Payments
- E-Payments
- Digital Finance
- Fintech
- Egypt
- Cards
- Wallets
- Bill Payments
- POS
- Micro-Finance
- Installments
- 3D Secure
- Refunds
- Webhooks
- Mobile SDK
- E-Commerce Plugins
- Magento
- Shopify
- WooCommerce
---
