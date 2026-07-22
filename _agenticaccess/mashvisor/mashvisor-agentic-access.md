---
acting_count: 0
action_class_counts:
  connected: 28
api_specs:
- filename: mashvisor-openapi.yml
  format: yaml
  label: Mashvisor Data API
  slug: mashvisor-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mashvisor/refs/heads/main/openapi/mashvisor-openapi.yml
consequence_counts:
  read: 28
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Mashvisor Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 28
overview: 'Mashvisor exposes 28 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 28 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Mashvisor
provider_slug: mashvisor
slug: mashvisor-agentic-access
source_filename: mashvisor-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/mashvisor-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 28\n  by_action_class:\n    connected: 28\n  by_consequence:\n    read: 28\n  human_in_the_loop_required: 0\noperations:\n- path: /client/city/list\n  method: get\n  operationId: listCities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/metadata/validate-city\n  method: get\n  operationId: validateCity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/city/neighborhoods/{state}/{city}\n  method:\
  \ get\n  operationId: listCityNeighborhoods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/city/top-markets\n  method: get\n  operationId: listTopMarkets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/city/investment/{state}/{city}\n  method: get\n  operationId: getCityInvestment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/city/properties/{state}/{city}\n  method: get\n  operationId: listCityProperties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/city/listings\n  method: get\n  operationId: listCityListings\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/trends/neighborhoods\n  method: get\n  operationId: listNeighborhoodTrends\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/neighborhood/{id}/bar\n  method: get\n  operationId: getNeighborhoodBar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/neighborhood/{id}/schools\n  method: get\n  operationId: getNeighborhoodSchools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/property\n  method: get\n  operationId: getProperty\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/property/{id}/images\n  method: get\n  operationId: getPropertyImages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/property/{id}/taxing\n  method: get\n  operationId: getPropertyTaxing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/property/{id}/transactions\n  method: get\n  operationId: getPropertyTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/property/estimates/{pid}\n  method: get\n  operationId: getPropertyEstimates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /client/property/{id}/estimates-history\n  method: get\n  operationId: getPropertyEstimatesHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/property/nearby\n  method: get\n  operationId: listNearbyProperties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/property/{id}/schools\n  method: get\n  operationId: getPropertySchools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/property/{id}/investment\n  method: get\n  operationId: getPropertyInvestment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/property/{id}/investment/breakdown\n\
  \  method: get\n  operationId: getPropertyInvestmentBreakdown\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/property/marker\n  method: get\n  operationId: getPropertyMarker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/neighborhood/{id}/airbnb/details\n  method: get\n  operationId: listNeighborhoodAirbnbDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/neighborhood/{id}/traditional/listing\n  method: get\n  operationId: listNeighborhoodTraditionalListings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/rental-rates\n  method:\
  \ get\n  operationId: getRentalRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/trends/cities\n  method: get\n  operationId: listCityTrends\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/trends/summary/{state}/{city}\n  method: get\n  operationId: getTrendsSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/trends/listing-price\n  method: get\n  operationId: getListingPriceTrends\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/search/heatmap\n  method: get\n  operationId: getSearchHeatmap\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mashvisor/refs/heads/main/agentic-access/mashvisor-agentic-access.yml
summary_line: 28 operations
tags:
- Company
- Real Estate
- Property Data
- Analytics
- Rental
- Airbnb
- Investment
- MLS
- Housing
---
