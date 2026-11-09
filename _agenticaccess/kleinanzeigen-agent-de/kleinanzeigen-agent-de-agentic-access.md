---
acting_count: 0
action_class_counts:
  connected: 14
api_specs:
- filename: kleinanzeigen-agent-de-ads-api-openapi.yml
  format: yaml
  label: kleinanzeigen-agent-de Ads API
  slug: kleinanzeigen-agent-de-ads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kleinanzeigen-agent-de/openapi/kleinanzeigen-agent-de-ads-api-openapi.yml
- filename: kleinanzeigen-agent-de-categories-api-openapi.yml
  format: yaml
  label: kleinanzeigen-agent-de Categories API
  slug: kleinanzeigen-agent-de-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kleinanzeigen-agent-de/openapi/kleinanzeigen-agent-de-categories-api-openapi.yml
- filename: kleinanzeigen-agent-de-history-api-openapi.yml
  format: yaml
  label: kleinanzeigen-agent-de History API
  slug: kleinanzeigen-agent-de-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kleinanzeigen-agent-de/openapi/kleinanzeigen-agent-de-history-api-openapi.yml
- filename: kleinanzeigen-agent-de-locations-api-openapi.yml
  format: yaml
  label: kleinanzeigen-agent-de Locations API
  slug: kleinanzeigen-agent-de-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kleinanzeigen-agent-de/openapi/kleinanzeigen-agent-de-locations-api-openapi.yml
- filename: kleinanzeigen-agent-de-search-api-openapi.yml
  format: yaml
  label: kleinanzeigen-agent-de Search API
  slug: kleinanzeigen-agent-de-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kleinanzeigen-agent-de/openapi/kleinanzeigen-agent-de-search-api-openapi.yml
- filename: kleinanzeigen-agent-de-sellers-api-openapi.yml
  format: yaml
  label: kleinanzeigen-agent-de Sellers API
  slug: kleinanzeigen-agent-de-sellers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kleinanzeigen-agent-de/openapi/kleinanzeigen-agent-de-sellers-api-openapi.yml
consequence_counts:
  read: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Kleinanzeigen Agent De Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'kleinanzeigen-agent-de exposes 14 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: kleinanzeigen-agent-de
provider_slug: kleinanzeigen-agent-de
slug: kleinanzeigen-agent-de-agentic-access
source_filename: kleinanzeigen-agent-de-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/kleinanzeigen-agent-de-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 14\n  by_consequence:\n    read: 14\n  human_in_the_loop_required: 0\noperations:\n- path: /search\n  method: get\n  operationId: searchKleinanzeigen\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/category-counts\n  method: get\n  operationId: getKleinanzeigenSearchCategoryCounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /history\n  method:\
  \ get\n  operationId: searchKleinanzeigenHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ads/{ad_id}\n  method: get\n  operationId: getKleinanzeigenAd\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ads/{ad_id}/status\n  method: get\n  operationId: getKleinanzeigenAdStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ads/{ad_id}/similar\n  method: get\n  operationId: getKleinanzeigenSimilarAds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ads/{ad_id}/seller-ads\n  method: get\n  operationId: getKleinanzeigenAdSellerAds\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sellers/{seller_id}/profile\n  method: get\n  operationId: getKleinanzeigenSellerProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sellers/{seller_id}/ads\n  method: get\n  operationId: getKleinanzeigenSellerAds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /categories\n  method: get\n  operationId: listKleinanzeigenCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /categories/{category_id}/metadata\n  method: get\n  operationId: getKleinanzeigenCategoryMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n \
  \   subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /categories/{category_id}/search-metadata\n  method: get\n  operationId: getKleinanzeigenCategorySearchMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locations\n  method: get\n  operationId: searchKleinanzeigenLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locations/{location_id}\n  method: get\n  operationId: getKleinanzeigenLocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/kleinanzeigen-agent-de/agentic-access/kleinanzeigen-agent-de-agentic-access.yml
summary_line: 14 operations
tags:
- Search
- Monitoring
- Market Analysis
- Germany
- Kleinanzeigen
---
