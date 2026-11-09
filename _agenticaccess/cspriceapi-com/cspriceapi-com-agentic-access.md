---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 13
api_specs:
- filename: cspriceapi-com-buyorder-prices-api-openapi.yml
  format: yaml
  label: cspriceapi-com Buyorder Prices API
  slug: cspriceapi-com-buyorder-prices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cspriceapi-com/openapi/cspriceapi-com-buyorder-prices-api-openapi.yml
- filename: cspriceapi-com-float-ranged-api-openapi.yml
  format: yaml
  label: cspriceapi-com Float Ranged API
  slug: cspriceapi-com-float-ranged-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cspriceapi-com/openapi/cspriceapi-com-float-ranged-api-openapi.yml
- filename: cspriceapi-com-indexes-api-openapi.yml
  format: yaml
  label: cspriceapi-com Indexes API
  slug: cspriceapi-com-indexes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cspriceapi-com/openapi/cspriceapi-com-indexes-api-openapi.yml
- filename: cspriceapi-com-listing-prices-api-openapi.yml
  format: yaml
  label: cspriceapi-com Listing Prices API
  slug: cspriceapi-com-listing-prices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cspriceapi-com/openapi/cspriceapi-com-listing-prices-api-openapi.yml
- filename: cspriceapi-com-price-history-api-openapi.yml
  format: yaml
  label: cspriceapi-com Price History API
  slug: cspriceapi-com-price-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cspriceapi-com/openapi/cspriceapi-com-price-history-api-openapi.yml
- filename: cspriceapi-com-sales-data-api-openapi.yml
  format: yaml
  label: cspriceapi-com Sales Data API
  slug: cspriceapi-com-sales-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cspriceapi-com/openapi/cspriceapi-com-sales-data-api-openapi.yml
- filename: cspriceapi-com-steam-api-openapi.yml
  format: yaml
  label: cspriceapi-com Steam API
  slug: cspriceapi-com-steam-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cspriceapi-com/openapi/cspriceapi-com-steam-api-openapi.yml
consequence_counts:
  read: 13
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cspriceapi Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'cspriceapi-com exposes 14 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: cspriceapi-com
provider_slug: cspriceapi-com
slug: cspriceapi-com-agentic-access
source_filename: cspriceapi-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/api.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 13\n    acting: 1\n  by_consequence:\n    read: 13\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/steam\n  method: get\n  operationId: getSteamMarket\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/prices/latest\n  method: get\n  operationId: getLatestPrices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/prices/latest\n  method: post\n  operationId:\
  \ postLatestPrices\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/prices/youpin/buyorder\n  method: get\n  operationId: getYoupinBuyorders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/prices/youpin/float-buyorder\n  method: get\n  operationId: getYoupinFloatBuyorders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/prices/buff163/buyorder\n  method: get\n  operationId: getBuffBuyorders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/prices/buff163/float-buyorder\n  method: get\n  operationId: getBuffFloatBuyorders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/prices/{market}/history\n  method: get\n  operationId: getMarketPriceHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/prices/float-ranged\n  method: get\n  operationId: getFloatRangedPricesV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/prices/buff163/float-ranged\n  method: get\n  operationId: getBuffFloatRangedPrices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/prices/search\n  method: get\n  operationId:\
  \ searchSkin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/indexes/market-cap\n  method: get\n  operationId: getYoupinMarketCap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/market-sales/search\n  method: get\n  operationId: searchMarketSales\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/market-sales/export\n  method: get\n  operationId: exportMarketSalesZip\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/cspriceapi-com/agentic-access/cspriceapi-com-agentic-access.yml
summary_line: 14 operations · 1 acting
tags:
- Company
- Gaming
- Price Data
- Marketplace
---
