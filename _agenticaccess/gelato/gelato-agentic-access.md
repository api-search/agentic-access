---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 10
api_specs:
- filename: gelato-openapi.yml
  format: yaml
  label: Gelato Orders API
  slug: gelato-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gelato/refs/heads/main/openapi/gelato-openapi.yml
- filename: gelato-openapi.yml
  format: yaml
  label: Gelato Product Catalog API
  slug: gelato-product-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gelato/refs/heads/main/openapi/gelato-openapi.yml
- filename: gelato-openapi.yml
  format: yaml
  label: Gelato Prices and Stock API
  slug: gelato-prices-stock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gelato/refs/heads/main/openapi/gelato-openapi.yml
- filename: gelato-openapi.yml
  format: yaml
  label: Gelato Shipment API
  slug: gelato-shipment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gelato/refs/heads/main/openapi/gelato-openapi.yml
- filename: gelato-openapi.yml
  format: yaml
  label: Gelato Ecommerce API
  slug: gelato-ecommerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gelato/refs/heads/main/openapi/gelato-openapi.yml
- filename: gelato-openapi.yml
  format: yaml
  label: Gelato Webhooks API
  slug: gelato-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gelato/refs/heads/main/openapi/gelato-openapi.yml
consequence_counts:
  physical: 5
  read: 10
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Gelato Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v4/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v4/orders/{orderId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v4/orders/{orderId}:cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v4/orders:quote
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v4/orders:search
operation_count: 18
overview: 'Gelato exposes 18 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read, 3 write, and 5 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Gelato
provider_slug: gelato
slug: gelato-agentic-access
source_filename: gelato-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/gelato-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    acting: 8\n    connected: 10\n  by_consequence:\n    physical: 5\n    read: 10\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /v4/orders\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v4/orders:search\n  method: post\n  operationId: searchOrders\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v4/orders:quote\n  method: post\n  operationId: quoteOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v4/orders/{orderId}\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/orders/{orderId}\n  method: patch\n  operationId:\
  \ patchDraftOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v4/orders/{orderId}:cancel\n  method: post\n  operationId: cancelOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/catalogs\n  method: get\n  operationId: listCatalogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/catalogs/{catalogUid}\n\
  \  method: get\n  operationId: getCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/catalogs/{catalogUid}/products:search\n  method: post\n  operationId: searchProducts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/products/{productUid}\n  method: get\n  operationId: getProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/products/{productUid}/cover-dimensions\n  method: get\n  operationId: getCoverDimensions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n  \
  \    max-ttl: 3600\n    audit: none\n- path: /v3/products/{productUid}/prices\n  method: get\n  operationId: getProductPrices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/stock/region-availability\n  method: post\n  operationId: getStockRegionAvailability\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/shipment-methods\n  method: get\n  operationId: listShipmentMethods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stores/{storeId}/products\n  method: get\n  operationId: listStoreProducts\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stores/{storeId}/products/{productId}\n  method: get\n  operationId: getStoreProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stores/{storeId}/products:create-from-template\n  method: post\n  operationId: createProductFromTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/templates/{templateId}\n  method: get\n  operationId: getTemplate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gelato/refs/heads/main/agentic-access/gelato-agentic-access.yml
summary_line: 18 operations · 8 acting
tags:
- Print on Demand
- Ecommerce
- Fulfillment
- Distributed Production
- Orders
---
