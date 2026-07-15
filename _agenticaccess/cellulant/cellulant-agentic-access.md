---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 1
api_specs:
- filename: cellulant-checkout-api-openapi.yml
  format: yaml
  label: Cellulant Tingg Checkout API
  slug: cellulant-tingg-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cellulant/refs/heads/main/openapi/cellulant-checkout-api-openapi.yml
- filename: cellulant-payouts-api-openapi.yml
  format: yaml
  label: Cellulant Tingg Payouts API
  slug: cellulant-tingg-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cellulant/refs/heads/main/openapi/cellulant-payouts-api-openapi.yml
- filename: cellulant-engage-api-openapi.yml
  format: yaml
  label: Cellulant Tingg Engage API
  slug: cellulant-tingg-engage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cellulant/refs/heads/main/openapi/cellulant-engage-api-openapi.yml
consequence_counts:
  physical: 6
  read: 1
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cellulant Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/engagement
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/global-api/payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/checkout-api/acknowledgement/request
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/checkout-api/checkout-request/charge
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/checkout-api/checkout-request/custom-request
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/checkout-api/checkout-request/express-request
operation_count: 8
overview: 'Cellulant exposes 8 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read, 1 write, and 6 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cellulant
provider_slug: cellulant
slug: cellulant-agentic-access
source_filename: cellulant-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/cellulant-checkout-api-openapi.yml, openapi/cellulant-engage-api-openapi.yml,\n  openapi/cellulant-payouts-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 7\n    connected: 1\n  by_consequence:\n    write: 1\n    physical: 6\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/oauth/token/request\n  method: post\n  operationId: requestAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v3/checkout-api/checkout-request/express-request\n  method: post\n  operationId: createExpressCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/checkout-api/checkout-request/custom-request\n  method: post\n  operationId: initiateCustomCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/checkout-api/checkout-request/charge\n  method: post\n  operationId: initiateChargeRequest\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/checkout-api/query-status\n  method: get\n  operationId: queryRequestStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/checkout-api/acknowledgement/request\n  method: post\n  operationId: acknowledgePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/engagement\n\
  \  method: post\n  operationId: sendEngagement\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/global-api/payments\n  method: post\n  operationId: postPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cellulant/refs/heads/main/agentic-access/cellulant-agentic-access.yml
summary_line: 8 operations · 7 acting
tags:
- Payments
- Mobile Money
- Checkout
- Payouts
- Disbursement
- Africa
- Pan-African
- Fintech
- Bank Transfer
- Cards
- Airtime
- Bill Payment
- SMS
- OTP
- Tingg
---
