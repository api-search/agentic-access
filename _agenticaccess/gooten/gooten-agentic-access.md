---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 9
api_specs:
- filename: gooten-openapi.yml
  format: yaml
  label: Gooten Products API
  slug: gooten-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gooten/refs/heads/main/openapi/gooten-openapi.yml
- filename: gooten-openapi.yml
  format: yaml
  label: Gooten Orders API
  slug: gooten-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gooten/refs/heads/main/openapi/gooten-openapi.yml
- filename: gooten-openapi.yml
  format: yaml
  label: Gooten Shipping API
  slug: gooten-shipping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gooten/refs/heads/main/openapi/gooten-openapi.yml
- filename: gooten-openapi.yml
  format: yaml
  label: Gooten Print Assets API
  slug: gooten-print-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gooten/refs/heads/main/openapi/gooten-openapi.yml
consequence_counts:
  physical: 5
  read: 9
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Gooten Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v/5/source/api/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v/5/source/api/price
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/v/5/source/api/shippingAddress
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/v/5/source/api/shippingMethod
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v/5/source/api/shippingprices
operation_count: 17
overview: 'Gooten exposes 17 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 3 write, and 5 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Gooten
provider_slug: gooten
slug: gooten-agentic-access
source_filename: gooten-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/gooten-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    connected: 9\n    acting: 8\n  by_consequence:\n    read: 9\n    physical: 5\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v/5/source/api/products\n  method: get\n  operationId: listProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v/5/source/api/productvariants\n  method: get\n  operationId: listProductVariants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/v/5/source/api/countries\n  method: get\n  operationId: listCountries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v/5/source/api/currencies\n  method: get\n  operationId: listCurrencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v/5/source/api/shippingprices\n  method: post\n  operationId: getShippingOptions\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v/5/source/api/price\n  method: post\n  operationId: getPriceEstimate\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v/5/source/api/orders\n  method: get\n  operationId: getOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v/5/source/api/orders\n  method: post\n  operationId: submitOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v/5/source/api/orderbilling\n  method: get\n\
  \  operationId: getOrderBilling\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v/5/source/api/shippingAddress\n  method: put\n  operationId: updateShippingAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v/5/source/api/shippingMethod\n  method: put\n  operationId: updateShippingMethod\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n   \
  \   - high-value\n    audit: required\n- path: /api/v/5/source/api/producttemplates\n  method: get\n  operationId: listProductTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/recipes/{recipeId}/printreadyproducts\n  method: get\n  operationId: listPrintReadyProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/recipes/{recipeId}/printreadyproducts\n  method: post\n  operationId: createPrintReadyProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/recipes/{recipeId}/printreadyproducts\n  method: put\n  operationId:\
  \ updatePrintReadyProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/recipes/{recipeId}/printreadyproducts/{productId}\n  method: delete\n  operationId: deletePrintReadyProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/recipes/{recipeId}/printreadyproducts/variants\n  method: get\n  operationId: listPrintReadyProductVariants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gooten/refs/heads/main/agentic-access/gooten-agentic-access.yml
summary_line: 17 operations · 8 acting
tags:
- Print on Demand
- Fulfillment
- Manufacturing
- Ecommerce
- Dropshipping
- Custom Products
---
