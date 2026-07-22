---
acting_count: 96
action_class_counts:
  acting: 96
  connected: 101
api_specs:
- filename: shoplazza-admin-openapi-original.json
  format: json
  label: Shoplazza Admin API
  slug: shoplazza-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shoplazza/refs/heads/main/openapi/shoplazza-admin-openapi-original.json
consequence_counts:
  physical: 24
  read: 101
  safety-critical: 1
  write: 71
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Shoplazza Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /openapi/2022-01/gift_cards/{id}/disable
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /openapi/2022-01/application_charges
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /openapi/2022-01/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /openapi/2022-01/orders/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /openapi/2022-01/orders/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /openapi/2022-01/orders/{id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /openapi/2022-01/orders/{id}/close
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /openapi/2022-01/orders/{id}/open
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /openapi/2022-01/orders/{id}/partial_refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /openapi/2022-01/orders/{id}/payment/success
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /openapi/2022-01/orders/{id}/refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /openapi/2022-01/orders/{id}/transactions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /openapi/2022-01/orders/{order_id}/fulfillments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /openapi/2022-01/orders/{order_id}/fulfillments/{fulfillment_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /openapi/2022-01/orders/{order_id}/fulfillments/{fulfillment_id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /openapi/2022-01/orders/{order_id}/fulfillments/{fulfillment_id}/complete
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /openapi/2022-01/orders/{order_id}/risks
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /openapi/2022-01/orders/{order_id}/risks/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /openapi/2022-01/orders/{order_id}/risks/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /openapi/2022-01/payments_apps/complete_callbacks
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /openapi/2022-01/payments_apps/notify_callbacks
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /openapi/2022-01/recurring_application_charges
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /openapi/2022-01/recurring_application_charges/{charge_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /openapi/2022-01/recurring_application_charges/{recurring_charge_id}/customize
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /openapi/2022-01/recurring_application_charges/{recurring_charge_id}/usage_charge
operation_count: 197
overview: 'Shoplazza exposes 197 API operations that an AI agent could call, of which 96 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 101 read, 71 write, 24 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Shoplazza
provider_slug: shoplazza
slug: shoplazza-agentic-access
source_filename: shoplazza-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/shoplazza-admin-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 197\n  by_action_class:\n    connected: 101\n    acting: 96\n  by_consequence:\n    read: 101\n    write: 71\n    physical: 24\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /openapi/2022-01/products\n  method: get\n  operationId: product_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2022-01/products\n  method: post\n  operationId: create_product\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/products/count\n  method: get\n  operationId: product_count\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2022-01/products/{product_id}\n  method: get\n  operationId: product_show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2022-01/products/{product_id}\n  method: put\n  operationId: update_product\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /openapi/2022-01/products/{product_id}\n  method: delete\n  operationId: delete_product\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/variants/{variant_id}\n  method: get\n  operationId: variant_show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2022-01/variants/{variant_id}\n  method: put\n  operationId: update_variant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /openapi/2022-01/products/{product_id}/variants/count\n  method: get\n  operationId: variant_count\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2022-01/products/{product_id}/variants\n  method: get\n  operationId: variant_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2022-01/products/{product_id}/variants\n  method: post\n  operationId: create_variant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/products/{product_id}/images\n  method: get\n  operationId: product_image_list\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2022-01/products/{product_id}/images\n  method: post\n  operationId: create_product_image\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/products/{product_id}/variants/{variant_id}\n  method: delete\n  operationId: delete_variant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/products/{product_id}/images/count\n  method: get\n  operationId: product_image_count\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2022-01/products/{product_id}/images/{image_id}\n  method: get\n  operationId: product_image_show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2022-01/products/{product_id}/images/{image_id}\n  method: delete\n  operationId: delete_product_image\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/products/{product_id}/images/{image_id}\n  method: put\n  operationId: update_product_image\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n   \
  \ subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/products/{product_id}/metafields\n  method: get\n  operationId: metafield_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2022-01/products/{product_id}/metafields\n  method: post\n  operationId: create-metafield\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/products/{product_id}/metafields/count\n  method: get\n  operationId: metafield_count\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2022-01/products/{product_id}/metafields/{metafield_id}\n  method: get\n  operationId: metafield_show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2022-01/products/{product_id}/metafields/{metafield_id}\n  method: delete\n  operationId: delate-metafield\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/products/{product_id}/metafields/{metafield_id}\n  method: put\n  operationId: update-metafield\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/variants/sku/{sku}\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/products/sku/{sku}/variants\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2022-01/collections\n  method: get\n  operationId: collection_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2022-01/collections\n  method: post\n\
  \  operationId: create_collection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/collections/count\n  method: get\n  operationId: collection_count\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2022-01/collections/{id}\n  method: get\n  operationId: collection_show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2022-01/collections/{id}\n  method: put\n  operationId: update_collection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/collections/{id}\n  method: delete\n  operationId: delete_collection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/collects\n  method: post\n  operationId: create_collect\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/collects\n  method: get\n  operationId: collect_list\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2020-07/collects/count\n  method: get\n  operationId: collect_count\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2022-01/collects/{id}\n  method: delete\n  operationId: delete_collect\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/collects/{id}\n  method: get\n  operationId: collect_show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2022-01/payments_apps/complete_callbacks\n  method:\
  \ post\n  operationId: payment-session\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/payments_apps/notify_callbacks\n  method: post\n  operationId: notify-payment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/oauth/access_scopes\n  method: get\n  operationId: get-access-scopes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2022-01/orders/{order_id}/fulfillments\n  method: get\n  operationId: fulfillment-list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2022-01/orders/{order_id}/fulfillments\n  method: post\n  operationId: create_fulfillment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/orders/{order_id}/fulfillments/count\n  method: get\n  operationId: fulfillment_count\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /openapi/2022-01/orders/{order_id}/fulfillments/{fulfillment_id}\n  method: get\n  operationId: fulfillment_show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2022-01/orders/{order_id}/fulfillments/{fulfillment_id}\n  method: put\n  operationId: update_fulfillment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/orders/{order_id}/fulfillments/{fulfillment_id}/complete\n  method: post\n  operationId: complete_fulfillment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/orders/{order_id}/fulfillments/{fulfillment_id}/cancel\n  method: post\n  operationId: cancel_fulfillment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/shop\n  method: get\n  operationId: shop-details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2022-01/shop/{shop_id}\n  method: patch\n  operationId: update-shop\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/orders\n  method: get\n  operationId: order-list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2022-01/orders\n  method: post\n  operationId: create-order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/orders/{id}\n  method: get\n  operationId: order-details\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2022-01/orders/{id}\n  method: delete\n  operationId: delete-order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/orders/{id}\n  method: put\n  operationId: update-order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/orders/number/{number}\n  method: get\n  operationId:\
  \ order-details-by-number\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2022-01/orders/count\n  method: get\n  operationId: order-count\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2022-01/orders/{id}/cancel\n  method: post\n  operationId: cancel-order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/orders/{id}/refund\n  method: post\n  operationId: order-refund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/orders/{id}/refund\n  method: get\n  operationId: refund-list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2022-01/orders/{id}/partial_refund\n  method: post\n  operationId: partial-order-refund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/orders/after_sales_list\n  method: get\n  operationId: after-sales-list\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2022-01/price_rules\n  method: get\n  operationId: price-rule-list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2022-01/price_rules\n  method: post\n  operationId: create-price-rule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/price_rules/count\n  method: get\n  operationId: price-rule-count\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2022-01/price_rules/{price_rule_id}\n\
  \  method: get\n  operationId: price-rule-detail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2022-01/price_rules/{price_rule_id}\n  method: put\n  operationId: update-price-rule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/price_rules/{price_rule_id}\n  method: delete\n  operationId: delete-price-rule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/price_rules/{price_rule_id}/discount_codes\n\
  \  method: post\n  operationId: create-discount-code\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/price_rules/{price_rule_id}/discount_codes\n  method: get\n  operationId: get-discount-code-list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2022-01/price_rules/{price_rule_id}/discount_codes\n  method: delete\n  operationId: delete-discount-code\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /openapi/2022-01/price_rules/{price_rule_id}/discount_codes/{discount_code_id}\n  method: put\n  operationId: update-discount-code\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/price_rules/{price_rule_id}/discount_codes/{discount_code_id}\n  method: get\n  operationId: get-discount-code\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2022-01/discount_codes/lookup\n  method: get\n  operationId: search-discount-code\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2022-01/redirects\n  method: post\n \
  \ operationId: create-redirect\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/redirects\n  method: get\n  operationId: redirect-list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2022-01/redirects/{id}\n  method: get\n  operationId: redirect-detail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2022-01/redirects/{id}\n  method: put\n  operationId: update-redirect\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/redirects/{id}\n  method: delete\n  operationId: delete-redirect\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/redirects/detail\n  method: post\n  operationId: search-redirect\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/themes/{theme_id}\n  method: get\n  operationId: get-theme\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2022-01/themes/{theme_id}\n  method: delete\n  operationId: delete-theme\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/themes/default-theme\n  method: get\n  operationId: get-default-theme\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2022-01/themes\n  method: get\n  operationId: get-theme-list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2022-01/themes/{theme_id}/publish\n  method: patch\n\
  \  operationId: publish-theme\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/themes/upload\n  method: post\n  operationId: upload-theme\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/themes/{theme_id}/download\n  method: get\n  operationId: download-theme\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2022-01/themes/{theme_id}/doctree\n  method: get\n  operationId: get-theme-doctree\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2022-01/themes/{theme_id}/doc\n  method: get\n  operationId: get-theme-file\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2022-01/themes/{theme_id}/doc\n  method: delete\n  operationId: delete-theme-file\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/themes/{theme_id}/doc\n  method: post\n  operationId: create-theme-file\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/themes/{theme_id}/doc\n  method: patch\n  operationId: update-theme-file\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/themes/{theme_id}/doc-asset\n  method: post\n  operationId: create-theme-assets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/customers\n  method: get\n  operationId: customer-list\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2022-01/customers\n  method: post\n  operationId: create-customer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/customers/{id}\n  method: get\n  operationId: customer-details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2022-01/customers/{id}\n  method: put\n  operationId: update-customer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/customers/count\n  method: get\n  operationId: customer-count\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2022-01/customers/{customer_id}/addresses\n  method: get\n  operationId: get-address-list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2022-01/customers/{customer_id}/addresses\n  method: post\n  operationId: create-address\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/customers/{customer_id}/addresses/{address_id}\n\
  \  method: get\n  operationId: get-address-details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2022-01/customers/{customer_id}/addresses/{address_id}\n  method: put\n  operationId: update-address\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/customers/{customer_id}/addresses/{address_id}\n  method: delete\n  operationId: delete-address\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /openapi/2022-01/customers/{customer_id}/addresses/{address_id}/default\n  method: put\n  operationId: set-default-address\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/webhooks\n  method: get\n  operationId: webhook-list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/2022-01/webhooks\n  method: post\n  operationId: create-webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/2022-01/webhooks/count\n\
  \  method: g\n\n# --- truncated at 32 KB (58 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/shoplazza/refs/heads/main/agentic-access/shoplazza-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shoplazza/refs/heads/main/agentic-access/shoplazza-agentic-access.yml
summary_line: 197 operations · 96 acting · 1 human-in-the-loop
tags:
- Company
- Enterprise
- E-Commerce
- Online Store
- Retail
- Payments
- Webhooks
- REST API
- Apps
- Developer Platform
---
