---
acting_count: 20
action_class_counts:
  acting: 20
  connected: 11
api_specs:
- filename: topi-seller-api-openapi-original.yaml
  format: yaml
  label: topi Seller API
  slug: topi-seller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/topi/refs/heads/main/openapi/topi-seller-api-openapi-original.yaml
consequence_counts:
  physical: 6
  read: 11
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Topi Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/orders/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/orders/{id}/accept
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/orders/{id}/acknowledge
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/orders/{id}/reject
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/shipment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/shipping-method/method
operation_count: 31
overview: 'Topi exposes 31 API operations that an AI agent could call, of which 20 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 14 write, and 6 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Topi
provider_slug: topi
slug: topi-agentic-access
source_filename: topi-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/topi-seller-api-openapi-original.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 31\n  by_action_class:\n    acting: 20\n    connected: 11\n  by_consequence:\n    write: 14\n    read: 11\n    physical: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/catalog/basket/pricing\n  method: post\n  operationId: catalog#calculateBasketPricing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - seller-catalog:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/catalog/carts/rental-overview\n\
  \  method: post\n  operationId: catalog#cartRentalOverview\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - seller-catalog:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/catalog/check-supported\n  method: post\n  operationId: catalog#checkSupported\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - seller-catalog:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/catalog/import\n  method: post\n  operationId: catalog#importCatalog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - seller-catalog:edit\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/catalog/imports\n  method: post\n  operationId: catalog#createImport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - seller-catalog:edit\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/catalog/imports/{id}\n  method: delete\n  operationId: catalog#cancelImport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - seller-catalog:edit\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/catalog/imports/{id}\n\
  \  method: get\n  operationId: catalog#getImport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - seller-catalog:edit\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/catalog/list-recommended-rental-prices\n  method: post\n  operationId: catalog#listRecommendedRentalPrices\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - seller-catalog:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/catalog/pricing\n  method: post\n  operationId: catalog#calculatePricing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - seller-catalog:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n  \
  \    triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/catalog/products\n  method: get\n  operationId: catalog#searchProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - seller-catalog:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/catalog/products_paginated\n  method: get\n  operationId: catalog#searchProductsPaginated\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - seller-catalog:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/catalog/products_paginated\n  method: post\n  operationId: catalog#searchAndFilterProductsPaginated\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - seller-catalog:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/offers\n  method: get\n  operationId: offer#listOffers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - seller-offer:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/offers\n  method: post\n  operationId: offer#create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - seller-offer:edit\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/offers/{id}\n  method: get\n  operationId: offer#show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - seller-offer:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/offers/{id}\n  method: put\n  operationId: offer#edit\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - seller-offer:edit\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/offers/{id}/void\n  method: post\n  operationId: offer#void\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - seller-offer:edit\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/offers/paginated\n  method: get\n  operationId: offer#listOffersPaginated\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - seller-offer:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/offers/partners\n\
  \  method: post\n  operationId: offer#createForPartner\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - seller-offer:edit\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/offers/ref/{seller_offer_reference}\n  method: get\n  operationId: offer#showByReference\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - seller-offer:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/offers/validate\n  method: post\n  operationId: offer#validate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - seller-offer:edit\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/orders\n  method: get\n  operationId: order#getBySeller\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - seller-order:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/orders/{id}\n  method: get\n  operationId: order#show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - seller-order:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/orders/{id}\n  method: patch\n  operationId: order#setMetadata\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - seller-order:edit\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/orders/{id}/accept\n\
  \  method: post\n  operationId: order#acceptOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - seller-order:edit\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/orders/{id}/acknowledge\n  method: post\n  operationId: order#acknowledgeOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - seller-order:edit\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/orders/{id}/reject\n  method: post\n  operationId: order#rejectOrder\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    scope:\n    - seller-order:edit\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/orders/paginated\n  method: get\n  operationId: order#getBySellerPaginated\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - seller-order:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/shipment\n  method: post\n  operationId: shipment#create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - seller-shipment:edit\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/shipping-method\n  method: get\n  operationId: shippingMethod#getShippingMethods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - seller-shipping-method:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/shipping-method/method\n  method: post\n  operationId: shippingMethod#create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - seller-shipping-method:edit\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/topi/refs/heads/main/agentic-access/topi-agentic-access.yml
summary_line: 31 operations · 20 acting
tags:
- Company
- Fintech
- Hardware as a Service
- Rental
- Embedded Finance
- B2B Payments
- Financing
- Checkout
- Germany
- API
---
