---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 3
api_specs:
- filename: ziina-openapi.yml
  format: yaml
  label: Ziina Payment Intent API
  slug: ziina-payment-intent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ziina/refs/heads/main/openapi/ziina-openapi.yml
- filename: ziina-openapi.yml
  format: yaml
  label: Ziina Refund API
  slug: ziina-refund-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ziina/refs/heads/main/openapi/ziina-openapi.yml
- filename: ziina-openapi.yml
  format: yaml
  label: Ziina Transfer API
  slug: ziina-transfer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ziina/refs/heads/main/openapi/ziina-openapi.yml
- filename: ziina-openapi.yml
  format: yaml
  label: Ziina Webhooks API
  slug: ziina-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ziina/refs/heads/main/openapi/ziina-openapi.yml
- filename: ziina-openapi.yml
  format: yaml
  label: Ziina Account API
  slug: ziina-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ziina/refs/heads/main/openapi/ziina-openapi.yml
consequence_counts:
  read: 3
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents - review and bind audience per deployment. Ziina moves real money, so write operations carry short token TTLs and human-in-the-loop escalation. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Ziina Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Ziina exposes 8 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 5 write.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Ziina
provider_slug: ziina
slug: ziina-agentic-access
source_filename: ziina-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: generated\nsource: openapi/ziina-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents - review and bind\n  audience per deployment. Ziina moves real money, so write operations carry short token TTLs and\n  human-in-the-loop escalation. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 5\n    connected: 3\n  by_consequence:\n    write: 5\n    read: 3\n  human_in_the_loop_required: 1\noperations:\n- path: /payment_intent\n  method: post\n  operationId: PaymentIntentController_createPaymentIntent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /payment_intent/{id}\n  method: get\n  operationId: PaymentIntentController_getPaymentIntent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /refund\n  method: post\n  operationId: RefundController_initiateRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /refund/{id}\n  method: get\n  operationId: RefundController_getRefund\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transfer\n  method: post\n  operationId: TransferController_initiateTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - money-movement\n      - high-value\n    audit: required\n- path: /transfer/{id}\n  method: get\n  operationId: TransferController_getTransfer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook\n  method: post\n  operationId: WebhookController_createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    audit: required\n- path: /account\n  method: get\n  operationId: AccountController_getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ziina/refs/heads/main/agentic-access/ziina-agentic-access.yml
summary_line: 8 operations · 5 acting · 1 human-in-the-loop
tags:
- Payments
- Fintech
- UAE
- MENA
- Money Transfer
- Wallet
---
