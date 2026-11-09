---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 20
api_specs:
- filename: shelfatlas-com-chains-api-openapi.yml
  format: yaml
  label: shelfatlas-com Chains API
  slug: shelfatlas-com-chains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shelfatlas-com/openapi/shelfatlas-com-chains-api-openapi.yml
- filename: shelfatlas-com-mcp-api-openapi.yml
  format: yaml
  label: shelfatlas-com MCP API
  slug: shelfatlas-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shelfatlas-com/openapi/shelfatlas-com-mcp-api-openapi.yml
- filename: shelfatlas-com-observations-api-openapi.yml
  format: yaml
  label: shelfatlas-com Observations API
  slug: shelfatlas-com-observations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shelfatlas-com/openapi/shelfatlas-com-observations-api-openapi.yml
- filename: shelfatlas-com-observedprices-api-openapi.yml
  format: yaml
  label: shelfatlas-com Observed Prices API
  slug: shelfatlas-com-observedprices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shelfatlas-com/openapi/shelfatlas-com-observedprices-api-openapi.yml
- filename: shelfatlas-com-offers-api-openapi.yml
  format: yaml
  label: shelfatlas-com Offers API
  slug: shelfatlas-com-offers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shelfatlas-com/openapi/shelfatlas-com-offers-api-openapi.yml
- filename: shelfatlas-com-price-history-api-openapi.yml
  format: yaml
  label: shelfatlas-com Price history API
  slug: shelfatlas-com-price-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shelfatlas-com/openapi/shelfatlas-com-price-history-api-openapi.yml
- filename: shelfatlas-com-products-api-openapi.yml
  format: yaml
  label: shelfatlas-com Products API
  slug: shelfatlas-com-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shelfatlas-com/openapi/shelfatlas-com-products-api-openapi.yml
- filename: shelfatlas-com-seoterms-api-openapi.yml
  format: yaml
  label: shelfatlas-com Seo Terms API
  slug: shelfatlas-com-seoterms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shelfatlas-com/openapi/shelfatlas-com-seoterms-api-openapi.yml
- filename: shelfatlas-com-stats-api-openapi.yml
  format: yaml
  label: shelfatlas-com Stats API
  slug: shelfatlas-com-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shelfatlas-com/openapi/shelfatlas-com-stats-api-openapi.yml
- filename: shelfatlas-com-stores-api-openapi.yml
  format: yaml
  label: shelfatlas-com Stores API
  slug: shelfatlas-com-stores-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shelfatlas-com/openapi/shelfatlas-com-stores-api-openapi.yml
consequence_counts:
  read: 20
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Shelfatlas Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 24
overview: 'shelfatlas-com exposes 24 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: shelfatlas-com
provider_slug: shelfatlas-com
slug: shelfatlas-com-agentic-access
source_filename: shelfatlas-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/shelfatlas-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 24\n  by_action_class:\n    connected: 20\n    acting: 4\n  by_consequence:\n    read: 20\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/public/catalog/products\n  method: get\n  operationId: listProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/public/catalog/products/{id}\n  method: get\n  operationId: getProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/v1/public/catalog/products/{id}/offers\n  method: get\n  operationId: listProductOffers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/public/catalog/offers\n  method: get\n  operationId: listOffers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/public/catalog/offers/{id}\n  method: get\n  operationId: getOffer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/public/catalog/offers/search\n  method: get\n  operationId: searchOffers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/public/catalog/offers/sample\n  method: get\n\
  \  operationId: sampleOffers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/public/catalog/offers/history\n  method: get\n  operationId: getOfferHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/public/catalog/offers/price-drops\n  method: get\n  operationId: listPriceDrops\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/public/catalog/offers/term-history\n  method: get\n  operationId: getOfferTermHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/public/catalog/price-history\n  method: get\n  operationId: getPriceHistory\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/public/catalog/stores\n  method: get\n  operationId: listStores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/public/catalog/stores/{id}\n  method: get\n  operationId: getStore\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/public/catalog/stores/{id}/stock\n  method: get\n  operationId: getStoreStock\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/public/catalog/stores/{id}/local-prices\n  method: get\n  operationId: getStoreLocalPrices\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/public/catalog/local-prices\n  method: get\n  operationId: listNearbyLocalPrices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/public/catalog/shelf-label/read\n  method: post\n  operationId: readShelfLabel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/public/catalog/chains\n  method: get\n  operationId: listChains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/public/catalog/stats\n  method: get\n  operationId:\
  \ getStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/public/catalog/observed-prices\n  method: get\n  operationId: listObservedPrices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/public/catalog/seo-terms\n  method: get\n  operationId: listSeoTerms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/observations\n  method: post\n  operationId: createObservation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/steering-events\n\
  \  method: post\n  operationId: recordSteeringEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/mcp\n  method: post\n  operationId: mcpJsonRpc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/shelfatlas-com/agentic-access/shelfatlas-com-agentic-access.yml
summary_line: 24 operations · 4 acting
tags:
- Company
- Grocery
- Denmark
- Retail
---
