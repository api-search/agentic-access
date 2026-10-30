---
acting_count: 4
action_class_counts:
  acting: 4
api_specs:
- filename: outpost-ai-oauth-api-openapi.yml
  format: yaml
  label: Outpost OAuth API
  slug: outpost-ai-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outpost-ai/openapi/outpost-ai-oauth-api-openapi.yml
- filename: outpost-ai-payments-api-openapi.yml
  format: yaml
  label: Outpost Payments API
  slug: outpost-ai-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outpost-ai/openapi/outpost-ai-payments-api-openapi.yml
- filename: outpost-ai-webhooks-api-openapi.yml
  format: yaml
  label: Outpost Webhooks API
  slug: outpost-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outpost-ai/openapi/outpost-ai-webhooks-api-openapi.yml
consequence_counts:
  physical: 3
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Outpost Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/payments/stripe/payment-intents
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/payments/stripe/setup-intents
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/payments/{paymentId}/refund
operation_count: 4
overview: 'Outpost exposes 4 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 write and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Outpost
provider_slug: outpost-ai
slug: outpost-ai-agentic-access
source_filename: outpost-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/stripe-billing-mor.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    acting: 4\n  by_consequence:\n    write: 1\n    physical: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /oauth/token\n  method: post\n  operationId: createAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/payments/stripe/setup-intents\n  method: post\n  operationId: createSetupIntent\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/payments/stripe/payment-intents\n  method: post\n  operationId: createPaymentIntent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/payments/{paymentId}/refund\n  method: post\n  operationId: refundPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/outpost-ai/agentic-access/outpost-ai-agentic-access.yml
summary_line: 4 operations · 4 acting
tags:
- Company
- Commerce
- Payments
- Tax
- Invoicing
- API
---
