---
acting_count: 0
action_class_counts:
  connected: 19
api_specs:
- filename: barcodes-gg-account-api-openapi.yml
  format: yaml
  label: Barcodes.GG Account API
  slug: barcodes-gg-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/barcodes-gg/openapi/barcodes-gg-account-api-openapi.yml
- filename: barcodes-gg-barcodes-api-openapi.yml
  format: yaml
  label: Barcodes.GG Barcodes API
  slug: barcodes-gg-barcodes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/barcodes-gg/openapi/barcodes-gg-barcodes-api-openapi.yml
- filename: barcodes-gg-images-api-openapi.yml
  format: yaml
  label: Barcodes.GG Images API
  slug: barcodes-gg-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/barcodes-gg/openapi/barcodes-gg-images-api-openapi.yml
- filename: barcodes-gg-legacy-v1-api-openapi.yml
  format: yaml
  label: Barcodes.GG Legacy v1 API
  slug: barcodes-gg-legacy-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/barcodes-gg/openapi/barcodes-gg-legacy-v1-api-openapi.yml
- filename: barcodes-gg-products-api-openapi.yml
  format: yaml
  label: Barcodes.GG Products API
  slug: barcodes-gg-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/barcodes-gg/openapi/barcodes-gg-products-api-openapi.yml
consequence_counts:
  read: 19
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Barcodes Gg Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 19
overview: 'Barcodes.GG exposes 19 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Barcodes.GG
provider_slug: barcodes-gg
slug: barcodes-gg-agentic-access
source_filename: barcodes-gg-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: generated\nsource: openapi/barcodes-gg-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    connected: 19\n  by_consequence:\n    read: 19\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/barcode/lookup/{barcode}\n  method: get\n  operationId: lookupBarcode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/barcode/lookup/sku/{style_code}\n  method: get\n  operationId: lookupBarcodesBySku\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/product/search\n\
  \  method: get\n  operationId: searchProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/product/search/bulk\n  method: post\n  operationId: searchProductsBulk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/product/lookup/sku/{style_code}\n  method: get\n  operationId: lookupProductBySku\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/product/lookup/uid/{product_unique_id}\n  method: get\n  operationId: lookupProductByUid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/product/details/{style_code}\n  method: get\n  operationId: getProductDetails\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/product/upcoming\n  method: get\n  operationId: listUpcomingProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/product/latest\n  method: get\n  operationId: listLatestProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/product/alternatives/{style_code}\n  method: get\n  operationId: getProductAlternatives\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/token/usage\n  method: get\n  operationId: getTokenUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /image/uid/{product_unique_id}\n  method: get\n  operationId: getImageByUid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /image/{style_code}\n  method: get\n  operationId: getImageByStyleCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /barcode/lookup/{barcode}\n  method: get\n  operationId: lookupBarcodeV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /barcode/lookup/sku/{style_code}\n  method: get\n  operationId: lookupBarcodesBySkuV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /product/search\n\
  \  method: get\n  operationId: searchProductsV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /product/lookup/sku/{style_code}\n  method: get\n  operationId: lookupProductBySkuV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /product/latest\n  method: get\n  operationId: listLatestProductsV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /product/details/{style_code}\n  method: get\n  operationId: getProductDetailsV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/barcodes-gg/agentic-access/barcodes-gg-agentic-access.yml
summary_line: 19 operations
tags:
- Company
- Barcodes
- Sneaker
- Streetwear
---
