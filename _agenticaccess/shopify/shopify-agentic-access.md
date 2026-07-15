---
acting_count: 739
action_class_counts:
  acting: 739
  connected: 808
api_specs:
- filename: shopify-api-openapi.yml
  format: yaml
  label: Shopify Admin REST API
  slug: shopify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopify/refs/heads/main/openapi/shopify-api-openapi.yml
- filename: shopify-ajax-api-openapi.yml
  format: yaml
  label: Shopify Ajax API
  slug: ajax-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopify/refs/heads/main/openapi/shopify-ajax-api-openapi.yml
- filename: shopify-webhooks-api-openapi.yml
  format: yaml
  label: Shopify Webhooks API
  slug: webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopify/refs/heads/main/openapi/shopify-webhooks-api-openapi.yml
- filename: shopify-multipass-api-openapi.yml
  format: yaml
  label: Shopify Multipass API
  slug: multipass-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopify/refs/heads/main/openapi/shopify-multipass-api-openapi.yml
consequence_counts:
  physical: 262
  read: 808
  safety-critical: 6
  write: 471
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 6
kind: agentic-access
layout: agentic-access
method: generated
name: Shopify Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /admin/api/2020-01/gift_cards/{gift_card_id}/disable.json
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /admin/api/2020-04/gift_cards/{gift_card_id}/disable.json
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /admin/api/2020-07/gift_cards/{gift_card_id}/disable.json
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /admin/api/2020-10/gift_cards/{gift_card_id}/disable.json
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /admin/api/2021-01/gift_cards/{gift_card_id}/disable.json
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /admin/api/unstable/gift_cards/{gift_card_id}/disable.json
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/api/2020-01/application_charges.json
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/api/2020-01/application_charges/{application_charge_id}/activate.json
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/api/2020-01/checkouts.json
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /admin/api/2020-01/checkouts/{token}.json
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/api/2020-01/checkouts/{token}/complete.json
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/api/2020-01/checkouts/{token}/payments.json
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/api/2020-01/customers/{customer_id}/send_invite.json
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/api/2020-01/fulfillment_orders/{fulfillment_order_id}/cancel.json
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/api/2020-01/fulfillment_orders/{fulfillment_order_id}/cancellation_request.json
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/api/2020-01/fulfillment_orders/{fulfillment_order_id}/cancellation_request/accept.json
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/api/2020-01/fulfillment_orders/{fulfillment_order_id}/cancellation_request/reject.json
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/api/2020-01/fulfillment_orders/{fulfillment_order_id}/close.json
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/api/2020-01/fulfillment_orders/{fulfillment_order_id}/fulfillment_request.json
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/api/2020-01/fulfillment_orders/{fulfillment_order_id}/fulfillment_request/accept.json
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/api/2020-01/fulfillment_orders/{fulfillment_order_id}/fulfillment_request/reject.json
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/api/2020-01/fulfillment_orders/{fulfillment_order_id}/move.json
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/api/2020-01/fulfillment_services.json
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /admin/api/2020-01/fulfillment_services/{fulfillment_service_id}.json
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /admin/api/2020-01/fulfillment_services/{fulfillment_service_id}.json
operation_count: 1547
overview: 'Shopify exposes 1547 API operations that an AI agent could call, of which 739 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 808 read, 471 write, 262 physical, and 6 safety-critical.


  6 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Shopify
provider_slug: shopify
slug: shopify-agentic-access
source_filename: shopify-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/shopify-admin-rest-api-openapi.yml, openapi/shopify-ajax-api-openapi.yml, openapi/shopify-api-openapi.yml,\n  openapi/shopify-multipass-api-openapi.yml, openapi/shopify-webhooks-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 1547\n  by_action_class:\n    connected: 808\n    acting: 739\n  by_consequence:\n    read: 808\n    write: 471\n    physical: 262\n    safety-critical: 6\n  human_in_the_loop_required: 6\noperations:\n- path: /products.json\n  method: get\n  operationId: listProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products.json\n  method:\
  \ post\n  operationId: createProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /products/count.json\n  method: get\n  operationId: getProductCount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/{product_id}.json\n  method: get\n  operationId: getProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/{product_id}.json\n  method: put\n  operationId: updateProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /products/{product_id}.json\n  method: delete\n  operationId: deleteProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /products/{product_id}/images.json\n  method: get\n  operationId: listProductImages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/{product_id}/images.json\n  method: post\n  operationId: createProductImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /products/{product_id}/images/count.json\n  method: get\n  operationId: getProductImageCount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/{product_id}/images/{image_id}.json\n  method: get\n  operationId: getProductImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/{product_id}/images/{image_id}.json\n  method: put\n  operationId: updateProductImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /products/{product_id}/images/{image_id}.json\n\
  \  method: delete\n  operationId: deleteProductImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /products/{product_id}/variants.json\n  method: get\n  operationId: listProductVariants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/{product_id}/variants.json\n  method: post\n  operationId: createProductVariant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers.json\n  method: get\n  operationId:\
  \ listCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers.json\n  method: post\n  operationId: createCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/count.json\n  method: get\n  operationId: getCustomerCount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/search.json\n  method: get\n  operationId: searchCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customer_id}.json\n\
  \  method: get\n  operationId: getCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customer_id}.json\n  method: put\n  operationId: updateCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{customer_id}/orders.json\n  method: get\n  operationId: listCustomerOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customer_id}/addresses.json\n  method: get\n  operationId: listCustomerAddresses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /customers/{customer_id}/addresses.json\n  method: post\n  operationId: createCustomerAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders.json\n  method: get\n  operationId: listOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders.json\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /orders/count.json\n  method: get\n  operationId: getOrderCount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{order_id}.json\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{order_id}.json\n  method: put\n  operationId: updateOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{order_id}.json\n  method: delete\n  operationId: deleteOrder\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{order_id}/cancel.json\n  method: post\n  operationId: cancelOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{order_id}/close.json\n  method: post\n  operationId: closeOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{order_id}/open.json\n  method: post\n  operationId: reopenOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{order_id}/fulfillment_orders.json\n  method: get\n  operationId: listOrderFulfillmentOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fulfillments.json\n  method: post\n  operationId: createFulfillment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fulfillments/{fulfillment_id}/update_tracking.json\n  method: post\n  operationId: updateFulfillmentTracking\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fulfillments/{fulfillment_id}/cancel.json\n  method: post\n  operationId: cancelFulfillment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n    \
  \  - abnormal\n      - high-value\n    audit: required\n- path: /inventory_items.json\n  method: get\n  operationId: listInventoryItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inventory_items/{inventory_item_id}.json\n  method: get\n  operationId: getInventoryItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inventory_items/{inventory_item_id}.json\n  method: put\n  operationId: updateInventoryItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inventory_levels.json\n  method: get\n  operationId: listInventoryLevels\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inventory_levels/set.json\n  method: post\n  operationId: setInventoryLevel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /locations.json\n  method: get\n  operationId: listLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locations/count.json\n  method: get\n  operationId: getLocationCount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locations/{location_id}.json\n  method: get\n  operationId: getLocation\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locations/{location_id}/inventory_levels.json\n  method: get\n  operationId: listLocationInventoryLevels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collection_id}.json\n  method: get\n  operationId: getCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collection_id}/products.json\n  method: get\n  operationId: listCollectionProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /custom_collections.json\n  method: get\n  operationId: listCustomCollections\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /custom_collections.json\n  method: post\n  operationId: createCustomCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /smart_collections.json\n  method: get\n  operationId: listSmartCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks.json\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks.json\n  method: post\n  operationId: createWebhook\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/count.json\n  method: get\n  operationId: getWebhookCount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/{webhook_id}.json\n  method: get\n  operationId: getWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/{webhook_id}.json\n  method: put\n  operationId: updateWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{webhook_id}.json\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shop.json\n  method: get\n  operationId: getShop\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/oauth/access_scopes.json\n  method: get\n  operationId: listAccessScopes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cart.js\n  method: get\n  operationId: getCart\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cart/add.js\n  method: post\n  operationId: addToCart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cart/update.js\n  method: post\n  operationId: updateCart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cart/change.js\n  method: post\n  operationId: changeCartItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cart/clear.js\n  method: post\n  operationId: clearCart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cart/shipping_rates.json\n  method: get\n  operationId: getCartShippingRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/{handle}.js\n  method: get\n  operationId: getProductByHandle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recommendations/products.json\n  method: get\n  operationId: getProductRecommendations\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/suggest.json\n  method: get\n  operationId: getPredictiveSearchResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/oauth/access_scopes.json\n  method: get\n  operationId: get_admin_oauth_access_scopes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/api/2020-01/storefront_access_tokens.json\n  method: post\n  operationId: deprecated_202001_create_storefront_access_tokens\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /admin/api/2020-01/storefront_access_tokens.json\n  method: get\n  operationId: deprecated_202001_get_storefront_access_tokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/api/2020-01/storefront_access_tokens/{storefront_access_token_id}.json\n  method: delete\n  operationId: deprecated_202001_delete_storefront_access_tokens_param_storefront_access_token_id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/api/2020-04/storefront_access_tokens.json\n  method: post\n  operationId: deprecated_202004_create_storefront_access_tokens\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/api/2020-04/storefront_access_tokens.json\n  method: get\n  operationId: deprecated_202004_get_storefront_access_tokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/api/2020-04/storefront_access_tokens/{storefront_access_token_id}.json\n  method: delete\n  operationId: deprecated_202004_delete_storefront_access_tokens_param_storefront_access_token_id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/api/2020-07/storefront_access_tokens.json\n\
  \  method: post\n  operationId: deprecated_202007_create_storefront_access_tokens\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/api/2020-07/storefront_access_tokens.json\n  method: get\n  operationId: deprecated_202007_get_storefront_access_tokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/api/2020-07/storefront_access_tokens/{storefront_access_token_id}.json\n  method: delete\n  operationId: deprecated_202007_delete_storefront_access_tokens_param_storefront_access_token_id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/api/2020-10/storefront_access_tokens.json\n  method: post\n  operationId: create_storefront_access_tokens\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/api/2020-10/storefront_access_tokens.json\n  method: get\n  operationId: get_storefront_access_tokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/api/2020-10/storefront_access_tokens/{storefront_access_token_id}.json\n  method: delete\n  operationId: delete_storefront_access_tokens_param_storefront_access_token_id\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/api/2021-01/storefront_access_tokens.json\n  method: post\n  operationId: deprecated_202101_create_storefront_access_tokens\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/api/2021-01/storefront_access_tokens.json\n  method: get\n  operationId: deprecated_202101_get_storefront_access_tokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/api/2021-01/storefront_access_tokens/{storefront_access_token_id}.json\n\
  \  method: delete\n  operationId: deprecated_202101_delete_storefront_access_tokens_param_storefront_access_token_id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/api/unstable/storefront_access_tokens.json\n  method: post\n  operationId: deprecated_unstable_create_storefront_access_tokens\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/api/unstable/storefront_access_tokens.json\n  method: get\n  operationId: deprecated_unstable_get_storefront_access_tokens\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/api/unstable/storefront_access_tokens/{storefront_access_token_id}.json\n  method: delete\n  operationId: deprecated_unstable_delete_storefront_access_tokens_param_storefront_access_token_id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/api/2020-01/reports.json\n  method: get\n  operationId: deprecated_202001_get_reports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/api/2020-01/reports.json\n  method: post\n  operationId: deprecated_202001_create_reports\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/api/2020-01/reports/{report_id}.json\n  method: get\n  operationId: deprecated_202001_get_reports_param_report_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/api/2020-01/reports/{report_id}.json\n  method: put\n  operationId: deprecated_202001_update_reports_param_report_id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/api/2020-01/reports/{report_id}.json\n  method: delete\n  operationId: deprecated_202001_delete_reports_param_report_id\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/api/2020-04/reports.json\n  method: get\n  operationId: deprecated_202004_get_reports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/api/2020-04/reports.json\n  method: post\n  operationId: deprecated_202004_create_reports\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/api/2020-04/reports/{report_id}.json\n  method: get\n  operationId: deprecated_202004_get_reports_param_report_id\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/api/2020-04/reports/{report_id}.json\n  method: put\n  operationId: deprecated_202004_update_reports_param_report_id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/api/2020-04/reports/{report_id}.json\n  method: delete\n  operationId: deprecated_202004_delete_reports_param_report_id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/api/2020-07/reports.json\n\
  \  method: get\n  operationId: deprecated_202007_get_reports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/api/2020-07/reports.json\n  method: post\n  operationId: deprecated_202007_create_reports\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/api/2020-07/reports/{report_id}.json\n  method: get\n  operationId: deprecated_202007_get_reports_param_report_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/api/2020-07/reports/{report_id}.json\n  method: put\n  operationId: deprecated_202007_update_reports_param_report_id\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/api/2020-07/reports/{report_id}.json\n  method: delete\n  operationId: deprecated_202007_delete_reports_param_report_id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/api/2020-10/reports.json\n  method: get\n  operationId: get_reports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/api/2020-10/reports.json\n  method: post\n  operationId: create_reports\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/api/2020-10/reports/{report_id}.json\n  method: get\n  operationId: get_reports_param_report_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/api/2020-10/reports/{report_id}.json\n  method: put\n  operationId: update_reports_param_report_id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - hi\n\n# --- truncated at 32 KB (533 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/shopify/refs/heads/main/agentic-access/shopify-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shopify/refs/heads/main/agentic-access/shopify-agentic-access.yml
summary_line: 1547 operations · 739 acting · 6 human-in-the-loop
tags:
- Commerce
- Ecommerce
- Payments
- Retail
- Shopping Cart
- T1
---
