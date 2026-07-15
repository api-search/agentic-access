---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 20
api_specs:
- filename: printful-openapi.yml
  format: yaml
  label: Printful Catalog API
  slug: catalog
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printful/refs/heads/main/openapi/printful-openapi.yml
- filename: printful-openapi.yml
  format: yaml
  label: Printful Store Products API
  slug: store-products
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printful/refs/heads/main/openapi/printful-openapi.yml
- filename: printful-openapi.yml
  format: yaml
  label: Printful Orders API
  slug: orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printful/refs/heads/main/openapi/printful-openapi.yml
- filename: printful-openapi.yml
  format: yaml
  label: Printful Files API
  slug: files
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printful/refs/heads/main/openapi/printful-openapi.yml
- filename: printful-openapi.yml
  format: yaml
  label: Printful Mockup Generator API
  slug: mockup-generator
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printful/refs/heads/main/openapi/printful-openapi.yml
- filename: printful-openapi.yml
  format: yaml
  label: Printful Shipping Rates API
  slug: shipping-rates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printful/refs/heads/main/openapi/printful-openapi.yml
- filename: printful-openapi.yml
  format: yaml
  label: Printful Warehouse API
  slug: warehouse
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printful/refs/heads/main/openapi/printful-openapi.yml
- filename: printful-openapi.yml
  format: yaml
  label: Printful Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printful/refs/heads/main/openapi/printful-openapi.yml
consequence_counts:
  physical: 6
  read: 20
  safety-critical: 1
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Printful Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v2/webhooks
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/order-estimation-tasks
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v2/orders/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v2/orders/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/orders/{id}/confirm
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/shipping-rates
operation_count: 31
overview: 'Printful exposes 31 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 read, 4 write, 6 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Printful
provider_slug: printful
slug: printful-agentic-access
source_filename: printful-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/printful-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 31\n  by_action_class:\n    connected: 20\n    acting: 11\n  by_consequence:\n    read: 20\n    physical: 6\n    write: 4\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /v2/catalog-products\n  method: get\n  operationId: getCatalogProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/catalog-products/{id}\n  method: get\n  operationId: getCatalogProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v2/catalog-products/{id}/catalog-variants\n  method: get\n  operationId: getCatalogProductVariants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/catalog-variants/{id}\n  method: get\n  operationId: getCatalogVariant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/catalog-products/{id}/prices\n  method: get\n  operationId: getCatalogProductPrices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/catalog-products/{id}/availability\n  method: get\n  operationId: getCatalogProductAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v2/catalog-categories\n  method: get\n  operationId: getCatalogCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/catalog-products/{id}/mockup-styles\n  method: get\n  operationId: getCatalogProductMockupStyles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/catalog-products/{id}/mockup-templates\n  method: get\n  operationId: getCatalogProductMockupTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /store/products\n  method: get\n  operationId: getStoreProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /store/products/{id}\n\
  \  method: get\n  operationId: getStoreProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/orders\n  method: get\n  operationId: getOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/orders\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/orders/{id}\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v2/orders/{id}\n  method: patch\n  operationId: updateOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/orders/{id}\n  method: delete\n  operationId: deleteOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/orders/{id}/confirm\n  method: post\n  operationId: confirmOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/orders/{id}/order-items\n  method: get\n  operationId: getOrderItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/order-estimation-tasks\n  method: post\n  operationId: createOrderEstimationTask\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/files\n  method: post\n  operationId: createFile\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/files/{id}\n  method: get\n  operationId: getFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/mockup-tasks\n  method: get\n  operationId: getMockupTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/mockup-tasks\n  method: post\n  operationId: createMockupTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /v2/shipping-rates\n  method: post\n  operationId: calculateShippingRates\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/warehouse-products\n  method: get\n  operationId: getWarehouseProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/warehouse-products/{id}\n  method: get\n  operationId: getWarehouseProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/webhooks\n  method: get\n  operationId: getWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/webhooks\n  method: post\n  operationId: setWebhooks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/webhooks\n  method: delete\n  operationId: disableWebhooks\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/webhook-events\n  method: get\n  operationId: getWebhookEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n- path: /v2/webhook-events\n  method: post\n  operationId: setWebhookEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/printful/refs/heads/main/agentic-access/printful-agentic-access.yml
summary_line: 31 operations · 11 acting · 1 human-in-the-loop
tags:
- Print on Demand
- Fulfillment
- Ecommerce
- Dropshipping
- Merchandise
---
