---
acting_count: 23
action_class_counts:
  acting: 23
  connected: 15
api_specs:
- filename: finditparts-addresses-api-openapi.yml
  format: yaml
  label: FinditParts Addresses API
  slug: finditparts-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finditparts/refs/heads/main/openapi/finditparts-addresses-api-openapi.yml
- filename: finditparts-carts-api-openapi.yml
  format: yaml
  label: FinditParts Carts API
  slug: finditparts-carts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finditparts/refs/heads/main/openapi/finditparts-carts-api-openapi.yml
- filename: finditparts-orders-api-openapi.yml
  format: yaml
  label: FinditParts Orders API
  slug: finditparts-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finditparts/refs/heads/main/openapi/finditparts-orders-api-openapi.yml
- filename: finditparts-partners-api-openapi.yml
  format: yaml
  label: FinditParts Partners API
  slug: finditparts-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finditparts/refs/heads/main/openapi/finditparts-partners-api-openapi.yml
- filename: finditparts-products-api-openapi.yml
  format: yaml
  label: FinditParts Products API
  slug: finditparts-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finditparts/refs/heads/main/openapi/finditparts-products-api-openapi.yml
- filename: finditparts-reseller-customer-sessions-api-openapi.yml
  format: yaml
  label: FinditParts Reseller Customer Sessions API
  slug: finditparts-reseller-customer-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finditparts/refs/heads/main/openapi/finditparts-reseller-customer-sessions-api-openapi.yml
- filename: finditparts-reseller-customers-api-openapi.yml
  format: yaml
  label: FinditParts Reseller Customers API
  slug: finditparts-reseller-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finditparts/refs/heads/main/openapi/finditparts-reseller-customers-api-openapi.yml
- filename: finditparts-sessions-api-openapi.yml
  format: yaml
  label: FinditParts Sessions API
  slug: finditparts-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finditparts/refs/heads/main/openapi/finditparts-sessions-api-openapi.yml
- filename: finditparts-shipping-api-openapi.yml
  format: yaml
  label: FinditParts Shipping API
  slug: finditparts-shipping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finditparts/refs/heads/main/openapi/finditparts-shipping-api-openapi.yml
- filename: finditparts-users-api-openapi.yml
  format: yaml
  label: FinditParts Users API
  slug: finditparts-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finditparts/refs/heads/main/openapi/finditparts-users-api-openapi.yml
- filename: finditparts-variants-api-openapi.yml
  format: yaml
  label: FinditParts Variants API
  slug: finditparts-variants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finditparts/refs/heads/main/openapi/finditparts-variants-api-openapi.yml
consequence_counts:
  physical: 6
  read: 15
  write: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Finditparts Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /carts/{cart_id}/complete_with_corporate_billing
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /carts/{cart_id}/complete_with_credit_card
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /carts/{cart_id}/shipping_address
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /carts/{cart_id}/shipping_methods
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /partners/place_order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /partners/shipping_methods
operation_count: 38
overview: 'FinditParts exposes 38 API operations that an AI agent could call, of which 23 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read, 17 write, and 6 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: FinditParts
provider_slug: finditparts
slug: finditparts-agentic-access
source_filename: finditparts-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: generated\nsource: openapi/finditparts-reseller-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 38\n  by_action_class:\n    connected: 15\n    acting: 23\n  by_consequence:\n    read: 15\n    write: 17\n    physical: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /products/{product_id}\n  method: get\n  operationId: getProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/{product_ids}/multi\n  method: get\n  operationId: getProductsMulti\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /products/lookup\n  method: get\n  operationId: lookupProductByPartNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products\n  method: get\n  operationId: productSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /variants/{variant_ids}\n  method: get\n  operationId: variantLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shipping_methods\n  method: get\n  operationId: shippingMethods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reseller_customer_sessions/{reseller_customer_session_id}\n  method: get\n  operationId: getResellerCustomerSession\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reseller_customer_sessions/{reseller_customer_session_id}\n  method: delete\n  operationId: cancelResellerCustomerSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reseller_customer_sessions\n  method: post\n  operationId: createResellerCustomerSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/refresh\n  method: post\n  operationId: refreshSession\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/current\n  method: get\n  operationId: getCurrentSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions\n  method: post\n  operationId: createSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions\n  method: delete\n  operationId: destroySessions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reseller_customers\n  method: post\n  operationId: createResellerCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reseller_customers\n  method: get\n  operationId: listResellerCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users\n  method: post\n  operationId: createUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n    \
  \  human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partners/shipping_methods\n  method: post\n  operationId: partnersShippingMethods\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partners/place_order\n  method: post\n  operationId: partnersPlaceOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/search\n  method: get\n  operationId:\
  \ searchOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{order_id}\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders\n  method: get\n  operationId: listOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /addresses/{address_id}/set_as_default\n  method: post\n  operationId: setDefaultAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /addresses/{address_id}\n  method: put\n\
  \  operationId: updateAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /addresses/{address_id}\n  method: delete\n  operationId: deleteAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /addresses\n  method: get\n  operationId: listAddresses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /addresses\n  method: post\n  operationId: createAddress\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /carts/{cart_id}/line_items\n  method: post\n  operationId: addCartLineItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /carts/{cart_id}/line_items\n  method: put\n  operationId: changeCartLineItems\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /carts/{cart_id}/shipping_methods\n  method: get\n\
  \  operationId: getCartShippingMethods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /carts/{cart_id}/shipping_methods\n  method: put\n  operationId: selectCartShippingMethod\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /carts/{cart_id}/shipping_address\n  method: put\n  operationId: setCartShippingAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /carts/{cart_id}/billing_address\n  method: put\n  operationId: setCartBillingAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /carts/{cart_id}/coupon\n  method: put\n  operationId: setCartCoupon\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /carts/{cart_id}/po_number\n  method: put\n  operationId: setCartPoNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n \
  \   escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /carts/{cart_id}/complete_with_credit_card\n  method: post\n  operationId: completeCartWithCreditCard\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /carts/{cart_id}/complete_with_corporate_billing\n  method: post\n  operationId: completeCartWithCorporateBilling\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /carts/{cart_id}\n  method: get\n  operationId: getCart\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /carts\n  method: post\n  operationId: createCart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finditparts/refs/heads/main/agentic-access/finditparts-agentic-access.yml
summary_line: 38 operations · 23 acting
tags:
- Company
- E-Commerce
- Marketplace
- Automotive
- Parts
- Heavy Duty Trucking
- Fleet
- Logistics
- Commerce
- Catalog
- Order
- Shipping
---
