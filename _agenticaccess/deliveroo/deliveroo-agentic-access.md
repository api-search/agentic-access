---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 4
api_specs:
- filename: deliveroo-order-api-openapi.yml
  format: yaml
  label: Deliveroo Order API
  slug: order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliveroo/refs/heads/main/openapi/deliveroo-order-api-openapi.yml
- filename: deliveroo-menu-api-openapi.yml
  format: yaml
  label: Deliveroo Menu API
  slug: menu-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliveroo/refs/heads/main/openapi/deliveroo-menu-api-openapi.yml
- filename: deliveroo-site-api-openapi.yml
  format: yaml
  label: Deliveroo Site API
  slug: site-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliveroo/refs/heads/main/openapi/deliveroo-site-api-openapi.yml
- filename: deliveroo-catalogue-api-openapi.yml
  format: yaml
  label: Deliveroo Catalogue API
  slug: catalogue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliveroo/refs/heads/main/openapi/deliveroo-catalogue-api-openapi.yml
- filename: deliveroo-picking-api-openapi.yml
  format: yaml
  label: Deliveroo Picking API
  slug: picking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliveroo/refs/heads/main/openapi/deliveroo-picking-api-openapi.yml
- filename: deliveroo-signature-api-openapi.yml
  format: yaml
  label: Deliveroo Signature API
  slug: signature-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliveroo/refs/heads/main/openapi/deliveroo-signature-api-openapi.yml
consequence_counts:
  physical: 7
  read: 4
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Deliveroo Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /order/v1/orders/{order_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /order/v1/orders/{order_id}/sync_status
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /picking/v1/orders/{order_id}/accept
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /picking/v1/orders/{order_id}/reject
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /picking/v1/orders/{order_id}/start_picking
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /picking/v2/orders/{order_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /signature/v1/orders
operation_count: 15
overview: 'Deliveroo exposes 15 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read, 4 write, and 7 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Deliveroo
provider_slug: deliveroo
slug: deliveroo-agentic-access
source_filename: deliveroo-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/deliveroo-catalogue-api-openapi.yml, openapi/deliveroo-menu-api-openapi.yml,\n  openapi/deliveroo-order-api-openapi.yml, openapi/deliveroo-picking-api-openapi.yml, openapi/deliveroo-signature-api-openapi.yml,\n  openapi/deliveroo-site-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 4\n    acting: 11\n  by_consequence:\n    read: 4\n    write: 4\n    physical: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /brands/{brand_id}/catalogue/{catalogue_id}\n  method: get\n  operationId: getCatalogue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /brands/{brand_id}/catalogue/{catalogue_id}/sites/{site_id}/prices\n  method: put\n  operationId: updatePricesPerSite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /menu/v1/brands/{brand_id}/menus/{id}\n  method: put\n  operationId: uploadMenu\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /menu/v1/brands/{brand_id}/menus/{id}\n  method: get\n  operationId: getMenu\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /order/v1/orders/{order_id}\n  method: patch\n  operationId: updateOrderStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /order/v1/orders/{order_id}/sync_status\n  method: post\n  operationId: createSyncStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /picking/v1/sites/{restaurant_id}/orders/active\n  method: get\n  operationId: getActiveOrders\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /picking/v1/orders/{order_id}/accept\n  method: put\n  operationId: acceptPickingOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /picking/v1/orders/{order_id}/reject\n  method: put\n  operationId: rejectPickingOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /picking/v1/orders/{order_id}/start_picking\n\
  \  method: put\n  operationId: startPicking\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /picking/v2/orders/{order_id}\n  method: put\n  operationId: updateOrderItems\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /signature/v1/quotes\n  method: post\n  operationId: createQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n   \
  \   max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /signature/v1/orders\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /daas/v1/deliveries\n  method: post\n  operationId: scheduleDelivery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /site/v1/brands/{brand_id}/sites/{site_id}/opening_hours\n  method: get\n  operationId:\
  \ getSiteOpeningHours\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deliveroo/refs/heads/main/agentic-access/deliveroo-agentic-access.yml
summary_line: 15 operations · 11 acting
tags:
- Food Delivery
- Grocery
- Marketplace
- Logistics
- Restaurants
---
