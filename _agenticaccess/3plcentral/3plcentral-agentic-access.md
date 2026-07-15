---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 12
api_specs:
- filename: 3plcentral-openapi.yml
  format: yaml
  label: 3PL Warehouse Manager Orders API
  slug: 3plcentral-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/3plcentral/refs/heads/main/openapi/3plcentral-openapi.yml
- filename: 3plcentral-openapi.yml
  format: yaml
  label: 3PL Warehouse Manager Items API
  slug: 3plcentral-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/3plcentral/refs/heads/main/openapi/3plcentral-openapi.yml
- filename: 3plcentral-openapi.yml
  format: yaml
  label: 3PL Warehouse Manager Inventory API
  slug: 3plcentral-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/3plcentral/refs/heads/main/openapi/3plcentral-openapi.yml
- filename: 3plcentral-openapi.yml
  format: yaml
  label: 3PL Warehouse Manager Stock Summaries API
  slug: 3plcentral-stock-summaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/3plcentral/refs/heads/main/openapi/3plcentral-openapi.yml
- filename: 3plcentral-openapi.yml
  format: yaml
  label: 3PL Warehouse Manager Receivers (ASN) API
  slug: 3plcentral-receivers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/3plcentral/refs/heads/main/openapi/3plcentral-openapi.yml
- filename: 3plcentral-openapi.yml
  format: yaml
  label: 3PL Warehouse Manager Customers API
  slug: 3plcentral-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/3plcentral/refs/heads/main/openapi/3plcentral-openapi.yml
- filename: 3plcentral-openapi.yml
  format: yaml
  label: 3PL Warehouse Manager Warehouses API
  slug: 3plcentral-warehouses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/3plcentral/refs/heads/main/openapi/3plcentral-openapi.yml
- filename: 3plcentral-openapi.yml
  format: yaml
  label: 3PL Warehouse Manager Packages API
  slug: 3plcentral-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/3plcentral/refs/heads/main/openapi/3plcentral-openapi.yml
consequence_counts:
  physical: 1
  read: 12
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: 3Plcentral Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders
operation_count: 15
overview: '3PL Warehouse Manager exposes 15 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read, 2 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: 3PL Warehouse Manager
provider_slug: 3plcentral
slug: 3plcentral-agentic-access
source_filename: 3plcentral-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/3plcentral-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    acting: 3\n    connected: 12\n  by_consequence:\n    write: 2\n    read: 12\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /AuthServer/api/Token\n  method: post\n  operationId: getAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers\n  method: get\n  operationId: listCustomers\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customerId}/items\n  method: get\n  operationId: listCustomerItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inventory\n  method: get\n  operationId: getInventory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inventory/stockdetails\n  method: get\n  operationId: getStockDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inventory/stocksummaries\n  method: get\n  operationId: getStockSummaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /inventory/facilities\n  method: get\n  operationId: listFacilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inventory/facilities/{facilityId}/locations\n  method: get\n  operationId: listFacilityLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders\n  method: get\n  operationId: listOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{orderId}\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{orderId}/packages\n  method: get\n  operationId: getOrderPackages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inventory/receivers\n  method: get\n  operationId: listReceivers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inventory/receivers\n  method: post\n  operationId: createReceiver\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inventory/receivers/{receiverId}\n  method: get\n  operationId: getReceiver\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/3plcentral/refs/heads/main/agentic-access/3plcentral-agentic-access.yml
summary_line: 15 operations · 3 acting
tags:
- Warehouse Management
- WMS
- 3PL
- Logistics
- Fulfillment
- Inventory
- Orders
- SecureWMS
- Extensiv
---
