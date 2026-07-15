---
acting_count: 17
action_class_counts:
  acting: 17
  connected: 14
api_specs:
- filename: fulfil-io-openapi.yml
  format: yaml
  label: Fulfil Sales Orders API
  slug: fulfil-io-sales-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulfil-io/refs/heads/main/openapi/fulfil-io-openapi.yml
- filename: fulfil-io-openapi.yml
  format: yaml
  label: Fulfil Products & Variants API
  slug: fulfil-io-products-variants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulfil-io/refs/heads/main/openapi/fulfil-io-openapi.yml
- filename: fulfil-io-openapi.yml
  format: yaml
  label: Fulfil Inventory & Stock API
  slug: fulfil-io-inventory-stock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulfil-io/refs/heads/main/openapi/fulfil-io-openapi.yml
- filename: fulfil-io-openapi.yml
  format: yaml
  label: Fulfil Customers API
  slug: fulfil-io-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulfil-io/refs/heads/main/openapi/fulfil-io-openapi.yml
- filename: fulfil-io-openapi.yml
  format: yaml
  label: Fulfil Shipments API
  slug: fulfil-io-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulfil-io/refs/heads/main/openapi/fulfil-io-openapi.yml
- filename: fulfil-io-openapi.yml
  format: yaml
  label: Fulfil Purchases API
  slug: fulfil-io-purchases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulfil-io/refs/heads/main/openapi/fulfil-io-openapi.yml
- filename: fulfil-io-openapi.yml
  format: yaml
  label: Fulfil Manufacturing API
  slug: fulfil-io-manufacturing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulfil-io/refs/heads/main/openapi/fulfil-io-openapi.yml
- filename: fulfil-io-openapi.yml
  format: yaml
  label: Fulfil Webhooks API
  slug: fulfil-io-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulfil-io/refs/heads/main/openapi/fulfil-io-openapi.yml
- filename: fulfil-io-openapi.yml
  format: yaml
  label: Fulfil Model Interface API
  slug: fulfil-io-model-interface-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulfil-io/refs/heads/main/openapi/fulfil-io-openapi.yml
consequence_counts:
  physical: 4
  read: 14
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Fulfil Io Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /model/production
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /model/purchase.purchase
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /model/sale.sale
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /model/sale.sale/search_read
operation_count: 31
overview: 'Fulfil exposes 31 API operations that an AI agent could call, of which 17 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read, 13 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Fulfil
provider_slug: fulfil-io
slug: fulfil-io-agentic-access
source_filename: fulfil-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/fulfil-io-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 31\n  by_action_class:\n    connected: 14\n    acting: 17\n  by_consequence:\n    read: 14\n    write: 13\n    physical: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /test\n  method: get\n  operationId: testCredentials\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /model/{model_name}\n  method: get\n  operationId: searchModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /model/{model_name}\n\
  \  method: post\n  operationId: createModelRecords\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /model/{model_name}/{id}\n  method: get\n  operationId: readModelRecord\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /model/{model_name}/{id}\n  method: put\n  operationId: updateModelRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /model/{model_name}/{id}\n  method: delete\n  operationId: deleteModelRecord\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /model/{model_name}/search_read\n  method: put\n  operationId: searchReadModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /model/{model_name}/count\n  method: put\n  operationId: countModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /model/{model_name}/{method}\n  method: put\n  operationId: callModelMethod\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /model/sale.sale\n  method: get\n  operationId: searchSalesOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /model/sale.sale\n  method: post\n  operationId: createSalesOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /model/sale.sale/search_read\n\
  \  method: put\n  operationId: searchReadSalesOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /model/product.template\n  method: get\n  operationId: searchProductTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /model/product.template\n  method: post\n  operationId: createProductTemplates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /model/product.product\n\
  \  method: get\n  operationId: searchProductVariants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /model/product.product\n  method: post\n  operationId: createProductVariants\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /model/product.product/search_read\n  method: put\n  operationId: searchReadProductVariants\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /model/stock.move\n  method: get\n  operationId: searchStockMoves\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /model/stock.move\n  method: post\n  operationId: createStockMoves\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /model/stock.location\n  method: get\n  operationId: searchStockLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /model/party.party\n  method: get\n  operationId: searchParties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /model/party.party\n  method: post\n  operationId:\
  \ createParties\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /model/party.party/search_read\n  method: put\n  operationId: searchReadParties\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /model/stock.shipment.out\n  method: get\n  operationId: searchOutboundShipments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /model/stock.shipment.in\n  method: get\n  operationId: searchInboundShipments\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /model/purchase.purchase\n  method: get\n  operationId: searchPurchaseOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /model/purchase.purchase\n  method: post\n  operationId: createPurchaseOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /model/production\n  method: get\n  operationId: searchProductionOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /model/production\n  method: post\n  operationId: createProductionOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /model/webhook.webhook\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /model/webhook.webhook\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fulfil-io/refs/heads/main/agentic-access/fulfil-io-agentic-access.yml
summary_line: 31 operations · 17 acting
tags:
- ERP
- E-commerce
- Order Management
- Inventory
- Warehouse Management
- Manufacturing
- Operations
---
