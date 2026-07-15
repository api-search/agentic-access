---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 4
api_specs:
- filename: opencart-rest-api.yml
  format: yaml
  label: OpenCart REST API
  slug: opencart-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opencart/refs/heads/main/openapi/opencart-rest-api.yml
consequence_counts:
  physical: 7
  read: 4
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Opencart Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment_address
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment_address/setAddress
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment_method
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /shipping_address
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /shipping_method
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /subscription
operation_count: 16
overview: 'OpenCart exposes 16 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read, 5 write, and 7 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: OpenCart
provider_slug: opencart
slug: opencart-agentic-access
source_filename: opencart-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/opencart-rest-api.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    acting: 12\n    connected: 4\n  by_consequence:\n    write: 5\n    read: 4\n    physical: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /login\n  method: post\n  operationId: apiLogin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cart\n  method: post\n  operationId: addProductsToCart\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cart/addProduct\n  method: post\n  operationId: addSingleProductToCart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cart/getProducts\n  method: get\n  operationId: getCartProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cart/getTotals\n  method: get\n  operationId: getCartTotals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /customer\n  method: post\n  operationId: setCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment_address\n  method: post\n  operationId: setPaymentAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment_address/setAddress\n  method: post\n  operationId: setPaymentAddressById\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n   \
  \   exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shipping_address\n  method: post\n  operationId: setShippingAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shipping_method\n  method: post\n  operationId: setShippingMethod\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /shipping_method/getShippingMethods\n  method: get\n  operationId: getShippingMethods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment_method\n  method: post\n  operationId: setPaymentMethod\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment_method/getPaymentMethods\n  method: get\n  operationId: getPaymentMethods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /order\n  method: post\n  operationId: manageOrder\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /affiliate\n  method: post\n  operationId: setAffiliate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscription\n  method: post\n  operationId: manageSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n  \
  \  audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opencart/refs/heads/main/agentic-access/opencart-agentic-access.yml
summary_line: 16 operations · 12 acting
tags:
- eCommerce
- Shopping Cart
- Open Source
- Self-Hosted
- Products
- Orders
- Customers
- Categories
---
