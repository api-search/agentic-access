---
acting_count: 0
action_class_counts:
  connected: 6
api_specs:
- filename: also-cart-api-openapi.yml
  format: yaml
  label: Also Cart API
  slug: also-cart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/also/refs/heads/main/openapi/also-cart-api-openapi.yml
- filename: also-collections-api-openapi.yml
  format: yaml
  label: Also Collections API
  slug: also-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/also/refs/heads/main/openapi/also-collections-api-openapi.yml
- filename: also-products-api-openapi.yml
  format: yaml
  label: Also Products API
  slug: also-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/also/refs/heads/main/openapi/also-products-api-openapi.yml
- filename: also-search-api-openapi.yml
  format: yaml
  label: Also Search API
  slug: also-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/also/refs/heads/main/openapi/also-search-api-openapi.yml
consequence_counts:
  read: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Also Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Also exposes 6 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Also
provider_slug: also
slug: also-agentic-access
source_filename: also-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: generated\nsource: openapi/also-storefront-json-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 6\n  by_consequence:\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /products.json\n  method: get\n  operationId: listProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/{handle}.json\n  method: get\n  operationId: getProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections.json\n  method: get\n  operationId:\
  \ listCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{handle}/products.json\n  method: get\n  operationId: listCollectionProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cart.js\n  method: get\n  operationId: getCart\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search\n  method: get\n  operationId: searchStorefront\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/also/refs/heads/main/agentic-access/also-agentic-access.yml
summary_line: 6 operations
tags:
- Company
- Micromobility
- Electric Vehicles
- Transportation
- E-Commerce
- Consumer Hardware
- Agentic Commerce
- Logistics
- Delivery
---
