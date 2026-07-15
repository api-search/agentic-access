---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 15
api_specs:
- filename: printify-openapi.yml
  format: yaml
  label: Printify Shops API
  slug: printify-shops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printify/refs/heads/main/openapi/printify-openapi.yml
- filename: printify-openapi.yml
  format: yaml
  label: Printify Catalog API
  slug: printify-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printify/refs/heads/main/openapi/printify-openapi.yml
- filename: printify-openapi.yml
  format: yaml
  label: Printify Products API
  slug: printify-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printify/refs/heads/main/openapi/printify-openapi.yml
- filename: printify-openapi.yml
  format: yaml
  label: Printify Orders API
  slug: printify-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printify/refs/heads/main/openapi/printify-openapi.yml
- filename: printify-openapi.yml
  format: yaml
  label: Printify Uploads API
  slug: printify-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printify/refs/heads/main/openapi/printify-openapi.yml
- filename: printify-openapi.yml
  format: yaml
  label: Printify Webhooks API
  slug: printify-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printify/refs/heads/main/openapi/printify-openapi.yml
consequence_counts:
  physical: 5
  read: 15
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Printify Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /shops/{shop_id}/express.json
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /shops/{shop_id}/orders.json
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /shops/{shop_id}/orders/shipping.json
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /shops/{shop_id}/orders/{order_id}/cancel.json
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /shops/{shop_id}/orders/{order_id}/send_to_production.json
operation_count: 33
overview: 'Printify exposes 33 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read, 13 write, and 5 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Printify
provider_slug: printify
slug: printify-agentic-access
source_filename: printify-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/printify-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 33\n  by_action_class:\n    connected: 15\n    acting: 18\n  by_consequence:\n    read: 15\n    write: 13\n    physical: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /shops.json\n  method: get\n  operationId: listShops\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shops/{shop_id}/connection.json\n  method: delete\n  operationId: disconnectShop\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /catalog/blueprints.json\n  method: get\n  operationId: listBlueprints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/blueprints/{blueprint_id}.json\n  method: get\n  operationId: getBlueprint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/blueprints/{blueprint_id}/print_providers.json\n  method: get\n  operationId: listBlueprintPrintProviders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/blueprints/{blueprint_id}/print_providers/{print_provider_id}/variants.json\n  method: get\n  operationId: listVariants\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/blueprints/{blueprint_id}/print_providers/{print_provider_id}/shipping.json\n  method: get\n  operationId: getVariantShipping\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/print_providers.json\n  method: get\n  operationId: listPrintProviders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/print_providers/{print_provider_id}.json\n  method: get\n  operationId: getPrintProvider\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shops/{shop_id}/products.json\n  method: get\n  operationId: listProducts\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shops/{shop_id}/products.json\n  method: post\n  operationId: createProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shops/{shop_id}/products/{product_id}.json\n  method: get\n  operationId: getProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shops/{shop_id}/products/{product_id}.json\n  method: put\n  operationId: updateProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shops/{shop_id}/products/{product_id}.json\n  method: delete\n  operationId: deleteProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shops/{shop_id}/products/{product_id}/publish.json\n  method: post\n  operationId: publishProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shops/{shop_id}/products/{product_id}/publishing_succeeded.json\n  method: post\n  operationId: setPublishSucceeded\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shops/{shop_id}/products/{product_id}/publishing_failed.json\n  method: post\n  operationId: setPublishFailed\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shops/{shop_id}/products/{product_id}/unpublish.json\n  method: post\n  operationId: unpublishProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /shops/{shop_id}/orders.json\n  method: get\n  operationId: listOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shops/{shop_id}/orders.json\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shops/{shop_id}/orders/{order_id}.json\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shops/{shop_id}/express.json\n  method: post\n  operationId: createExpressOrder\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shops/{shop_id}/orders/shipping.json\n  method: post\n  operationId: calculateShipping\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shops/{shop_id}/orders/{order_id}/send_to_production.json\n  method: post\n  operationId: sendOrderToProduction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shops/{shop_id}/orders/{order_id}/cancel.json\n  method: post\n  operationId: cancelOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /uploads.json\n  method: get\n  operationId: listUploads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /uploads/{image_id}.json\n  method: get\n  operationId: getUpload\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /uploads/images.json\n  method: post\n  operationId: uploadImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /uploads/{image_id}/archive.json\n  method: post\n  operationId: archiveUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shops/{shop_id}/webhooks.json\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /shops/{shop_id}/webhooks.json\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shops/{shop_id}/webhooks/{webhook_id}.json\n  method: put\n  operationId: updateWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shops/{shop_id}/webhooks/{webhook_id}.json\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/printify/refs/heads/main/agentic-access/printify-agentic-access.yml
summary_line: 33 operations · 18 acting
tags:
- Print on Demand
- Ecommerce
- Marketplace
- Fulfillment
- Merchandise
---
