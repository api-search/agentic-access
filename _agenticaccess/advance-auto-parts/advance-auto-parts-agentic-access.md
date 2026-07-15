---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 12
api_specs:
- filename: advance-auto-parts-catalog-api-openapi.yml
  format: yaml
  label: Advance Auto Parts Catalog API
  slug: advance-auto-parts-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advance-auto-parts/refs/heads/main/openapi/advance-auto-parts-catalog-api-openapi.yml
- filename: advance-auto-parts-commerce-api-openapi.yml
  format: yaml
  label: Advance Auto Parts Commerce API
  slug: advance-auto-parts-commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advance-auto-parts/refs/heads/main/openapi/advance-auto-parts-commerce-api-openapi.yml
consequence_counts:
  physical: 1
  read: 12
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Advance Auto Parts Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders
operation_count: 14
overview: 'Advance Auto Parts exposes 14 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read, 1 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Advance Auto Parts
provider_slug: advance-auto-parts
slug: advance-auto-parts-agentic-access
source_filename: advance-auto-parts-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/advance-auto-parts-catalog-api-openapi.yml, openapi/advance-auto-parts-commerce-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 12\n    acting: 2\n  by_consequence:\n    read: 12\n    write: 1\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /vehicles/years\n  method: get\n  operationId: getVehicleYears\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vehicles/makes\n  method: get\n  operationId: getVehicleMakes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /vehicles/models\n  method: get\n  operationId: getVehicleModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products\n  method: get\n  operationId: searchProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/{productId}\n  method: get\n  operationId: getProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inventory\n  method: get\n  operationId: checkInventory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stores\n  method: get\n  operationId: getStores\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cart\n  method: get\n  operationId: getCart\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cart\n  method: post\n  operationId: addToCart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders\n  method: get\n  operationId: getOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{orderId}\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /loyalty/account\n  method: get\n  operationId: getLoyaltyAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /loyalty/transactions\n  method: get\n  operationId: getLoyaltyTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/advance-auto-parts/refs/heads/main/agentic-access/advance-auto-parts-agentic-access.yml
summary_line: 14 operations · 2 acting
tags:
- Automotive
- E-Commerce
- Parts Catalog
- Retail
- Supply Chain
- Fortune 500
---
