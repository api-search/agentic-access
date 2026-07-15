---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 5
api_specs:
- filename: shippingeasy-customer-api-openapi.yml
  format: yaml
  label: ShippingEasy Customer API
  slug: shippingeasy-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippingeasy/refs/heads/main/openapi/shippingeasy-customer-api-openapi.yml
consequence_counts:
  physical: 3
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Shippingeasy Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /stores/{store_api_key}/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /stores/{store_api_key}/orders/{external_order_identifier}/status
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /stores/{store_api_key}/orders/{order_number}/cancellations
operation_count: 8
overview: 'ShippingEasy exposes 8 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ShippingEasy
provider_slug: shippingeasy
slug: shippingeasy-agentic-access
source_filename: shippingeasy-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/shippingeasy-customer-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 5\n    acting: 3\n  by_consequence:\n    read: 5\n    physical: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /stores\n  method: get\n  operationId: listStores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders\n  method: get\n  operationId: findOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{id}\n  method: get\n  operationId:\
  \ findOrderById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stores/{store_api_key}/orders\n  method: get\n  operationId: findOrdersByStore\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stores/{store_api_key}/orders\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stores/{store_api_key}/orders/{external_order_identifier}\n  method: get\n  operationId: findOrderByExternalOrderNumber\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stores/{store_api_key}/orders/{external_order_identifier}/status\n  method: put\n  operationId: updateOrderStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stores/{store_api_key}/orders/{order_number}/cancellations\n  method: post\n  operationId: cancelOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shippingeasy/refs/heads/main/agentic-access/shippingeasy-agentic-access.yml
summary_line: 8 operations · 3 acting
tags:
- Shipping
- Logistics
- Multi-Carrier
- Labels
- Order Management
- Ecommerce
- Auctane
- Stamps.com
---
