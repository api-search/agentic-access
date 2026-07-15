---
acting_count: 17
action_class_counts:
  acting: 17
  connected: 13
api_specs:
- filename: squarespace-commerce-api-openapi.yml
  format: yaml
  label: Squarespace Commerce API
  slug: squarespace-commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/squarespace/refs/heads/main/openapi/squarespace-commerce-api-openapi.yml
- filename: squarespace-orders-api-openapi.yml
  format: yaml
  label: Squarespace Orders API
  slug: squarespace-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/squarespace/refs/heads/main/openapi/squarespace-orders-api-openapi.yml
- filename: squarespace-products-api-openapi.yml
  format: yaml
  label: Squarespace Products API
  slug: squarespace-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/squarespace/refs/heads/main/openapi/squarespace-products-api-openapi.yml
- filename: squarespace-inventory-api-openapi.yml
  format: yaml
  label: Squarespace Inventory API
  slug: squarespace-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/squarespace/refs/heads/main/openapi/squarespace-inventory-api-openapi.yml
- filename: squarespace-profiles-api-openapi.yml
  format: yaml
  label: Squarespace Profiles API
  slug: squarespace-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/squarespace/refs/heads/main/openapi/squarespace-profiles-api-openapi.yml
- filename: squarespace-transactions-api-openapi.yml
  format: yaml
  label: Squarespace Transactions API
  slug: squarespace-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/squarespace/refs/heads/main/openapi/squarespace-transactions-api-openapi.yml
- filename: squarespace-webhook-subscriptions-api-openapi.yml
  format: yaml
  label: Squarespace Webhook Subscriptions API
  slug: squarespace-webhook-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/squarespace/refs/heads/main/openapi/squarespace-webhook-subscriptions-api-openapi.yml
consequence_counts:
  physical: 4
  read: 13
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Squarespace Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /commerce/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /commerce/orders/{orderId}/fulfillments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /commerce/products/{productId}/images/reorder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /webhook_subscriptions/{subscriptionId}/actions/sendTestNotification
operation_count: 30
overview: 'Squarespace exposes 30 API operations that an AI agent could call, of which 17 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read, 13 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Squarespace
provider_slug: squarespace
slug: squarespace-agentic-access
source_filename: squarespace-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/squarespace-commerce-api-openapi.yml, openapi/squarespace-inventory-api-openapi.yml,\n  openapi/squarespace-orders-api-openapi.yml, openapi/squarespace-products-api-openapi.yml,\n  openapi/squarespace-profiles-api-openapi.yml, openapi/squarespace-transactions-api-openapi.yml,\n  openapi/squarespace-webhook-subscriptions-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 30\n  by_action_class:\n    connected: 13\n    acting: 17\n  by_consequence:\n    read: 13\n    write: 13\n    physical: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /authorization/website\n  method: get\n  operationId: retrieveSiteInfo\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /commerce/inventory\n  method: get\n  operationId: listInventory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /commerce/inventory/{variantIds}\n  method: get\n  operationId: getInventoryByVariants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /commerce/inventory/adjustments\n  method: post\n  operationId: adjustInventory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commerce/orders\n  method: get\n  operationId: listOrders\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /commerce/orders\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commerce/orders/{orderId}\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /commerce/orders/{orderId}/fulfillments\n  method: post\n  operationId: fulfillOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commerce/products\n  method: get\n  operationId: listProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /commerce/products\n  method: post\n  operationId: createProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commerce/products/{productIds}\n  method: get\n  operationId: getProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /commerce/products/{productIds}\n\
  \  method: post\n  operationId: updateProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commerce/products/{productIds}\n  method: delete\n  operationId: deleteProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commerce/products/{productId}/variants\n  method: post\n  operationId: createProductVariant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /commerce/products/{productId}/variants/{variantId}\n  method: post\n  operationId: updateProductVariant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commerce/products/{productId}/images\n  method: post\n  operationId: uploadProductImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commerce/products/{productId}/images/{imageId}\n  method: post\n  operationId: updateProductImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commerce/products/{productId}/images/{imageId}\n  method: delete\n  operationId: deleteProductImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commerce/products/{productId}/images/reorder\n  method: post\n  operationId: reorderProductImages\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /profiles\n  method: get\n  operationId: listProfiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profiles/{profileIds}\n  method: get\n  operationId: getProfiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /commerce/transactions\n  method: get\n  operationId: listTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /commerce/transactions/{transactionIds}\n  method: get\n  operationId: getTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook_subscriptions\n  method: get\n  operationId: listWebhookSubscriptions\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook_subscriptions\n  method: post\n  operationId: createWebhookSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook_subscriptions/{subscriptionId}\n  method: get\n  operationId: getWebhookSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook_subscriptions/{subscriptionId}\n  method: post\n  operationId: updateWebhookSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n   \
  \   max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook_subscriptions/{subscriptionId}\n  method: delete\n  operationId: deleteWebhookSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook_subscriptions/{subscriptionId}/actions/sendTestNotification\n  method: post\n  operationId: sendTestNotification\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /webhook_subscriptions/{subscriptionId}/actions/rotateSecret\n  method: post\n  operationId: rotateWebhookSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/squarespace/refs/heads/main/agentic-access/squarespace-agentic-access.yml
summary_line: 30 operations · 17 acting
tags:
- Commerce
- E-Commerce
- Marketing
- Payments
- Retail
- Website Builder
- Webhooks
---
