---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 2
api_specs:
- filename: carry1st-pay1st-gateway-openapi.yml
  format: yaml
  label: Pay1st Gateway API
  slug: pay1st-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carry1st/refs/heads/main/openapi/carry1st-pay1st-gateway-openapi.yml
consequence_counts:
  physical: 2
  read: 2
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Carry1St Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/pay1st/payments/create
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/pay1st/transactions/refunds/create
operation_count: 6
overview: 'Carry1st exposes 6 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read, 2 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Carry1st
provider_slug: carry1st
slug: carry1st-agentic-access
source_filename: carry1st-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/carry1st-pay1st-gateway-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    acting: 4\n    connected: 2\n  by_consequence:\n    write: 2\n    read: 2\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/pay1st/auth/token\n  method: post\n  operationId: generateAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/pay1st/auth/refresh\n  method: post\n  operationId: refreshAccessToken\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/pay1st/payments/methods\n  method: get\n  operationId: listPaymentMethods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/pay1st/payments/create\n  method: post\n  operationId: createPaymentRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/pay1st/payments\n  method: get\n  operationId: queryPaymentStatus\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/pay1st/transactions/refunds/create\n  method: post\n  operationId: createRefundRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carry1st/refs/heads/main/agentic-access/carry1st-agentic-access.yml
summary_line: 6 operations · 4 acting
tags:
- Company
- Payments
- Payment Gateway
- Fintech
- Gaming
- Mobile Games
- Africa
- Digital Commerce
- Merchant of Record
- Games Publishing
---
