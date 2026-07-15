---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 6
api_specs:
- filename: ingram-micro-reseller-api-openapi.yml
  format: yaml
  label: Ingram Micro Reseller API
  slug: reseller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ingram-micro/refs/heads/main/openapi/ingram-micro-reseller-api-openapi.yml
- filename: ingram-micro-vendor-api-openapi.yml
  format: yaml
  label: Ingram Micro Vendor API
  slug: vendor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ingram-micro/refs/heads/main/openapi/ingram-micro-vendor-api-openapi.yml
consequence_counts:
  physical: 1
  read: 6
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ingram Micro Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders
operation_count: 8
overview: 'ingram-micro exposes 8 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 1 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ingram-micro
provider_slug: ingram-micro
slug: ingram-micro-agentic-access
source_filename: ingram-micro-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/ingram-micro-reseller-api-openapi.yml, openapi/ingram-micro-vendor-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 6\n    acting: 2\n  by_consequence:\n    read: 6\n    physical: 1\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /catalog\n  method: get\n  operationId: getCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/{ingramPartNumber}\n  method: get\n  operationId: getProductDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /orders\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{orderId}\n  method: get\n  operationId: getOrderStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pricing\n  method: post\n  operationId: getPricing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inventory\n\
  \  method: get\n  operationId: getInventory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders\n  method: get\n  operationId: getVendorOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shipments\n  method: get\n  operationId: getShipments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ingram-micro/refs/heads/main/agentic-access/ingram-micro-agentic-access.yml
summary_line: 8 operations · 2 acting
tags:
- Fortune 100
---
