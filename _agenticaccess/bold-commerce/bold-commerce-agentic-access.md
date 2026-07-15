---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 11
api_specs:
- filename: bold-commerce-openapi.yml
  format: yaml
  label: Bold Subscriptions API
  slug: bold-commerce-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bold-commerce/refs/heads/main/openapi/bold-commerce-openapi.yml
- filename: bold-commerce-openapi.yml
  format: yaml
  label: Bold Checkout API
  slug: bold-commerce-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bold-commerce/refs/heads/main/openapi/bold-commerce-openapi.yml
- filename: bold-commerce-openapi.yml
  format: yaml
  label: Bold Price Rules API
  slug: bold-commerce-price-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bold-commerce/refs/heads/main/openapi/bold-commerce-openapi.yml
- filename: bold-commerce-openapi.yml
  format: yaml
  label: Bold Products API
  slug: bold-commerce-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bold-commerce/refs/heads/main/openapi/bold-commerce-openapi.yml
- filename: bold-commerce-openapi.yml
  format: yaml
  label: Bold Customers API
  slug: bold-commerce-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bold-commerce/refs/heads/main/openapi/bold-commerce-openapi.yml
- filename: bold-commerce-openapi.yml
  format: yaml
  label: Bold Shops API
  slug: bold-commerce-shops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bold-commerce/refs/heads/main/openapi/bold-commerce-openapi.yml
consequence_counts:
  physical: 6
  read: 11
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bold Commerce Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkout/storefront/{shop_id}/{order_id}/addresses/billing
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkout/storefront/{shop_id}/{order_id}/addresses/shipping
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkout/storefront/{shop_id}/{order_id}/discounts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkout/storefront/{shop_id}/{order_id}/line_items
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkout/storefront/{shop_id}/{order_id}/payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /subscriptions/v1/shops/{shop_identifier}/subscriptions/{subscription_id}/orders/{order_id}/skip
operation_count: 29
overview: 'Bold Commerce exposes 29 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 12 write, and 6 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bold Commerce
provider_slug: bold-commerce
slug: bold-commerce-agentic-access
source_filename: bold-commerce-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/bold-commerce-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 29\n  by_action_class:\n    connected: 11\n    acting: 18\n  by_consequence:\n    read: 11\n    write: 12\n    physical: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /subscriptions/v1/shops/{shop_identifier}/subscriptions\n  method: get\n  operationId: listSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions/v1/shops/{shop_identifier}/subscriptions\n  method: post\n  operationId: createSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/v1/shops/{shop_identifier}/subscriptions/{subscription_id}\n  method: get\n  operationId: getSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions/v1/shops/{shop_identifier}/subscriptions/{subscription_id}\n  method: put\n  operationId: replaceSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/v1/shops/{shop_identifier}/subscriptions/{subscription_id}\n  method: patch\n  operationId:\
  \ patchSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/v1/shops/{shop_identifier}/subscriptions/{subscription_id}/pause\n  method: post\n  operationId: pauseSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/v1/shops/{shop_identifier}/subscriptions/{subscription_id}/cancel\n  method: post\n  operationId: cancelSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/v1/shops/{shop_identifier}/subscriptions/{subscription_id}/activate\n  method: post\n  operationId: activateSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/v1/shops/{shop_identifier}/subscriptions/{subscription_id}/line_items\n  method: post\n  operationId: addSubscriptionLineItems\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/v1/shops/{shop_identifier}/subscriptions/{subscription_id}/intervals\n\
  \  method: get\n  operationId: listSubscriptionIntervals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions/v1/shops/{shop_identifier}/subscriptions/{subscription_id}/orders\n  method: get\n  operationId: listSubscriptionOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions/v1/shops/{shop_identifier}/subscriptions/{subscription_id}/orders/{order_id}/skip\n  method: put\n  operationId: skipSubscriptionOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /checkout/storefront/{shop_id}/{order_id}/addresses/shipping\n\
  \  method: post\n  operationId: setShippingAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /checkout/storefront/{shop_id}/{order_id}/addresses/shipping\n  method: get\n  operationId: getShippingAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /checkout/storefront/{shop_id}/{order_id}/addresses/billing\n  method: post\n  operationId: setBillingAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /checkout/storefront/{shop_id}/{order_id}/line_items\n  method: post\n  operationId: addCheckoutLineItems\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /checkout/storefront/{shop_id}/{order_id}/discounts\n  method: post\n  operationId: applyCheckoutDiscount\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /checkout/storefront/{shop_id}/{order_id}/payments\n\
  \  method: post\n  operationId: addCheckoutPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /price_rules/rules/v2/shops/{shop_identifier}/rulesets\n  method: get\n  operationId: listRulesets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /price_rules/rules/v2/shops/{shop_identifier}/rulesets\n  method: post\n  operationId: createRuleset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /price_rules/rules/v2/shops/{shop_identifier}/rulesets/{ruleset_id}\n  method: get\n  operationId: getRuleset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /price_rules/rules/v2/shops/{shop_identifier}/rulesets/{ruleset_id}\n  method: put\n  operationId: updateRuleset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /price_rules/rules/v2/shops/{shop_identifier}/rulesets/{ruleset_id}\n  method: delete\n  operationId: deleteRuleset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /price_rules/rules/v2/shops/{shop_identifier}/process\n  method: post\n  operationId: processPrice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /products/v2/shops/{shop_identifier}/products\n  method: get\n  operationId: listProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/v2/shops/{shop_identifier}/products/{product_id}\n  method: get\n  operationId: getProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/v2/shops/{shop_identifier}/customers\n\
  \  method: get\n  operationId: listCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/v2/shops/{shop_identifier}/customers\n  method: post\n  operationId: createCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shops/v1/info\n  method: get\n  operationId: getShopInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bold-commerce/refs/heads/main/agentic-access/bold-commerce-agentic-access.yml
summary_line: 29 operations · 18 acting
tags:
- E-Commerce
- Subscriptions
- Checkout
- Pricing
- Headless Commerce
- Shopify
---
