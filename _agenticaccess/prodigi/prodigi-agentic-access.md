---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 4
api_specs:
- filename: prodigi-openapi.yml
  format: yaml
  label: Prodigi Orders API
  slug: prodigi-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prodigi/refs/heads/main/openapi/prodigi-openapi.yml
- filename: prodigi-openapi.yml
  format: yaml
  label: Prodigi Quotes API
  slug: prodigi-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prodigi/refs/heads/main/openapi/prodigi-openapi.yml
- filename: prodigi-openapi.yml
  format: yaml
  label: Prodigi Product Details API
  slug: prodigi-product-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prodigi/refs/heads/main/openapi/prodigi-openapi.yml
- filename: prodigi-openapi.yml
  format: yaml
  label: Prodigi Webhooks / Callbacks
  slug: prodigi-webhooks-callbacks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prodigi/refs/heads/main/openapi/prodigi-openapi.yml
consequence_counts:
  physical: 5
  read: 4
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Prodigi Agentic Access
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
  path: /orders/{orderId}/actions/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/{orderId}/actions/updateMetadata
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/{orderId}/actions/updateRecipient
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/{orderId}/actions/updateShippingMethod
operation_count: 10
overview: 'Prodigi exposes 10 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read, 1 write, and 5 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Prodigi
provider_slug: prodigi
slug: prodigi-agentic-access
source_filename: prodigi-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/prodigi-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    acting: 6\n    connected: 4\n  by_consequence:\n    physical: 5\n    read: 4\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /orders\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders\n  method: get\n  operationId: listOrders\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{orderId}\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{orderId}/actions\n  method: get\n  operationId: getOrderActions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{orderId}/actions/cancel\n  method: post\n  operationId: cancelOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{orderId}/actions/updateShippingMethod\n\
  \  method: post\n  operationId: updateShippingMethod\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{orderId}/actions/updateRecipient\n  method: post\n  operationId: updateRecipient\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{orderId}/actions/updateMetadata\n  method: post\n  operationId: updateMetadata\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /quotes\n  method: post\n  operationId: createQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /products/{sku}\n  method: get\n  operationId: getProductDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prodigi/refs/heads/main/agentic-access/prodigi-agentic-access.yml
summary_line: 10 operations · 6 acting
tags:
- Print on Demand
- Printing
- Dropshipping
- Fulfillment
- E-commerce
---
