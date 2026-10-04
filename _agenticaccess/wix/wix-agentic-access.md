---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 8
api_specs:
- filename: wix-asyncapi.yml
  format: yaml
  label: Wix Webhooks
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/wix/refs/heads/main/asyncapi/wix-asyncapi.yml
- filename: wix-cart-api-openapi.yml
  format: yaml
  label: Wix Cart API
  slug: wix-cart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wix/refs/heads/main/openapi/wix-cart-api-openapi.yml
- filename: wix-checkout-api-openapi.yml
  format: yaml
  label: Wix Checkout API
  slug: wix-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wix/refs/heads/main/openapi/wix-checkout-api-openapi.yml
- filename: wix-orders-api-openapi.yml
  format: yaml
  label: Wix Orders API
  slug: wix-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wix/refs/heads/main/openapi/wix-orders-api-openapi.yml
- filename: wix-products-api-openapi.yml
  format: yaml
  label: Wix Products API
  slug: wix-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wix/refs/heads/main/openapi/wix-products-api-openapi.yml
- filename: wix-oauth-api-openapi.yml
  format: yaml
  label: Wix O Auth API
  slug: wix-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wix/refs/heads/main/openapi/wix-oauth-api-openapi.yml
consequence_counts:
  physical: 4
  read: 8
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Wix Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ecom/v1/checkouts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ecom/v1/checkouts/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ecom/v1/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ecom/v1/orders/{id}
operation_count: 19
overview: 'Wix exposes 19 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 7 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Wix
provider_slug: wix
slug: wix-agentic-access
source_filename: wix-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/wix-cart-api-openapi.yml, openapi/wix-checkout-api-openapi.yml, openapi/wix-oauth-api-openapi.yml,\n  openapi/wix-orders-api-openapi.yml, openapi/wix-products-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    acting: 11\n    connected: 8\n  by_consequence:\n    write: 7\n    read: 8\n    physical: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /ecom/v1/carts\n  method: post\n  operationId: createCart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /ecom/v1/carts/{id}\n  method: get\n  operationId: getCart\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ecom/v1/carts/{id}\n  method: delete\n  operationId: deleteCart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ecom/v1/carts/{id}/update\n  method: post\n  operationId: updateCart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ecom/v1/checkouts\n  method:\
  \ post\n  operationId: createCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ecom/v1/checkouts/{id}\n  method: get\n  operationId: getCheckout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ecom/v1/checkouts/{id}\n  method: post\n  operationId: updateCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /oauth2/token\n  method: post\n  operationId: requestAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth2/token/refresh\n  method: post\n  operationId: refreshAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth2/token/info\n  method: get\n  operationId: getTokenInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ecom/v1/orders\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ecom/v1/orders/{id}\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ecom/v1/orders/{id}\n  method: post\n  operationId: updateOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ecom/v1/orders/search\n  method: post\n  operationId: searchOrders\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stores/v3/products\n  method: post\n  operationId: createProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stores/v3/products/query\n  method: post\n  operationId: queryProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stores/v3/products/search\n  method: post\n  operationId: searchProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stores/v3/products/{id}\n  method: get\n\
  \  operationId: getProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stores/v3/products/{id}\n  method: patch\n  operationId: updateProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wix/refs/heads/main/agentic-access/wix-agentic-access.yml
summary_line: 19 operations · 11 acting
tags:
- CMS
- E-Commerce
- Headless
- Website Builder
---
