---
acting_count: 0
action_class_counts:
  connected: 20
api_specs:
- filename: birkinbagstock-com-alternatives-api-openapi.yml
  format: yaml
  label: birkinbagstock-com Alternatives API
  slug: birkinbagstock-com-alternatives-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/birkinbagstock-com/openapi/birkinbagstock-com-alternatives-api-openapi.yml
- filename: birkinbagstock-com-auction-results-api-openapi.yml
  format: yaml
  label: birkinbagstock-com Auction Results API
  slug: birkinbagstock-com-auction-results-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/birkinbagstock-com/openapi/birkinbagstock-com-auction-results-api-openapi.yml
- filename: birkinbagstock-com-auctions-api-openapi.yml
  format: yaml
  label: birkinbagstock-com Auctions API
  slug: birkinbagstock-com-auctions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/birkinbagstock-com/openapi/birkinbagstock-com-auctions-api-openapi.yml
- filename: birkinbagstock-com-buy-api-openapi.yml
  format: yaml
  label: birkinbagstock-com Buy API
  slug: birkinbagstock-com-buy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/birkinbagstock-com/openapi/birkinbagstock-com-buy-api-openapi.yml
- filename: birkinbagstock-com-data-api-openapi.yml
  format: yaml
  label: birkinbagstock-com Data API
  slug: birkinbagstock-com-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/birkinbagstock-com/openapi/birkinbagstock-com-data-api-openapi.yml
- filename: birkinbagstock-com-freshness-api-openapi.yml
  format: yaml
  label: birkinbagstock-com Freshness API
  slug: birkinbagstock-com-freshness-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/birkinbagstock-com/openapi/birkinbagstock-com-freshness-api-openapi.yml
- filename: birkinbagstock-com-inventory-api-openapi.yml
  format: yaml
  label: birkinbagstock-com Inventory API
  slug: birkinbagstock-com-inventory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/birkinbagstock-com/openapi/birkinbagstock-com-inventory-api-openapi.yml
- filename: birkinbagstock-com-listing-api-openapi.yml
  format: yaml
  label: birkinbagstock-com Listing API
  slug: birkinbagstock-com-listing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/birkinbagstock-com/openapi/birkinbagstock-com-listing-api-openapi.yml
- filename: birkinbagstock-com-merchants-api-openapi.yml
  format: yaml
  label: birkinbagstock-com Merchants API
  slug: birkinbagstock-com-merchants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/birkinbagstock-com/openapi/birkinbagstock-com-merchants-api-openapi.yml
- filename: birkinbagstock-com-news-api-openapi.yml
  format: yaml
  label: birkinbagstock-com News API
  slug: birkinbagstock-com-news-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/birkinbagstock-com/openapi/birkinbagstock-com-news-api-openapi.yml
- filename: birkinbagstock-com-recommend-api-openapi.yml
  format: yaml
  label: birkinbagstock-com Recommend API
  slug: birkinbagstock-com-recommend-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/birkinbagstock-com/openapi/birkinbagstock-com-recommend-api-openapi.yml
- filename: birkinbagstock-com-services-api-openapi.yml
  format: yaml
  label: birkinbagstock-com Services API
  slug: birkinbagstock-com-services-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/birkinbagstock-com/openapi/birkinbagstock-com-services-api-openapi.yml
- filename: birkinbagstock-com-well-known-api-openapi.yml
  format: yaml
  label: birkinbagstock-com .well Known API
  slug: birkinbagstock-com-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/birkinbagstock-com/openapi/birkinbagstock-com-well-known-api-openapi.yml
consequence_counts:
  read: 20
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Birkinbagstock Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 20
overview: 'birkinbagstock-com exposes 20 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: birkinbagstock-com
provider_slug: birkinbagstock-com
slug: birkinbagstock-com-agentic-access
source_filename: birkinbagstock-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/birkinbagstock-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    connected: 20\n  by_consequence:\n    read: 20\n  human_in_the_loop_required: 0\noperations:\n- path: /.well-known/source-index.json\n  method: get\n  operationId: getBirkinWellKnownSourceIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/alternatives/search\n  method: get\n  operationId: searchBirkinAlternatives\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/v1/alternatives/{slug}\n  method: get\n  operationId: getBirkinAlternativeProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/auction-results\n  method: get\n  operationId: getHermesAuctionResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/auctions\n  method: get\n  operationId: listHermesAuctions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/buy/{id}\n  method: get\n  operationId: getBuyUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/freshness\n  method: get\n  operationId: getInventoryFreshness\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/inventory\n  method: get\n  operationId: searchBirkinBags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/listing/{id}\n  method: get\n  operationId: getBirkinListing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/listing/{id}/alternatives\n  method: get\n  operationId: getBirkinListingAlternatives\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/merchants\n  method: get\n  operationId: listBirkinResellers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/v1/news\n  method: get\n  operationId: getBirkinNews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/recommend\n  method: get\n  operationId: recommendBirkin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/services\n  method: get\n  operationId: findHermesCareServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/api-directory.json\n  method: get\n  operationId: getBirkinApiDirectory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/birkin-alternatives.json\n  method: get\n  operationId:\
  \ getBirkinAlternativesIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/birkin-price-appreciation-index.json\n  method: get\n  operationId: getBirkinMatchedPriceIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/dataset-card.md\n  method: get\n  operationId: getBirkinDatasetCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/dataset-metadata.json\n  method: get\n  operationId: getBirkinDatasetMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/listing-price-history/{listing_id}.json\n  method: get\n  operationId: getListingPriceHistory\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/birkinbagstock-com/agentic-access/birkinbagstock-com-agentic-access.yml
summary_line: 20 operations
tags:
- Luxury Resale
- Marketplace
- Authentication
- Price Index
- Bag Marketplace
- Collector Tools
---
