---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 58
api_specs:
- filename: ecomscout-com-analytics-api-openapi.yml
  format: yaml
  label: EcomScout Analytics API
  slug: ecomscout-com-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecomscout-com/openapi/ecomscout-com-analytics-api-openapi.yml
- filename: ecomscout-com-apps-api-openapi.yml
  format: yaml
  label: EcomScout Apps API
  slug: ecomscout-com-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecomscout-com/openapi/ecomscout-com-apps-api-openapi.yml
- filename: ecomscout-com-audiences-api-openapi.yml
  format: yaml
  label: EcomScout Audiences API
  slug: ecomscout-com-audiences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecomscout-com/openapi/ecomscout-com-audiences-api-openapi.yml
- filename: ecomscout-com-changes-api-openapi.yml
  format: yaml
  label: EcomScout Changes API
  slug: ecomscout-com-changes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecomscout-com/openapi/ecomscout-com-changes-api-openapi.yml
- filename: ecomscout-com-discovery-api-openapi.yml
  format: yaml
  label: EcomScout Discovery API
  slug: ecomscout-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecomscout-com/openapi/ecomscout-com-discovery-api-openapi.yml
- filename: ecomscout-com-products-api-openapi.yml
  format: yaml
  label: EcomScout Products API
  slug: ecomscout-com-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecomscout-com/openapi/ecomscout-com-products-api-openapi.yml
- filename: ecomscout-com-scrapes-api-openapi.yml
  format: yaml
  label: EcomScout Scrapes API
  slug: ecomscout-com-scrapes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecomscout-com/openapi/ecomscout-com-scrapes-api-openapi.yml
- filename: ecomscout-com-signals-api-openapi.yml
  format: yaml
  label: EcomScout Signals API
  slug: ecomscout-com-signals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecomscout-com/openapi/ecomscout-com-signals-api-openapi.yml
- filename: ecomscout-com-stores-api-openapi.yml
  format: yaml
  label: EcomScout Stores API
  slug: ecomscout-com-stores-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecomscout-com/openapi/ecomscout-com-stores-api-openapi.yml
consequence_counts:
  physical: 1
  read: 58
  safety-critical: 1
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Ecomscout Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/signals/{id}/stop
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/audiences/enrich
operation_count: 72
overview: 'EcomScout exposes 72 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 58 read, 12 write, 1 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: EcomScout
provider_slug: ecomscout-com
slug: ecomscout-com-agentic-access
source_filename: ecomscout-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: generated\nsource: openapi/ecomscout-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 72\n  by_action_class:\n    connected: 58\n    acting: 14\n  by_consequence:\n    read: 58\n    write: 12\n    physical: 1\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /v1/health\n  method: get\n  operationId: health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/examples\n  method: get\n  operationId: examples\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stores\n\
  \  method: get\n  operationId: listStores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stores/compare\n  method: get\n  operationId: compareStores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stores/{domain}\n  method: get\n  operationId: getStore\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stores/{domain}/history\n  method: get\n  operationId: getStoreHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stores/{domain}/traffic\n  method: get\n  operationId: getStoreTraffic\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stores/{domain}/apps\n  method: get\n  operationId: getStoreApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stores/{domain}/competitors\n  method: get\n  operationId: listStoreCompetitors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stores/{domain}/inventory-probe\n  method: get\n  operationId: getStoreInventoryProbe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stores/{domain}/products\n  method: get\n  operationId: listStoreProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/stores/{domain}/changes\n  method: get\n  operationId: listStoreChangesForDomain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stores/{domain}/contacts\n  method: get\n  operationId: getStoreContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stores/{domain}/verify-contacts\n  method: get\n  operationId: getVerifyContactsStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stores/{domain}/verify-contacts\n  method: post\n  operationId: requestVerifyContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/contacts\n\
  \  method: get\n  operationId: getContactsByQuery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/products/search\n  method: get\n  operationId: searchProductResearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/products/search/suggest\n  method: get\n  operationId: suggestProductResearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/products/search/trending\n  method: get\n  operationId: trendingProductResearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/products/research/{id}\n  method: get\n  operationId: getProductResearch\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/products/research/{id}/sellers\n  method: get\n  operationId: listProductResearchSellers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/products\n  method: get\n  operationId: listProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/products/{domain}/{handle}\n  method: get\n  operationId: getProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/products/changes\n  method: get\n  operationId: listProductChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/changes\n  method: get\n  operationId: unifiedChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps\n  method: get\n  operationId: listApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{slug}\n  method: get\n  operationId: getApp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{slug}/stores\n  method: get\n  operationId: listAppStores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/analytics/overview\n  method: get\n  operationId: marketOverview\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/analytics/verticals\n  method: get\n  operationId: verticalStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/analytics/countries\n  method: get\n  operationId: countryStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/analytics/movers\n  method: get\n  operationId: storeMovers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/analytics/trends\n  method: get\n  operationId: trafficTrends\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/analytics/trends/stores\n  method: get\n  operationId: trafficTrendStores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/analytics/trends/coverage\n  method: get\n  operationId: trafficTrendCoverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/audiences/options\n  method: get\n  operationId: audienceOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/audiences/preview\n  method: get\n  operationId: audiencePreview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/audiences/preview\n  method: post\n  operationId: audiencePreviewPost\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/audiences/export\n  method: get\n  operationId: audienceExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/audiences/export\n  method: post\n  operationId: audienceExportPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/audiences/enrich\n  method: post\n  operationId: audienceEnrich\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/audiences/lookalike\n  method: post\n  operationId: audienceLookalike\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/audiences\n  method: post\n  operationId: createAudience\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/audiences\n  method: get\n  operationId:\
  \ listAudiences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/audiences/{id}\n  method: get\n  operationId: getAudience\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/audiences/{id}\n  method: patch\n  operationId: updateAudience\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/audiences/{id}\n  method: delete\n  operationId: deleteAudience\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/audiences/{id}/changes\n  method: get\n  operationId: audienceChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/audiences/{id}/export\n  method: get\n  operationId: audienceSavedExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/signals\n  method: get\n  operationId: listSignals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/signals\n  method: post\n  operationId: createSignal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/signals/insights\n  method: get\n  operationId: listSignalInsights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/signals/{id}\n  method: get\n  operationId: getSignal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/signals/{id}\n  method: patch\n  operationId: patchSignal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/signals/{id}\n  method: delete\n  operationId: deleteSignal\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/signals/{id}/stop\n  method: post\n  operationId: stopSignal\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/signals/{id}/probe\n  method: get\n  operationId: signalProbeStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/signals/{id}/probe\n  method: post\n  operationId: probeSignal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/signals/{id}/stats\n  method: get\n  operationId: signalStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/signals/{id}/sales\n  method: get\n  operationId: signalSales\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/signals/{id}/daily\n  method: get\n  operationId: signalDaily\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/signals/{id}/inventory\n  method: get\n  operationId: signalInventory\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/signals/{id}/ads/overview\n  method: get\n  operationId: signalAdsOverview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/signals/{id}/ads\n  method: get\n  operationId: signalAds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/signals/{id}/apps\n  method: get\n  operationId: signalApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/signals/{id}/insights\n  method: get\n  operationId: signalInsights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/scrapes\n\
  \  method: post\n  operationId: createScrape\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/scrapes/bulk\n  method: post\n  operationId: createScrapeBulk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/scrapes/{id}\n  method: get\n  operationId: getScrape\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/llms.txt\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n \
  \   subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/docs.md\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/openapi.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/ecomscout-com/agentic-access/ecomscout-com-agentic-access.yml
summary_line: 72 operations · 14 acting · 1 human-in-the-loop
tags:
- Company
- Shopify
- Analytics
- E-Commerce
- Data
---
