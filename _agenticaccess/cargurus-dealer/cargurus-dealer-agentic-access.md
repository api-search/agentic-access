---
acting_count: 0
action_class_counts:
  connected: 6
api_specs:
- filename: cargurus-dealer-car-selector-api-openapi.yml
  format: yaml
  label: CarGurus Car Selector API
  slug: cargurus-dealer-car-selector-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargurus-dealer/refs/heads/main/openapi/cargurus-dealer-car-selector-api-openapi.yml
- filename: cargurus-dealer-dealer-reviews-api-openapi.yml
  format: yaml
  label: CarGurus Dealer Reviews API
  slug: cargurus-dealer-dealer-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargurus-dealer/refs/heads/main/openapi/cargurus-dealer-dealer-reviews-api-openapi.yml
- filename: cargurus-dealer-dealer-stats-api-openapi.yml
  format: yaml
  label: CarGurus Dealer Stats API
  slug: cargurus-dealer-dealer-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargurus-dealer/refs/heads/main/openapi/cargurus-dealer-dealer-stats-api-openapi.yml
- filename: cargurus-dealer-instant-market-value-api-openapi.yml
  format: yaml
  label: CarGurus Instant Market Value API
  slug: cargurus-dealer-instant-market-value-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargurus-dealer/refs/heads/main/openapi/cargurus-dealer-instant-market-value-api-openapi.yml
consequence_counts:
  read: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cargurus Dealer Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'CarGurus exposes 6 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CarGurus
provider_slug: cargurus-dealer
slug: cargurus-dealer-agentic-access
source_filename: cargurus-dealer-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/cargurus-dealer-car-selector-api-openapi.yml, openapi/cargurus-dealer-dealer-reviews-api-openapi.yml,\n  openapi/cargurus-dealer-dealer-stats-api-openapi.yml, openapi/cargurus-dealer-instant-market-value-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 6\n  by_consequence:\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /carselector/listMakes.action\n  method: get\n  operationId: listMakes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /carselector/listModels.action\n  method: get\n  operationId: listModels\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /carselector/listingSearch.action\n  method: get\n  operationId: listingSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dealerReviewsRequest.action\n  method: post\n  operationId: dealerReviewsRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dealerStatsRequest.action\n  method: post\n  operationId: dealerStatsRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /imvRequest.action\n  method: post\n  operationId: imvRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cargurus-dealer/refs/heads/main/agentic-access/cargurus-dealer-agentic-access.yml
summary_line: 6 operations
tags:
- Automotive
- Marketplace
- Car Listings
- Dealers
- Vehicle Pricing
- Reviews
- Inventory
---
