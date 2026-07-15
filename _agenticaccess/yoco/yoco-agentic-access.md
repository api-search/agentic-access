---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 6
api_specs:
- filename: yoco-openapi.yml
  format: yaml
  label: Yoco Checkout API
  slug: yoco-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoco/refs/heads/main/openapi/yoco-openapi.yml
- filename: yoco-openapi.yml
  format: yaml
  label: Yoco Refunds API
  slug: yoco-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoco/refs/heads/main/openapi/yoco-openapi.yml
- filename: yoco-openapi.yml
  format: yaml
  label: Yoco Webhooks API
  slug: yoco-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoco/refs/heads/main/openapi/yoco-openapi.yml
- filename: yoco-openapi.yml
  format: yaml
  label: Yoco Payments API
  slug: yoco-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoco/refs/heads/main/openapi/yoco-openapi.yml
- filename: yoco-openapi.yml
  format: yaml
  label: Yoco Payment Links API
  slug: yoco-payment-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoco/refs/heads/main/openapi/yoco-openapi.yml
consequence_counts:
  physical: 2
  read: 6
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Yoco Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkouts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkouts/{checkoutId}/refund
operation_count: 10
overview: 'Yoco exposes 10 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 2 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Yoco
provider_slug: yoco
slug: yoco-agentic-access
source_filename: yoco-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/yoco-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    acting: 4\n    connected: 6\n  by_consequence:\n    physical: 2\n    read: 6\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /checkouts\n  method: post\n  operationId: createCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /checkouts/{checkoutId}\n  method: get\n  operationId:\
  \ getCheckout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /checkouts/{checkoutId}/refund\n  method: post\n  operationId: refundCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: post\n  operationId: registerWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{webhookId}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/payments\n  method: get\n  operationId: listPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/payments/{paymentId}\n  method: get\n  operationId: getPayment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/refunds/{refundId}\n  method: get\n  operationId: getRefund\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/payment_links/{paymentLinkId}\n  method: get\n  operationId: getPaymentLink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yoco/refs/heads/main/agentic-access/yoco-agentic-access.yml
summary_line: 10 operations · 4 acting
tags:
- Payments
- Fintech
- Payment Gateway
- Card Payments
- South Africa
- Online Payments
- Checkout
- Point of Sale
- SMB
- Financial Infrastructure
---
