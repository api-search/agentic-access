---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 2
api_specs:
- filename: geidea-openapi.yml
  format: yaml
  label: Geidea Checkout API
  slug: geidea-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geidea/refs/heads/main/openapi/geidea-openapi.yml
- filename: geidea-openapi.yml
  format: yaml
  label: Geidea Direct API
  slug: geidea-direct-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geidea/refs/heads/main/openapi/geidea-openapi.yml
- filename: geidea-openapi.yml
  format: yaml
  label: Geidea Tokenization API
  slug: geidea-tokenization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geidea/refs/heads/main/openapi/geidea-openapi.yml
- filename: geidea-openapi.yml
  format: yaml
  label: Geidea Transaction Management API
  slug: geidea-transaction-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geidea/refs/heads/main/openapi/geidea-openapi.yml
consequence_counts:
  physical: 4
  read: 2
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Geidea Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment-intent/api/v2/direct/session
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pgw/api/v1/direct/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pgw/api/v2/direct/refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pgw/api/v3/direct/void
operation_count: 10
overview: 'Geidea exposes 10 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read, 4 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Geidea
provider_slug: geidea
slug: geidea-agentic-access
source_filename: geidea-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/geidea-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    acting: 8\n    connected: 2\n  by_consequence:\n    physical: 4\n    write: 4\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /payment-intent/api/v2/direct/session\n  method: post\n  operationId: createSession\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pgw/api/v6/direct/authenticate/initiate\n\
  \  method: post\n  operationId: initiateAuthentication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pgw/api/v6/direct/authenticate/payer\n  method: post\n  operationId: authenticatePayer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pgw/api/v2/direct/pay\n  method: post\n  operationId: pay\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /pgw/api/v1/direct/capture\n  method: post\n  operationId: captureTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pgw/api/v3/direct/void\n  method: post\n  operationId: voidPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pgw/api/v2/direct/refund\n  method: post\n  operationId: refund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n  \
  \  audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pgw/api/v1/direct/cancel\n  method: post\n  operationId: cancelOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pgw/api/v1/direct/order/{orderId}\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pgw/api/v1/direct/token/{tokenId}\n  method: get\n  operationId: retrieveToken\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geidea/refs/heads/main/agentic-access/geidea-agentic-access.yml
summary_line: 10 operations · 8 acting
tags:
- Payments
- Payment Gateway
- Saudi Arabia
- Egypt
- MENA
- mada
- Cards
- POS
- Checkout
- Fintech
---
