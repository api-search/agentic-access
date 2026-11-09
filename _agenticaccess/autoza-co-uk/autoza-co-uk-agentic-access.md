---
acting_count: 0
action_class_counts:
  connected: 9
api_specs:
- filename: autoza-co-uk-dealers-api-openapi.yml
  format: yaml
  label: Autoza UK Dealers API
  slug: autoza-co-uk-dealers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autoza-co-uk/openapi/autoza-co-uk-dealers-api-openapi.yml
- filename: autoza-co-uk-listing-api-openapi.yml
  format: yaml
  label: Autoza UK Listing API
  slug: autoza-co-uk-listing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autoza-co-uk/openapi/autoza-co-uk-listing-api-openapi.yml
- filename: autoza-co-uk-makes-api-openapi.yml
  format: yaml
  label: Autoza UK Makes API
  slug: autoza-co-uk-makes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autoza-co-uk/openapi/autoza-co-uk-makes-api-openapi.yml
- filename: autoza-co-uk-market-api-openapi.yml
  format: yaml
  label: Autoza UK Market API
  slug: autoza-co-uk-market-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autoza-co-uk/openapi/autoza-co-uk-market-api-openapi.yml
- filename: autoza-co-uk-search-api-openapi.yml
  format: yaml
  label: Autoza UK Search API
  slug: autoza-co-uk-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autoza-co-uk/openapi/autoza-co-uk-search-api-openapi.yml
- filename: autoza-co-uk-stats-api-openapi.yml
  format: yaml
  label: Autoza UK Stats API
  slug: autoza-co-uk-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autoza-co-uk/openapi/autoza-co-uk-stats-api-openapi.yml
- filename: autoza-co-uk-vehicles-api-openapi.yml
  format: yaml
  label: Autoza UK Vehicles API
  slug: autoza-co-uk-vehicles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autoza-co-uk/openapi/autoza-co-uk-vehicles-api-openapi.yml
consequence_counts:
  read: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Autoza Co Uk Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'Autoza UK exposes 9 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Autoza UK
provider_slug: autoza-co-uk
slug: autoza-co-uk-agentic-access
source_filename: autoza-co-uk-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/autoza-co-uk-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 9\n  by_consequence:\n    read: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/vehicles\n  method: get\n  operationId: searchVehicles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/vehicles/{id}\n  method: get\n  operationId: getVehicle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/dealers\n  method: get\n  operationId: searchDealers\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/dealers/{id}\n  method: get\n  operationId: getDealer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/search\n  method: get\n  operationId: searchListings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/listing/{id}\n  method: get\n  operationId: getListing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/makes\n  method: get\n  operationId: listMakes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/v1/stats\n  method: get\n  operationId: getStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/market/uk\n  method: get\n  operationId: getMarketSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/autoza-co-uk/agentic-access/autoza-co-uk-agentic-access.yml
summary_line: 9 operations
tags:
- Automotive
- Marketplace
- Artificial Intelligence
- Used Vehicles
- United Kingdom
---
