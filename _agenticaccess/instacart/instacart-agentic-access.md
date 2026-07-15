---
acting_count: 19
action_class_counts:
  acting: 19
  connected: 4
api_specs:
- filename: instacart-developer-platform-api-openapi.yml
  format: yaml
  label: Instacart Developer Platform API
  slug: developer-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instacart/refs/heads/main/openapi/instacart-developer-platform-api-openapi.yml
- filename: instacart-connect-fulfillment-api-openapi.yml
  format: yaml
  label: Instacart Connect Fulfillment API
  slug: connect-fulfillment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instacart/refs/heads/main/openapi/instacart-connect-fulfillment-api-openapi.yml
- filename: instacart-connect-post-checkout-api-openapi.yml
  format: yaml
  label: Instacart Connect Post-Checkout API
  slug: connect-post-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instacart/refs/heads/main/openapi/instacart-connect-post-checkout-api-openapi.yml
- filename: instacart-catalog-api-openapi.yml
  format: yaml
  label: Instacart Catalog API
  slug: catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instacart/refs/heads/main/openapi/instacart-catalog-api-openapi.yml
consequence_counts:
  physical: 14
  read: 4
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Instacart Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/fulfillment/lastmile/orders/{order_id}/staged
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/fulfillment/lastmile/users/{user_id}/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/fulfillment/lastmile/users/{user_id}/service_options
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/fulfillment/stores/delivery
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/fulfillment/stores/last_mile
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/fulfillment/stores/pickup
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/fulfillment/users/{user_id}/orders/delivery
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/fulfillment/users/{user_id}/orders/pickup
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/fulfillment/users/{user_id}/orders/{order_id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/fulfillment/users/{user_id}/service_options/delivery
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/fulfillment/users/{user_id}/service_options/delivery/hold
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/fulfillment/users/{user_id}/service_options/pickup
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/post_checkout/chat/{order_id}/messages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v2/post_checkout/orders/{order_id}/items/{order_item_id}/replacement
operation_count: 23
overview: 'instacart exposes 23 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read, 5 write, and 14 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: instacart
provider_slug: instacart
slug: instacart-agentic-access
source_filename: instacart-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/instacart-catalog-api-openapi.yml, openapi/instacart-connect-fulfillment-api-openapi.yml,\n  openapi/instacart-connect-post-checkout-api-openapi.yml, openapi/instacart-developer-platform-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    acting: 19\n    connected: 4\n  by_consequence:\n    write: 5\n    physical: 14\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/data_ingestion/catalog/product/submission\n  method: post\n  operationId: submitProducts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/data_ingestion/catalog/item/submission\n  method: post\n  operationId: submitItems\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/oauth/token\n  method: post\n  operationId: generateAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/fulfillment/stores/delivery\n  method: post\n  operationId: findDeliveryStores\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/fulfillment/users/{user_id}/service_options/delivery\n  method: post\n  operationId: previewDeliveryTimeSlots\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/fulfillment/users/{user_id}/service_options/delivery/hold\n  method: post\n  operationId: reserveDeliveryTimeSlot\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/fulfillment/users/{user_id}/orders/delivery\n  method: post\n  operationId: createDeliveryOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/fulfillment/users/{user_id}/orders/{order_id}\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/fulfillment/users/{user_id}/orders/{order_id}/cancel\n  method: post\n  operationId: cancelOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/fulfillment/stores/pickup\n  method: post\n  operationId: findPickupStores\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/fulfillment/users/{user_id}/service_options/pickup\n  method: post\n  operationId: previewPickupTimeSlots\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/fulfillment/users/{user_id}/orders/pickup\n  method: post\n  operationId: createPickupOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/fulfillment/stores/last_mile\n  method: post\n  operationId: findLastMileStores\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /v2/fulfillment/lastmile/users/{user_id}/service_options\n  method: post\n  operationId: previewLastMileServiceOptions\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/fulfillment/lastmile/users/{user_id}/orders\n  method: post\n  operationId: createLastMileOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/fulfillment/lastmile/orders/{order_id}/staged\n  method: post\n  operationId: stageLastMileOrder\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/post_checkout/orders/{order_id}/handling\n  method: get\n  operationId: getOrderHandling\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/post_checkout/orders/{order_id}/items\n  method: get\n  operationId: getOrderItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/post_checkout/orders/{order_id}/items/{order_item_id}/replacement\n  method: put\n  operationId: updateItemReplacement\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/post_checkout/chat/{order_id}/messages\n  method: get\n  operationId: getChatMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/post_checkout/chat/{order_id}/messages\n  method: post\n  operationId: sendChatMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /idp/v1/products/products_link\n\
  \  method: post\n  operationId: createShoppingListPage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /idp/v1/products/recipe\n  method: post\n  operationId: createRecipePage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instacart/refs/heads/main/agentic-access/instacart-agentic-access.yml
summary_line: 23 operations · 19 acting
tags: []
---
