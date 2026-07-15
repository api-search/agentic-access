---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 2
api_specs:
- filename: apple-pay-js-openapi.yml
  format: yaml
  label: Apple Pay JS API
  slug: apple-pay-js-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apple-pay/refs/heads/main/openapi/apple-pay-js-openapi.yml
- filename: apple-pay-payment-token-openapi.yml
  format: yaml
  label: Apple Pay Payment Token API
  slug: apple-pay-payment-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apple-pay/refs/heads/main/openapi/apple-pay-payment-token-openapi.yml
consequence_counts:
  physical: 2
  read: 2
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Apple Pay Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /paymentSession
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/apple-pay
operation_count: 6
overview: 'Apple Pay exposes 6 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read, 2 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Apple Pay
provider_slug: apple-pay
slug: apple-pay-agentic-access
source_filename: apple-pay-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/apple-pay-js-openapi.yml, openapi/apple-pay-payment-token-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    acting: 4\n    connected: 2\n  by_consequence:\n    physical: 2\n    write: 2\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /paymentSession\n  method: post\n  operationId: requestPaymentSession\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /registerMerchant\n  method: post\n  operationId: registerMerchant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domains\n  method: get\n  operationId: listMerchantDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domains\n  method: delete\n  operationId: removeMerchantDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/apple-pay\n  method: post\n  operationId: processApplePayPayment\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/apple-pay/{transactionId}\n  method: get\n  operationId: getPaymentStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apple-pay/refs/heads/main/agentic-access/apple-pay-agentic-access.yml
summary_line: 6 operations · 4 acting
tags:
- Apple
- Contactless Payments
- Digital Wallet
- E-Commerce
- Mobile Payments
- Payments
---
