---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 13
api_specs:
- filename: ordergroove-openapi.yml
  format: yaml
  label: Ordergroove Subscriptions API
  slug: ordergroove-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordergroove/refs/heads/main/openapi/ordergroove-openapi.yml
- filename: ordergroove-openapi.yml
  format: yaml
  label: Ordergroove Customers API
  slug: ordergroove-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordergroove/refs/heads/main/openapi/ordergroove-openapi.yml
- filename: ordergroove-openapi.yml
  format: yaml
  label: Ordergroove Orders API
  slug: ordergroove-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordergroove/refs/heads/main/openapi/ordergroove-openapi.yml
- filename: ordergroove-openapi.yml
  format: yaml
  label: Ordergroove Items API
  slug: ordergroove-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordergroove/refs/heads/main/openapi/ordergroove-openapi.yml
- filename: ordergroove-openapi.yml
  format: yaml
  label: Ordergroove Products API
  slug: ordergroove-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordergroove/refs/heads/main/openapi/ordergroove-openapi.yml
- filename: ordergroove-openapi.yml
  format: yaml
  label: Ordergroove Offers and Incentives API
  slug: ordergroove-offers-incentives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordergroove/refs/heads/main/openapi/ordergroove-openapi.yml
- filename: ordergroove-openapi.yml
  format: yaml
  label: Ordergroove Webhooks API
  slug: ordergroove-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordergroove/refs/heads/main/openapi/ordergroove-openapi.yml
consequence_counts:
  physical: 2
  read: 13
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ordergroove Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/{public_id}/cancel/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/{public_id}/send_now/
operation_count: 25
overview: 'Ordergroove exposes 25 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read, 10 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Ordergroove
provider_slug: ordergroove
slug: ordergroove-agentic-access
source_filename: ordergroove-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/ordergroove-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 25\n  by_action_class:\n    connected: 13\n    acting: 12\n  by_consequence:\n    read: 13\n    write: 10\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /subscriptions/\n  method: get\n  operationId: listSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions/{public_id}/\n  method: get\n  operationId: retrieveSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /subscriptions/{public_id}/\n  method: put\n  operationId: updateSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/{public_id}/cancel/\n  method: post\n  operationId: cancelSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/{public_id}/reactivate/\n  method: post\n  operationId: reactivateSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/{public_id}/change_frequency/\n  method: post\n  operationId: changeSubscriptionFrequency\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/\n  method: get\n  operationId: listCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/\n  method: post\n  operationId: createCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{public_id}/\n  method: get\n  operationId: retrieveCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{public_id}/\n  method: put\n  operationId: updateCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/\n  method: get\n  operationId: listOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{public_id}/\n  method: get\n  operationId: retrieveOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{public_id}/cancel/\n  method: post\n  operationId: cancelOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{public_id}/send_now/\n  method: post\n  operationId: sendOrderNow\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /items/\n  method: get\n  operationId: listItems\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /items/\n  method: post\n  operationId: createItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /items/{public_id}/\n  method: get\n  operationId: retrieveItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /items/{public_id}/\n  method: delete\n  operationId: deleteItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /products/\n  method: get\n  operationId: listProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/{id}/\n  method: get\n  operationId: retrieveProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/{id}/\n  method: put\n  operationId: updateProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /offer_profiles/\n  method: get\n  operationId: listOfferProfiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /otd/\n  method: get\n  operationId: listOneTimeDiscounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /otd/\n  method: post\n  operationId: createOneTimeDiscount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /entitlements/\n  method: get\n  operationId: listEntitlements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ordergroove/refs/heads/main/agentic-access/ordergroove-agentic-access.yml
summary_line: 25 operations · 12 acting
tags:
- Subscriptions
- Recurring Commerce
- Relationship Commerce
- eCommerce
- Autoship
- DTC
- Retail
- Subscription Management
---
