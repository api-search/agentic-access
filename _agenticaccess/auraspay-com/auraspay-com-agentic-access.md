---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 6
api_specs:
- filename: auraspay-com-account-api-openapi.yml
  format: yaml
  label: AurasPay Account API
  slug: auraspay-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auraspay-com/openapi/auraspay-com-account-api-openapi.yml
- filename: auraspay-com-agent-checkout-api-openapi.yml
  format: yaml
  label: AurasPay Agent Checkout API
  slug: auraspay-com-agent-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auraspay-com/openapi/auraspay-com-agent-checkout-api-openapi.yml
- filename: auraspay-com-payment-links-api-openapi.yml
  format: yaml
  label: AurasPay Payment Links API
  slug: auraspay-com-payment-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auraspay-com/openapi/auraspay-com-payment-links-api-openapi.yml
- filename: auraspay-com-supported-tokens-api-openapi.yml
  format: yaml
  label: AurasPay Supported Tokens API
  slug: auraspay-com-supported-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auraspay-com/openapi/auraspay-com-supported-tokens-api-openapi.yml
consequence_counts:
  physical: 4
  read: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Auraspay Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/payment-links
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/payment-links/{id}/verify
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/x402/payments/{publicId}/prepare
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/x402/payments/{publicId}/proof
operation_count: 10
overview: 'AurasPay exposes 10 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AurasPay
provider_slug: auraspay-com
slug: auraspay-com-agentic-access
source_filename: auraspay-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/auraspay-com-openapi.json, openapi/auraspay-com-x402-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    acting: 4\n    connected: 6\n  by_consequence:\n    physical: 4\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/payment-links\n  method: post\n  operationId: createPaymentLink\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/payment-links\n\
  \  method: get\n  operationId: listPaymentLinks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/payment-links/{id}\n  method: get\n  operationId: getPaymentLink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/payment-links/{id}/verify\n  method: post\n  operationId: verifyPaymentLink\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/account\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/supported-tokens\n  method: get\n  operationId: listSupportedTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/x402/payments/{publicId}\n  method: get\n  operationId: resolveOrSettlePaymentLink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/x402/payments/{publicId}/prepare\n  method: post\n  operationId: preparePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/x402/payments/{publicId}/proof\n\
  \  method: post\n  operationId: submitPaymentProof\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/x402/payments/{publicId}/status\n  method: get\n  operationId: getPaymentStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/auraspay-com/agentic-access/auraspay-com-agentic-access.yml
summary_line: 10 operations · 4 acting
tags:
- Company
- Payments
- Cryptocurrency
- Stablecoins
---
