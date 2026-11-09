---
acting_count: 0
action_class_counts:
  connected: 13
api_specs:
- filename: apibara-tech-filters-api-openapi.yml
  format: yaml
  label: Apibara.tech Filters API
  slug: apibara-tech-filters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apibara-tech/openapi/apibara-tech-filters-api-openapi.yml
- filename: apibara-tech-image-proxy-api-openapi.yml
  format: yaml
  label: Apibara.tech Image Proxy API
  slug: apibara-tech-image-proxy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apibara-tech/openapi/apibara-tech-image-proxy-api-openapi.yml
- filename: apibara-tech-locations-api-openapi.yml
  format: yaml
  label: Apibara.tech Locations API
  slug: apibara-tech-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apibara-tech/openapi/apibara-tech-locations-api-openapi.yml
- filename: apibara-tech-related-vehicles-api-openapi.yml
  format: yaml
  label: Apibara.tech Related Vehicles API
  slug: apibara-tech-related-vehicles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apibara-tech/openapi/apibara-tech-related-vehicles-api-openapi.yml
- filename: apibara-tech-shipping-api-openapi.yml
  format: yaml
  label: Apibara.tech Shipping API
  slug: apibara-tech-shipping-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apibara-tech/openapi/apibara-tech-shipping-api-openapi.yml
- filename: apibara-tech-url-tools-api-openapi.yml
  format: yaml
  label: Apibara.tech URL Tools API
  slug: apibara-tech-url-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apibara-tech/openapi/apibara-tech-url-tools-api-openapi.yml
- filename: apibara-tech-usage-api-openapi.yml
  format: yaml
  label: Apibara.tech Usage API
  slug: apibara-tech-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apibara-tech/openapi/apibara-tech-usage-api-openapi.yml
- filename: apibara-tech-vehicle-history-api-openapi.yml
  format: yaml
  label: Apibara.tech Vehicle History API
  slug: apibara-tech-vehicle-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apibara-tech/openapi/apibara-tech-vehicle-history-api-openapi.yml
- filename: apibara-tech-vehicles-api-openapi.yml
  format: yaml
  label: Apibara.tech Vehicles API
  slug: apibara-tech-vehicles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apibara-tech/openapi/apibara-tech-vehicles-api-openapi.yml
- filename: apibara-tech-change-stream-api-openapi.yml
  format: yaml
  label: Apibara.tech Change Stream API
  slug: apibara-tech-change-stream-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apibara-tech/openapi/apibara-tech-change-stream-api-openapi.yml
- filename: apibara-tech-market-api-openapi.yml
  format: yaml
  label: Apibara.tech Market API
  slug: apibara-tech-market-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apibara-tech/openapi/apibara-tech-market-api-openapi.yml
consequence_counts:
  read: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Apibara Tech Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'Apibara.tech exposes 13 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Apibara.tech
provider_slug: apibara-tech
slug: apibara-tech-agentic-access
source_filename: apibara-tech-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/apibara-tech-change-stream-api-openapi.yml, openapi/apibara-tech-filters-api-openapi.yml,\n  openapi/apibara-tech-image-proxy-api-openapi.yml, openapi/apibara-tech-locations-api-openapi.yml,\n  openapi/apibara-tech-market-api-openapi.yml, openapi/apibara-tech-related-vehicles-api-openapi.yml,\n  openapi/apibara-tech-shipping-api-openapi.yml, openapi/apibara-tech-url-tools-api-openapi.yml,\n  openapi/apibara-tech-usage-api-openapi.yml, openapi/apibara-tech-vehicle-history-api-openapi.yml,\n  openapi/apibara-tech-vehicles-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 13\n  by_consequence:\n    read: 13\n  human_in_the_loop_required:\
  \ 0\noperations:\n- path: /changes\n  method: get\n  operationId: listVehicleChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vehicles/filters\n  method: get\n  operationId: getVehicleFilters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /image-proxy\n  method: get\n  operationId: proxyAuctionImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locations\n  method: get\n  operationId: listAuctionLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /market/sold-prices\n  method: get\n  operationId: marketSoldPriceStats\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vehicles/{slugVin}/related\n  method: get\n  operationId: getRelatedVehicles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vehicles/{slugVin}/shipping\n  method: get\n  operationId: getVehicleShipping\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shipping/auction-to-port\n  method: get\n  operationId: getAuctionToPortShipping\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vehicles/urltodetails\n  method: get\n  operationId: getVehicleDetailsFromUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /usage\n  method: get\n  operationId: getApiUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vehicles/{slugVin}/history\n  method: get\n  operationId: getVehicleHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vehicles\n  method: get\n  operationId: listAuctionVehicles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vehicles/{slugVin}\n  method: get\n  operationId: getVehicleDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/apibara-tech/agentic-access/apibara-tech-agentic-access.yml
summary_line: 13 operations
tags:
- Automotive
- vehicle-auction-data
- Copart
- IAAI
- vin-history
- Marketplace
- REST API
- Vehicle Auctions
- Salvage Auctions
- VIN Data
- Used-Car Marketplace Data
- Data Infrastructure
- Data as a Service
- REST
- JSON:API
- MCP
- Agent-Native
---
