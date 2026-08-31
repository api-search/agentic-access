---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 7
api_specs:
- filename: barogo-areas-api-openapi.yml
  format: yaml
  label: Barogo Areas API
  slug: barogo-areas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barogo/refs/heads/main/openapi/barogo-areas-api-openapi.yml
- filename: barogo-delivery-api-openapi.yml
  format: yaml
  label: Barogo Delivery API
  slug: barogo-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barogo/refs/heads/main/openapi/barogo-delivery-api-openapi.yml
- filename: barogo-deposits-api-openapi.yml
  format: yaml
  label: Barogo Deposits API
  slug: barogo-deposits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barogo/refs/heads/main/openapi/barogo-deposits-api-openapi.yml
- filename: barogo-orders-api-openapi.yml
  format: yaml
  label: Barogo Orders API
  slug: barogo-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barogo/refs/heads/main/openapi/barogo-orders-api-openapi.yml
- filename: barogo-stores-api-openapi.yml
  format: yaml
  label: Barogo Stores API
  slug: barogo-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barogo/refs/heads/main/openapi/barogo-stores-api-openapi.yml
consequence_counts:
  physical: 12
  read: 7
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Barogo Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/delivery-possible
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/flexible/delivery-possible
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/flexible/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/flexible/orders/{orderAgencyOrderId}/delivery-price
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/orders/{orderAgencyOrderId}/drop-info
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/orders/{orderAgencyOrderId}/memo-info
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/orders/{orderAgencyOrderId}/payment-info
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/orders/{orderAgencyOrderId}/phone-info
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/orders/{orderAgencyOrderId}/pickup-wish-at
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/orders/{orderAgencyOrderId}/prepare-complete
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/orders/{orderAgencyOrderId}/status/cancel
operation_count: 21
overview: 'Barogo exposes 21 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read, 2 write, and 12 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Barogo
provider_slug: barogo
slug: barogo-agentic-access
source_filename: barogo-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: generated\nsource: openapi/barogo-gorela-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    connected: 7\n    acting: 14\n  by_consequence:\n    read: 7\n    physical: 12\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/delivery-conditions\n  method: get\n  operationId: getDeliveryAgencyConditions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/delivery-possible\n  method: post\n  operationId: checkDeliveryPossible\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/deposit-infos\n  method: get\n  operationId: getStoreDepositInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/flexible/delivery-possible\n  method: post\n  operationId: checkFlexibleDeliveryPossible\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/flexible/orders\n  method: post\n  operationId: createFlexibleOrder\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/flexible/orders/{orderAgencyOrderId}/delivery-price\n  method: put\n  operationId: updateFlexibleOrderDeliveryPrice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/order-agency-stores/{orderAgencyStoreId}/areas\n  method: get\n  operationId: getStoreAreas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/orders\n\
  \  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/orders\n  method: get\n  operationId: listOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/orders/{orderAgencyOrderId}\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/orders/{orderAgencyOrderId}/drop-info\n  method: put\n  operationId: updateOrderDropInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/orders/{orderAgencyOrderId}/memo-info\n  method: put\n  operationId: updateOrderMemoInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/orders/{orderAgencyOrderId}/payment-info\n  method: put\n  operationId: updateOrderPaymentInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/orders/{orderAgencyOrderId}/phone-info\n  method: put\n  operationId: updateOrderPhoneInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/orders/{orderAgencyOrderId}/pickup-wish-at\n  method: put\n  operationId: updateOrderPickupWishAt\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /api/orders/{orderAgencyOrderId}/prepare-complete\n  method: post\n  operationId: markOrderPrepareComplete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/orders/{orderAgencyOrderId}/status/cancel\n  method: put\n  operationId: cancelOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/store-mapping\n  method: post\n  operationId: createStoreMapping\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/store-mapping/pause\n  method: put\n  operationId: pauseStoreMapping\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/store-mapping/{orderAgencyStoreId}\n  method: get\n  operationId: getStoreMapping\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/stores\n  method: get\n  operationId: listStores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/barogo/refs/heads/main/agentic-access/barogo-agentic-access.yml
summary_line: 21 operations · 14 acting
tags:
- Company
- Delivery
- Logistics
- Last Mile Delivery
- Food Delivery
- Courier
- Fulfillment
- Order
- Webhook
- South Korea
- Transportation
- Marketplace
---
