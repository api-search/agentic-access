---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 13
api_specs:
- filename: komerce-shipping-cost-openapi.yml
  format: yaml
  label: RajaOngkir Shipping Cost API
  slug: shipping-cost
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/komerce/refs/heads/main/openapi/komerce-shipping-cost-openapi.yml
- filename: komerce-shipping-delivery-openapi.yml
  format: yaml
  label: Komerce Shipping Delivery API (Komship)
  slug: shipping-delivery
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/komerce/refs/heads/main/openapi/komerce-shipping-delivery-openapi.yml
- filename: komerce-payment-openapi.yml
  format: yaml
  label: Komerce Payment Service API
  slug: payment
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/komerce/refs/heads/main/openapi/komerce-payment-openapi.yml
- filename: komerce-qrisly-openapi.yml
  format: yaml
  label: Komerce QRISLY API
  slug: qrisly
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/komerce/refs/heads/main/openapi/komerce-qrisly-openapi.yml
consequence_counts:
  physical: 8
  read: 13
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Komerce Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/user/payment/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/user/payment/create
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /calculate/domestic-cost
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /calculate/international-cost
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /order/api/v1/orders/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /order/api/v1/orders/print-label
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /order/api/v1/orders/store
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /order/api/v1/pickup/request
operation_count: 25
overview: 'Komerce exposes 25 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read, 4 write, and 8 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Komerce
provider_slug: komerce
slug: komerce-agentic-access
source_filename: komerce-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/komerce-payment-openapi.yml, openapi/komerce-qrisly-openapi.yml, openapi/komerce-shipping-cost-openapi.yml,\n  openapi/komerce-shipping-delivery-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 25\n  by_action_class:\n    connected: 13\n    acting: 12\n  by_consequence:\n    read: 13\n    physical: 8\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/user/methods\n  method: get\n  operationId: getPaymentMethods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/user/payment/create\n  method: post\n  operationId: createPayment\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/user/payment/status/{payment_id}\n  method: get\n  operationId: getPaymentStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/user/payment/cancel\n  method: post\n  operationId: cancelPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/qrisly/upload-qris\n\
  \  method: post\n  operationId: uploadQris\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/qrisly/generate-qris\n  method: post\n  operationId: generateQris\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/qrisly/payment-status/{history_id}\n  method: get\n  operationId: getQrisPaymentStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /destination/domestic-destination\n  method: get\n  operationId:\
  \ searchDomesticDestination\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /destination/international-destination\n  method: get\n  operationId: searchInternationalDestination\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calculate/domestic-cost\n  method: post\n  operationId: calculateDomesticCost\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calculate/international-cost\n  method: post\n  operationId: calculateInternationalCost\n  x-agentic-access:\n    action-class: acting\n   \
  \ consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /track/waybill\n  method: post\n  operationId: trackWaybill\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /destination/province\n  method: get\n  operationId: listProvinces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /destination/city/{province_id}\n  method: get\n  operationId: listCities\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /destination/district/{city_id}\n  method: get\n  operationId: listDistricts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /destination/sub-district/{district_id}\n  method: get\n  operationId: listSubdistricts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calculate/district/domestic-cost\n  method: post\n  operationId: calculateDistrictDomesticCost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tariff/api/v1/destination/search\n  method: get\n  operationId:\
  \ searchDeliveryDestination\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tariff/api/v1/calculate\n  method: get\n  operationId: calculateDeliveryPrice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /order/api/v1/orders/store\n  method: post\n  operationId: storeOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /order/api/v1/orders/cancel\n  method: put\n  operationId: cancelOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n  \
  \  audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /order/api/v1/orders/detail\n  method: get\n  operationId: getOrderDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /order/api/v1/orders/history-airway-bill\n  method: get\n  operationId: getAirwayBillHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /order/api/v1/orders/print-label\n  method: post\n  operationId: printOrderLabel\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /order/api/v1/pickup/request\n  method: post\n  operationId: requestPickup\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/komerce/refs/heads/main/agentic-access/komerce-agentic-access.yml
summary_line: 25 operations · 12 acting
tags:
- Company
- Shipping
- Logistics
- E-Commerce
- Payments
- QRIS
- Indonesia
- Couriers
- Tracking
- Fulfillment
---
