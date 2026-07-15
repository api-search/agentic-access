---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 2
api_specs:
- filename: juspay-openapi.yml
  format: yaml
  label: Juspay Orders API
  slug: juspay-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juspay/refs/heads/main/openapi/juspay-openapi.yml
- filename: juspay-openapi.yml
  format: yaml
  label: Juspay Transactions API
  slug: juspay-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juspay/refs/heads/main/openapi/juspay-openapi.yml
- filename: juspay-openapi.yml
  format: yaml
  label: Juspay Session API
  slug: juspay-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juspay/refs/heads/main/openapi/juspay-openapi.yml
- filename: juspay-openapi.yml
  format: yaml
  label: Juspay Refunds API
  slug: juspay-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juspay/refs/heads/main/openapi/juspay-openapi.yml
- filename: juspay-openapi.yml
  format: yaml
  label: Juspay Customers API
  slug: juspay-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juspay/refs/heads/main/openapi/juspay-openapi.yml
consequence_counts:
  physical: 4
  read: 2
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Juspay Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/{order_id}/refunds
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /session
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v4/order-status
operation_count: 8
overview: 'Juspay exposes 8 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read, 2 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Juspay
provider_slug: juspay
slug: juspay-agentic-access
source_filename: juspay-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/juspay-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 6\n    connected: 2\n  by_consequence:\n    physical: 4\n    read: 2\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /orders\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{order_id}\n  method: get\n  operationId: getOrderStatus\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/order-status\n  method: post\n  operationId: getOrderStatusV4\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /txns\n  method: post\n  operationId: createTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /session\n  method: post\n  operationId: createSession\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{order_id}/refunds\n  method: post\n  operationId: createRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers\n  method: post\n  operationId: createCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /customers/{customer_id}\n  method: get\n  operationId: getCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/juspay/refs/heads/main/agentic-access/juspay-agentic-access.yml
summary_line: 8 operations · 6 acting
tags:
- Payments
- Payment Orchestration
- Checkout
- India
- UPI
- Cards
- Payment Gateway
- Fintech
- HyperSDK
- Financial Infrastructure
---
