---
acting_count: 0
action_class_counts:
  connected: 9
api_specs:
- filename: ikea-product-catalog-openapi.yml
  format: yaml
  label: IKEA Product Catalog API (Unofficial)
  slug: product-catalog
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ikea/main/openapi/ikea-product-catalog-openapi.yml
- filename: ikea-search-openapi.yml
  format: yaml
  label: IKEA Search API (Unofficial)
  slug: search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ikea/main/openapi/ikea-search-openapi.yml
- filename: ikea-sales-item-openapi.yml
  format: yaml
  label: IKEA Sales Item API (Unofficial)
  slug: sales-item
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ikea/main/openapi/ikea-sales-item-openapi.yml
- filename: ikea-after-purchase-ordering-openapi.yml
  format: yaml
  label: IKEA After Purchase Ordering API (Unofficial)
  slug: after-purchase-ordering
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ikea/main/openapi/ikea-after-purchase-ordering-openapi.yml
consequence_counts:
  read: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ikea Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'IKEA exposes 9 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: IKEA
provider_slug: ikea
slug: ikea-agentic-access
source_filename: ikea-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/ikea-after-purchase-ordering-openapi.yml, openapi/ikea-product-catalog-openapi.yml,\n  openapi/ikea-sales-item-openapi.yml, openapi/ikea-search-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 9\n  by_consequence:\n    read: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /part/{partId}\n  method: get\n  operationId: getPartById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/{partialPartId}\n  method: get\n  operationId: searchParts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products\n  method: get\n  operationId: getProductParts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /meta-data/informera/stores-detailed.json\n  method: get\n  operationId: getStores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /meta-data/navigation/catalog-products-slim.json\n  method: get\n  operationId: getCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/{productIdSuffix}/{productId}.json\n  method: get\n  operationId: getProductById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /availabilities/{classUnitType}/{classUnitCode}\n  method: get\n  operationId: getProductAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /product-list-page\n  method: get\n  operationId: findProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /product-list-page/more-products\n  method: get\n  operationId: findProductsPaginated\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ikea/refs/heads/main/agentic-access/ikea-agentic-access.yml
summary_line: 9 operations
tags:
- Retail
- Home Furnishings
- Consumer Products
- Opensource
- Community
- Unofficial API
- Smart Home
---
