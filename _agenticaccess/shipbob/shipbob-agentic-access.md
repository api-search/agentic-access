---
acting_count: 30
action_class_counts:
  acting: 30
  connected: 42
api_specs:
- filename: shipbob-openapi.json
  format: json
  label: ShipBob Developer API
  slug: shipbob-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipbob/refs/heads/main/openapi/shipbob-openapi.json
consequence_counts:
  physical: 16
  read: 42
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Shipbob Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /2026-01/order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /2026-01/order/{orderId}/shipment/{shipmentId}:cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /2026-01/order/{orderId}:cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /2026-01/order:estimate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /2026-01/receiving
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /2026-01/receiving/{id}:cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /2026-01/return
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /2026-01/return/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /2026-01/return/{id}:cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /2026-01/shipment/{shipmentId}:cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /2026-01/shipment/{shipmentId}:updateAddress
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /2026-01/shipment/{shipmentId}:updateLineItems
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /2026-01/shipment:batchCancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /2026-01/shipment:batchUpdateTrackingUpload
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /2026-01/shipment:bulkUpdateShippingService
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /2026-01/simulate/shipment
operation_count: 72
overview: 'ShipBob exposes 72 API operations that an AI agent could call, of which 30 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 42 read, 14 write, and 16 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ShipBob
provider_slug: shipbob
slug: shipbob-agentic-access
source_filename: shipbob-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/shipbob-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 72\n  by_action_class:\n    connected: 42\n    acting: 30\n  by_consequence:\n    read: 42\n    physical: 16\n    write: 14\n  human_in_the_loop_required: 0\noperations:\n- path: /2026-01/channel\n  method: get\n  operationId: get-channels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2026-01/order\n  method: post\n  operationId: create-order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n\
  \      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2026-01/order\n  method: get\n  operationId: get-orders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2026-01/order/{orderId}\n  method: get\n  operationId: get-order\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2026-01/shipment/{shipmentId}\n  method: get\n  operationId: get-shipment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2026-01/shipment/{shipmentId}/timeline\n  method: get\n  operationId: get-shipment-timeline\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2026-01/shipment:batchCancel\n  method: post\n  operationId: batch-cancel-shipments\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2026-01/shipment:batchUpdateTrackingUpload\n  method: post\n  operationId: mark-tracking-uploaded\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2026-01/shipment/{shipmentId}:updateAddress\n  method:\
  \ put\n  operationId: update-shipment-address\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2026-01/shipment/{shipmentId}:getLineItems\n  method: get\n  operationId: get-shipment-line-items\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2026-01/shipment/{shipmentId}:updateLineItems\n  method: post\n  operationId: update-shipment-line-items\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2026-01/shipment:bulkUpdateShippingService\n  method: put\n  operationId: bulk-update-shipping-service\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2026-01/order/{orderId}:cancel\n  method: post\n  operationId: cancel-order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2026-01/shipment/{shipmentId}:cancel\n  method: post\n\
  \  operationId: cancel-shipment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2026-01/shipping-method\n  method: get\n  operationId: get-shipping-methods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2026-01/order/{orderId}/shipment/{shipmentId}/timeline\n  method: get\n  operationId: get-shipment-status-timeline-by-order-id-and-shipment-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2026-01/order/{orderId}/shipment\n  method: get\n  operationId: get-all-shipments-for-order\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2026-01/order/{orderId}/shipment/{shipmentId}/logs\n  method: get\n  operationId: get-shipment-logs-by-order-id-and-shipment-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2026-01/order/{orderId}/shipment/{shipmentId}:cancel\n  method: post\n  operationId: cancel-shipment-by-order-id-and-shipment-id\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2026-01/shipment/{shipmentId}/logs\n  method: get\n  operationId: get-shipment-logs\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2026-01/order/{orderId}/shipment/{shipmentId}\n  method: get\n  operationId: get-shipment-by-order-id-and-shipment-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2026-01/order:estimate\n  method: post\n  operationId: estimate-fulfillment-cost-for-order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2026-01/order/{orderId}/store-order-json\n  method: get\n  operationId: get-order-store-data\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2026-01/product\n  method: post\n  operationId: create-product\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2026-01/product\n  method: get\n  operationId: get-products\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2026-01/product/{productId}\n  method: get\n  operationId: get-product\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2026-01/product/{productId}\n  method: patch\n  operationId: update-product\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2026-01/product/{productId}\n  method: delete\n  operationId: delete-product-bundle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2026-01/product/{productId}/variants\n  method: get\n  operationId: get-product-variants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2026-01/product/{productId}/variants\n  method: post\n  operationId: add-product-variants\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2026-01/product/{productId}/variants\n  method: patch\n  operationId: update-product-variants\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2026-01/variant/{variantId}:merge\n  method: post\n  operationId: merge-variants\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2026-01/product/{productId}:moveVariants\n\
  \  method: post\n  operationId: move-variants-between-products\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2026-01/product:moveVariants\n  method: post\n  operationId: move-variants-to-new-product\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2026-01/packaging-requirement\n  method: get\n  operationId: get-packaging-requirement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2026-01/taxonomy\n  method: get\n\
  \  operationId: get-taxonomies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2026-01/taxonomy/{id}\n  method: get\n  operationId: get-taxonomy-by-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2026-01/taxonomy/{id}/parent\n  method: get\n  operationId: get-taxonomy-parent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2026-01/variant/{variantId}:convertToBundle\n  method: post\n  operationId: convert-variant-to-bundle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /2026-01/inventory-level\n  method: get\n  operationId: get-all-inventory-levels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2026-01/inventory-level/{inventoryId}\n  method: get\n  operationId: get-inventory-levels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2026-01/inventory/{inventoryId}\n  method: get\n  operationId: get-inventory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2026-01/inventory\n  method: get\n  operationId: get-all-inventories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2026-01/inventory/history:query\n\
  \  method: post\n  operationId: query-inventory-history-events\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2026-01/inventory-level/locations\n  method: get\n  operationId: get-all-inventory-levels-grouped-by-fulfillment-center\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2026-01/inventory-level/{inventoryId}/locations\n  method: get\n  operationId: get-inventory-levels-grouped-by-fulfillment-center\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2026-01/inventory-level/lots\n  method: get\n  operationId: get-all-inventory-levels-grouped-by-lot\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2026-01/inventory-level/{inventoryId}/lots\n  method: get\n  operationId: get-inventory-levels-grouped-by-lot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2026-01/receiving\n  method: post\n  operationId: create-warehouse-receiving-order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2026-01/receiving\n  method: get\n  operationId: get-multiple-warehouse-receiving-orders\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2026-01/receiving/{id}\n  method: get\n  operationId: get-warehouse-receiving-order\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2026-01/fulfillment-center\n  method: get\n  operationId: get-fulfillment-centers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2026-01/receiving/{id}/boxes\n  method: get\n  operationId: get-warehouse-receiving-order-boxes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2026-01/receiving/{id}/labels\n  method: get\n  operationId: get-warehouse-receiving-order-box-labels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n   \
  \ subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2026-01/receiving/{id}:cancel\n  method: post\n  operationId: cancel-warehouse-receiving-order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2026-01/receiving:setExternalSync\n  method: post\n  operationId: set-external-sync-flag-for-wros\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2026-01/receiving/{id}/distributions\n  method: get\n  operationId: get-inventory-distributions-by-wro-id\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2026-01/return\n  method: post\n  operationId: create-return-order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2026-01/return\n  method: get\n  operationId: get-return-orders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2026-01/return/{id}\n  method: get\n  operationId: get-return-order\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /2026-01/return/{id}\n  method: put\n  operationId: edit-return-order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2026-01/return/{id}:cancel\n  method: post\n  operationId: cancel-return-order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2026-01/webhook\n  method: post\n  operationId: create-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2026-01/webhook\n  method: get\n  operationId: get-subscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2026-01/webhook/{id}\n  method: delete\n  operationId: delete-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2026-01/location\n  method: get\n  operationId: get-locations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2026-01/transactions:query\n\
  \  method: post\n  operationId: search-transactions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2026-01/invoices\n  method: get\n  operationId: get-invoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2026-01/invoices/{invoiceId}/transactions\n  method: get\n  operationId: get-transactions-by-invoice-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2026-01/transaction-fees\n  method: get\n  operationId: get-transaction-fees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /2026-01/simulate/shipment\n  method: post\n  operationId: simulates-shipment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2026-01/simulate/status/{simulationId}\n  method: get\n  operationId: get-simulation-status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shipbob/refs/heads/main/agentic-access/shipbob-agentic-access.yml
summary_line: 72 operations · 30 acting
tags:
- Logistics
- Fulfillment
- 3PL
- Ecommerce
- Inventory
- Warehousing
- Shipping
- Direct-to-Consumer
---
