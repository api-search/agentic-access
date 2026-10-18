---
acting_count: 26
action_class_counts:
  acting: 26
  connected: 17
api_specs:
- filename: extend-claims-management-api-openapi.yml
  format: yaml
  label: Extend Claims Management API
  slug: extend-claims-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extend/refs/heads/main/openapi/extend-claims-management-api-openapi.yml
- filename: extend-contracts-api-openapi.yml
  format: yaml
  label: Extend Contracts API
  slug: extend-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extend/refs/heads/main/openapi/extend-contracts-api-openapi.yml
- filename: extend-leads-api-openapi.yml
  format: yaml
  label: Extend Leads API
  slug: extend-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extend/refs/heads/main/openapi/extend-leads-api-openapi.yml
- filename: extend-offers-api-openapi.yml
  format: yaml
  label: Extend Offers API
  slug: extend-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extend/refs/heads/main/openapi/extend-offers-api-openapi.yml
- filename: extend-orders-api-openapi.yml
  format: yaml
  label: Extend Orders API
  slug: extend-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extend/refs/heads/main/openapi/extend-orders-api-openapi.yml
- filename: extend-products-api-openapi.yml
  format: yaml
  label: Extend Products API
  slug: extend-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extend/refs/heads/main/openapi/extend-products-api-openapi.yml
- filename: extend-refunds-api-openapi.yml
  format: yaml
  label: Extend Refunds API
  slug: extend-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extend/refs/heads/main/openapi/extend-refunds-api-openapi.yml
- filename: extend-service-orders-api-openapi.yml
  format: yaml
  label: Extend Service Orders API
  slug: extend-service-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extend/refs/heads/main/openapi/extend-service-orders-api-openapi.yml
- filename: extend-dynamic-return-policy-api-openapi.yml
  format: yaml
  label: Extend Dynamic Return Policy API
  slug: extend-dynamic-return-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extend/refs/heads/main/openapi/extend-dynamic-return-policy-api-openapi.yml
- filename: extend-line-items-api-openapi.yml
  format: yaml
  label: Extend Line Items API
  slug: extend-line-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extend/refs/heads/main/openapi/extend-line-items-api-openapi.yml
- filename: extend-shippingoffers-api-openapi.yml
  format: yaml
  label: Extend Shipping Offers API
  slug: extend-shippingoffers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extend/refs/heads/main/openapi/extend-shippingoffers-api-openapi.yml
- filename: extend-webhooks-api-openapi.yml
  format: yaml
  label: Extend Webhooks API
  slug: extend-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extend/refs/heads/main/openapi/extend-webhooks-api-openapi.yml
consequence_counts:
  physical: 21
  read: 17
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Extend Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /line-items/fulfill
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /line-items/shipments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /line-items/shipments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /line-items/shipments/delete
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /line-items/{lineItemId}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/batch
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/batch?historical
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/{orderId}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/{orderId}/line-item
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /refunds
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /service-orders/service-claim
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /service-orders/{serviceOrderId}/accept-repair
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /service-orders/{serviceOrderId}/expenses
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /service-orders/{serviceOrderId}/expenses/{expenseId}/void
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /service-orders/{serviceOrderId}/fulfill
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /service-orders/{serviceOrderId}/generate-repair-label
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /service-orders/{serviceOrderId}/request-payment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /service-orders/{serviceOrderId}/update-repair
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /shipping-offers/quotes
operation_count: 43
overview: 'Extend exposes 43 API operations that an AI agent could call, of which 26 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read, 5 write, and 21 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Extend
provider_slug: extend
slug: extend-agentic-access
source_filename: extend-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: generated\nsource: openapi/extend-claims-management-api-openapi.yml, openapi/extend-contracts-api-openapi.yml,\n  openapi/extend-entitlements-api-openapi.yml, openapi/extend-leads-api-openapi.yml, openapi/extend-offers-api-openapi.yml,\n  openapi/extend-orders-api-openapi.yml, openapi/extend-products-api-openapi.yml, openapi/extend-refunds-api-openapi.yml,\n  openapi/extend-service-orders-api-openapi.yml, openapi/extend-shipping-offers-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 43\n  by_action_class:\n    connected: 17\n    acting: 26\n  by_consequence:\n    read: 17\n    write: 5\n    physical: 21\n  human_in_the_loop_required: 0\noperations:\n- path: /claims-management/claims/{claimId}/photos\n\
  \  method: get\n  operationId: claimPhotosList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/claims\n  method: post\n  operationId: claimWebhookNotification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/search\n  method: get\n  operationId: contractsSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts/{contractId}\n  method: get\n  operationId: contractsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /contracts/{contractId}\n  method: put\n  operationId: contractsUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /entitlements-management/dynamic-return-policy-content\n  method: post\n  operationId: fetchDynamicReturnPolicyContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leads\n  method: post\n  operationId: createLead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /leads/offers\n  method: get\n\
  \  operationId: contractLeadsOffersBatchGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leads/{leadToken}/offers\n  method: get\n  operationId: contractLeadsOfferGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /offers\n  method: get\n  operationId: getOffer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /line-items/fulfill\n  method: post\n  operationId: lineItemsFulfill\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n  \
  \    - high-value\n    audit: required\n- path: /line-items/search\n  method: get\n  operationId: lineItemsSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /line-items/shipments\n  method: put\n  operationId: lineItemsShipmentUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /line-items/shipments\n  method: post\n  operationId: lineItemsShipmentAdd\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /line-items/shipments/delete\n  method: post\n  operationId: lineItemsShipmentDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /line-items/{lineItemId}\n  method: get\n  operationId: ordersGetLineItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /line-items/{lineItemId}/cancel\n  method: post\n  operationId: lineItemsCancel\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders\n  method: post\n  operationId: ordersCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders\n  method: put\n  operationId: ordersUpsert\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/batch\n  method: post\n  operationId:\
  \ ordersBatchCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/batch?historical\n  method: post\n  operationId: ordersBatchCreateHistorical\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/search\n  method: get\n  operationId: ordersSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /orders/{orderId}\n  method: get\n  operationId: ordersGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{orderId}/cancel\n  method: post\n  operationId: ordersCancel\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{orderId}/line-item\n  method: post\n  operationId: ordersAddLineItem\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n  \
  \    - high-value\n    audit: required\n- path: /stores/{storeId}/products\n  method: post\n  operationId: storesProductsCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stores/{storeId}/products/{productId}\n  method: get\n  operationId: storesProductsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stores/{storeId}/products/{productId}\n  method: delete\n  operationId: storesProductsDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /refunds\n  method: post\n  operationId: refundsCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service-orders/search\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /service-orders/service-claim\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /service-orders/{serviceOrderId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /service-orders/{serviceOrderId}/accept-repair\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service-orders/{serviceOrderId}/expenses\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /service-orders/{serviceOrderId}/expenses\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service-orders/{serviceOrderId}/expenses/{expenseId}/void\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service-orders/{serviceOrderId}/fulfill\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /service-orders/{serviceOrderId}/generate-repair-label\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service-orders/{serviceOrderId}/request-payment\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service-orders/{serviceOrderId}/update-repair\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shipping-offers/config\n  method: get\n  operationId: shippingOffersConfigGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shipping-offers/config/marketing\n  method: get\n  operationId: shippingOffersMarketingGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shipping-offers/quotes\n  method: post\n  operationId: shippingOffersQuoteCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/extend/refs/heads/main/agentic-access/extend-agentic-access.yml
summary_line: 43 operations · 26 acting
tags:
- Company
- Consumer
- Product Protection
- Extended Warranty
- Shipping Protection
- E-Commerce
- Warranty
- Claims
- Contracts
- Retail
- Insurance
---
