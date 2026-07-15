---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 7
api_specs:
- filename: apicbase-openapi.yml
  format: yaml
  label: Apicbase Ingredients API
  slug: ingredients
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicbase/refs/heads/main/openapi/apicbase-openapi.yml
- filename: apicbase-openapi.yml
  format: yaml
  label: Apicbase Recipes API
  slug: recipes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicbase/refs/heads/main/openapi/apicbase-openapi.yml
- filename: apicbase-openapi.yml
  format: yaml
  label: Apicbase Products API
  slug: products
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicbase/refs/heads/main/openapi/apicbase-openapi.yml
- filename: apicbase-openapi.yml
  format: yaml
  label: Apicbase Inventory & Stock API
  slug: inventory-stock
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicbase/refs/heads/main/openapi/apicbase-openapi.yml
- filename: apicbase-openapi.yml
  format: yaml
  label: Apicbase Purchase Orders API
  slug: purchase-orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicbase/refs/heads/main/openapi/apicbase-openapi.yml
- filename: apicbase-openapi.yml
  format: yaml
  label: Apicbase Suppliers API
  slug: suppliers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicbase/refs/heads/main/openapi/apicbase-openapi.yml
- filename: apicbase-openapi.yml
  format: yaml
  label: Apicbase Outlets API
  slug: outlets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicbase/refs/heads/main/openapi/apicbase-openapi.yml
- filename: apicbase-openapi.yml
  format: yaml
  label: Apicbase Webhooks
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicbase/refs/heads/main/openapi/apicbase-openapi.yml
consequence_counts:
  physical: 1
  read: 7
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Apicbase Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/procurement/purchase_orders/
operation_count: 10
overview: 'Apicbase exposes 10 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read, 2 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Apicbase
provider_slug: apicbase
slug: apicbase-agentic-access
source_filename: apicbase-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/apicbase-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 7\n    acting: 3\n  by_consequence:\n    read: 7\n    write: 2\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v2/products/ingredients/\n  method: get\n  operationId: listIngredients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/products/ingredients/\n  method: post\n  operationId: createIngredient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/products/ingredients/{id}/\n  method: get\n  operationId: getIngredient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/products/recipes/\n  method: get\n  operationId: listRecipes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/products/recipes/\n  method: post\n  operationId: createRecipe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/products/stock_items/\n  method:\
  \ get\n  operationId: listStockItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/procurement/purchase_orders/\n  method: get\n  operationId: listPurchaseOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/procurement/purchase_orders/\n  method: post\n  operationId: createPurchaseOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/suppliers/\n  method: get\n  operationId: listSuppliers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/accounts/outlets/\n  method: get\n  operationId: listOutlets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apicbase/refs/heads/main/agentic-access/apicbase-agentic-access.yml
summary_line: 10 operations · 3 acting
tags:
- Food and Beverage
- Restaurant
- Back of House
- Inventory
- Procurement
- Recipes
---
