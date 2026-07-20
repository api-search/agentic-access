---
acting_count: 22
action_class_counts:
  acting: 22
  connected: 11
api_specs:
- filename: kurly-kls-fulfillment-openapi.yml
  format: yaml
  label: Kurly Logistics Services (KLS) Fulfillment API
  slug: kurly-logistics-services-kls-fulfillment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kurly/refs/heads/main/openapi/kurly-kls-fulfillment-openapi.yml
- filename: kurly-kls-delivery-agency-openapi.yml
  format: yaml
  label: Kurly Logistics Services (KLS) Delivery Agency API
  slug: kurly-logistics-services-kls-delivery-agency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kurly/refs/heads/main/openapi/kurly-kls-delivery-agency-openapi.yml
- filename: kurly-kls-delivery-tracking-openapi.yml
  format: yaml
  label: Kurly Logistics Services (KLS) Delivery Tracking API
  slug: kurly-logistics-services-kls-delivery-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kurly/refs/heads/main/openapi/kurly-kls-delivery-tracking-openapi.yml
- filename: kurly-kls-auth-openapi.yml
  format: yaml
  label: Kurly Logistics Services (KLS) Authentication API
  slug: kurly-logistics-services-kls-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kurly/refs/heads/main/openapi/kurly-kls-auth-openapi.yml
consequence_counts:
  physical: 10
  read: 11
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Kurly Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/fulfillment/v1/operation-plans
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/fulfillment/v1/operation-plans/bulk
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/fulfillment/v2/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/fulfillment/v2/orders/bulk
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/fulfillment/v2/orders/bulk/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/fulfillment/v2/orders/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/invoices/print-data
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/orders/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/orders/cancel/by-request-key
operation_count: 33
overview: 'Kurly exposes 33 API operations that an AI agent could call, of which 22 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 12 write, and 10 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Kurly
provider_slug: kurly
slug: kurly-agentic-access
source_filename: kurly-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/kurly-kls-auth-openapi.yml, openapi/kurly-kls-delivery-agency-openapi.yml, openapi/kurly-kls-delivery-tracking-openapi.yml,\n  openapi/kurly-kls-fulfillment-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 33\n  by_action_class:\n    acting: 22\n    connected: 11\n  by_consequence:\n    write: 12\n    physical: 10\n    read: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /auth/token\n  method: post\n  operationId: issueToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n  \
  \    - high-value\n    audit: required\n- path: /api/delivery-agency/v1/delivery-policies\n  method: post\n  operationId: findDeliveryPolicies\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/invoices/print-data\n  method: post\n  operationId: findInvoicePrintData\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/orders\n  method: post\n  operationId: createDeliveryOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/orders\n  method: get\n  operationId: findDeliveryOrdersByClientOrderCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/orders/by-request-keys\n  method: get\n  operationId: findDeliveryOrdersByRequestKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/orders/cancel/by-request-key\n  method: post\n  operationId: cancelDeliveryOrderByRequestKey\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/orders/cancel\n  method: post\n  operationId: cancelDeliveryOrderByClientOrderCode\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/couriers/{courier}/trackings/{invoiceNumber}\n  method: get\n  operationId: findDeliveryTracking\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/goods/skus\n  method: post\n  operationId: saveSku\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/goods/skus\n  method: put\n  operationId: updateSku\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/goods/skus\n  method: get\n  operationId: findSkuList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/goods/sales-channel-mapping\n  method: get\n  operationId: findSalesChannelMappingList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/goods/sales-channel-mapping\n\
  \  method: post\n  operationId: saveSalesChannelMapping\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/goods/sales-channel-mapping\n  method: put\n  operationId: updateSalesChannelMapping\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/receiving-request/specification\n  method: get\n  operationId: downloadReceivingSpecification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/v1/receiving-request\n\
  \  method: post\n  operationId: createReceivingRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/receiving-request/cancel\n  method: patch\n  operationId: cancelReceivingRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/receiving-request/plans/search\n  method: post\n  operationId: searchReceivingPlans\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/receiving-request/reports/search\n  method: post\n  operationId: searchReceivingReports\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/receiving-request/items/status/search\n  method: post\n  operationId: searchReceivingItemStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/receiving-request/search\n  method: post\n  operationId: searchReceivingRequests\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/v1/receiving-request/receiving-label/print\n  method: get\n  operationId: printReceivingLabel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/lot-ledgers\n  method: get\n  operationId: findLotLedgers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ledgers\n  method: get\n  operationId: findLedgers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/inventories\n  method: get\n  operationId: findInventories\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/fulfillment/v2/orders/bulk\n  method: post\n  operationId: createOrdersBulkV2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/fulfillment/v2/orders\n  method: post\n  operationId: createOrderV2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/fulfillment/v1/orders\n\
  \  method: get\n  operationId: findOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/fulfillment/v2/orders/bulk/cancel\n  method: put\n  operationId: cancelOrdersBulkV2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/fulfillment/v2/orders/cancel\n  method: put\n  operationId: cancelOrderV2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n \
  \     - high-value\n    audit: required\n- path: /api/fulfillment/v1/operation-plans/bulk\n  method: post\n  operationId: findOperationPlansBulk\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/fulfillment/v1/operation-plans\n  method: post\n  operationId: findOperationPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kurly/refs/heads/main/agentic-access/kurly-agentic-access.yml
summary_line: 33 operations · 22 acting
tags:
- Company
- Technology
- Logistics
- Fulfillment
- Supply Chain
- Delivery
- Ecommerce
- Grocery
- Shipping
- Order Management
- Inventory
- Tracking
- South Korea
---
