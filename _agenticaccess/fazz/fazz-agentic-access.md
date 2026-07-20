---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 5
api_specs:
- filename: fazz-openapi.yml
  format: yaml
  label: Fazz Accept API (Singapore)
  slug: fazz-accept-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fazz/refs/heads/main/openapi/fazz-openapi.yml
- filename: fazz-openapi.yml
  format: yaml
  label: Fazz Send API (Singapore)
  slug: fazz-send-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fazz/refs/heads/main/openapi/fazz-openapi.yml
- filename: fazz-openapi.yml
  format: yaml
  label: Fazz Payment Methods API
  slug: fazz-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fazz/refs/heads/main/openapi/fazz-openapi.yml
consequence_counts:
  read: 5
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/. Note - this API moves real money (payments and disbursements); write operations are high-consequence and should default to human-in-the-loop.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Fazz Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Fazz exposes 8 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 3 write.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Fazz
provider_slug: fazz
slug: fazz-agentic-access
source_filename: fazz-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: generated\nsource: openapi/fazz-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/. Note - this API moves real\n  money (payments and disbursements); write operations are high-consequence and should default\n  to human-in-the-loop.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 3\n    connected: 5\n  by_consequence:\n    write: 3\n    read: 5\n  human_in_the_loop_required: 3\noperations:\n- path: /payments\n  method: post\n  operationId: createPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - money-movement\n      - high-value\n     \
  \ - abnormal\n    audit: required\n- path: /payments\n  method: get\n  operationId: listPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/{paymentId}\n  method: get\n  operationId: getPayment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment_methods/{type}\n  method: post\n  operationId: createPaymentMethod\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment_methods/{paymentMethodId}/payments\n  method: get\n  operationId: listPaymentsForPaymentMethod\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /disbursements\n  method: post\n  operationId: createDisbursement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - money-movement\n      - high-value\n      - abnormal\n    audit: required\n- path: /disbursements\n  method: get\n  operationId: listDisbursements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /disbursements/{disbursementId}\n  method: get\n  operationId: getDisbursement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fazz/refs/heads/main/agentic-access/fazz-agentic-access.yml
summary_line: 8 operations · 3 acting · 3 human-in-the-loop
tags:
- Fintech
- Payments
- Business Banking
- Disbursements
- Southeast Asia
- PayNow
- Virtual Accounts
---
