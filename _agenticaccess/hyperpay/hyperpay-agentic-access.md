---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 3
api_specs:
- filename: hyperpay-openapi.yml
  format: yaml
  label: HyperPay COPYandPAY API
  slug: hyperpay-copyandpay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperpay/refs/heads/main/openapi/hyperpay-openapi.yml
- filename: hyperpay-openapi.yml
  format: yaml
  label: HyperPay Server-to-Server Payments API
  slug: hyperpay-server-to-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperpay/refs/heads/main/openapi/hyperpay-openapi.yml
- filename: hyperpay-openapi.yml
  format: yaml
  label: HyperPay Registration Tokens API
  slug: hyperpay-registration-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperpay/refs/heads/main/openapi/hyperpay-openapi.yml
- filename: hyperpay-openapi.yml
  format: yaml
  label: HyperPay Query API
  slug: hyperpay-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperpay/refs/heads/main/openapi/hyperpay-openapi.yml
consequence_counts:
  read: 3
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. Payment operations move money and MUST default to human-in-the-loop. See research/curity/agentic-governance/.
human_in_the_loop: 5
kind: agentic-access
layout: agentic-access
method: generated
name: Hyperpay Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'HyperPay exposes 9 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 6 write.


  5 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: HyperPay
provider_slug: hyperpay
slug: hyperpay-agentic-access
source_filename: hyperpay-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: generated\nsource: openapi/hyperpay-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. Payment operations move money and MUST default to human-in-the-loop.\n  See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    acting: 6\n    connected: 3\n  by_consequence:\n    write: 6\n    read: 3\n  human_in_the_loop_required: 5\noperations:\n- path: /v1/checkouts\n  method: post\n  operationId: createCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - money-movement\n      - high-value\n    audit: required\n- path: /v1/checkouts/{id}/payment\n  method: get\n\
  \  operationId: getCheckoutStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/payments\n  method: post\n  operationId: createPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - money-movement\n      - card-data\n      - high-value\n    audit: required\n- path: /v1/payments/{id}\n  method: post\n  operationId: managePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - money-movement\n      - refund\n      - reversal\n    audit: required\n- path: /v1/registrations\n  method: post\n  operationId: createRegistration\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - card-data\n      - tokenization\n    audit: required\n- path: /v1/registrations/{id}\n  method: get\n  operationId: getRegistration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: required\n- path: /v1/registrations/{id}\n  method: delete\n  operationId: deleteRegistration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    audit: required\n- path: /v1/registrations/{id}/payments\n  method: post\n  operationId: createRegistrationPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n \
  \   subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - money-movement\n      - recurring\n      - high-value\n    audit: required\n- path: /v1/query/{id}\n  method: get\n  operationId: queryPayment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hyperpay/refs/heads/main/agentic-access/hyperpay-agentic-access.yml
summary_line: 9 operations · 6 acting · 5 human-in-the-loop
tags:
- Payments
- Payment Gateway
- Fintech
- MENA
- Saudi Arabia
- mada
- Apple Pay
- Cards
---
