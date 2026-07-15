---
acting_count: 0
action_class_counts:
  connected: 8
api_specs:
- filename: best-buy-products-api.yaml
  format: yaml
  label: Best Buy Products API
  slug: products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/best-buy/refs/heads/main/openapi/best-buy-products-api.yaml
- filename: best-buy-stores-api.yaml
  format: yaml
  label: Best Buy Stores API
  slug: stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/best-buy/refs/heads/main/openapi/best-buy-stores-api.yaml
- filename: best-buy-recommendations-api.yaml
  format: yaml
  label: Best Buy Recommendations API
  slug: recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/best-buy/refs/heads/main/openapi/best-buy-recommendations-api.yaml
consequence_counts:
  read: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Best Buy Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Best Buy exposes 8 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Best Buy
provider_slug: best-buy
slug: best-buy-agentic-access
source_filename: best-buy-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/best-buy-products-api.yaml, openapi/best-buy-recommendations-api.yaml, openapi/best-buy-stores-api.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 8\n  by_consequence:\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /products\n  method: get\n  operationId: listProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/{sku}\n  method: get\n  operationId: getProductBySku\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /products/trendingViewed\n  method: get\n  operationId: getTrendingProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/mostViewed\n  method: get\n  operationId: getMostViewedProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/{sku}/alsoViewed\n  method: get\n  operationId: getAlsoViewedProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/{sku}/alsoBought\n  method: get\n  operationId: getAlsoBoughtProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stores\n  method: get\n  operationId: listStores\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stores/{storeId}\n  method: get\n  operationId: getStoreById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/best-buy/refs/heads/main/agentic-access/best-buy-agentic-access.yml
summary_line: 8 operations
tags:
- Fortune 100
- Retail
- Consumer Electronics
- E-Commerce
- Products
- Stores
---
