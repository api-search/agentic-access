---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 23
api_specs:
- filename: compsniper-com-account-api-openapi.yml
  format: yaml
  label: compsniper-com Account API
  slug: compsniper-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsniper-com/openapi/compsniper-com-account-api-openapi.yml
- filename: compsniper-com-best-offer-prices-api-openapi.yml
  format: yaml
  label: compsniper-com Best Offer Prices API
  slug: compsniper-com-best-offer-prices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsniper-com/openapi/compsniper-com-best-offer-prices-api-openapi.yml
- filename: compsniper-com-bulk-search-api-openapi.yml
  format: yaml
  label: compsniper-com Bulk Search API
  slug: compsniper-com-bulk-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsniper-com/openapi/compsniper-com-bulk-search-api-openapi.yml
- filename: compsniper-com-cards-api-openapi.yml
  format: yaml
  label: compsniper-com Cards API
  slug: compsniper-com-cards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsniper-com/openapi/compsniper-com-cards-api-openapi.yml
- filename: compsniper-com-depop-api-openapi.yml
  format: yaml
  label: compsniper-com Depop API
  slug: compsniper-com-depop-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsniper-com/openapi/compsniper-com-depop-api-openapi.yml
- filename: compsniper-com-grailed-api-openapi.yml
  format: yaml
  label: compsniper-com Grailed API
  slug: compsniper-com-grailed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsniper-com/openapi/compsniper-com-grailed-api-openapi.yml
- filename: compsniper-com-mercari-api-openapi.yml
  format: yaml
  label: compsniper-com Mercari API
  slug: compsniper-com-mercari-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsniper-com/openapi/compsniper-com-mercari-api-openapi.yml
- filename: compsniper-com-poshmark-api-openapi.yml
  format: yaml
  label: compsniper-com Poshmark API
  slug: compsniper-com-poshmark-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsniper-com/openapi/compsniper-com-poshmark-api-openapi.yml
- filename: compsniper-com-psa-api-openapi.yml
  format: yaml
  label: compsniper-com PSA API
  slug: compsniper-com-psa-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsniper-com/openapi/compsniper-com-psa-api-openapi.yml
- filename: compsniper-com-scrape-api-openapi.yml
  format: yaml
  label: compsniper-com Scrape API
  slug: compsniper-com-scrape-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsniper-com/openapi/compsniper-com-scrape-api-openapi.yml
- filename: compsniper-com-shipping-rates-api-openapi.yml
  format: yaml
  label: compsniper-com Shipping Rates API
  slug: compsniper-com-shipping-rates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsniper-com/openapi/compsniper-com-shipping-rates-api-openapi.yml
- filename: compsniper-com-sold-history-api-openapi.yml
  format: yaml
  label: compsniper-com Sold history API
  slug: compsniper-com-sold-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsniper-com/openapi/compsniper-com-sold-history-api-openapi.yml
- filename: compsniper-com-summary-api-openapi.yml
  format: yaml
  label: compsniper-com Summary API
  slug: compsniper-com-summary-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsniper-com/openapi/compsniper-com-summary-api-openapi.yml
- filename: compsniper-com-tcgplayer-api-openapi.yml
  format: yaml
  label: compsniper-com TC Gplayer API
  slug: compsniper-com-tcgplayer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsniper-com/openapi/compsniper-com-tcgplayer-api-openapi.yml
consequence_counts:
  read: 23
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Compsniper Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 28
overview: 'compsniper-com exposes 28 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 23 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: compsniper-com
provider_slug: compsniper-com
slug: compsniper-com-agentic-access
source_filename: compsniper-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/compsniper-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 28\n  by_action_class:\n    connected: 23\n    acting: 5\n  by_consequence:\n    read: 23\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/research/sold\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tcgplayer/sold\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tcgplayer/listings\n  method: get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/grailed/sold\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/grailed/listings\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/depop/listings\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/psa/search\n  method: get\n  operationId: searchPsaCards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/psa/card\n  method: get\n  operationId: getPsaCard\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/psa/sets\n  method: get\n  operationId: listPsaSets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/psa/set\n  method: get\n  operationId: getPsaSetPopulation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/scrape\n  method: get\n  operationId: searchSoldListings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/scrape/category\n  method: get\n  operationId: browseSoldListingsByCategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/summary\n  method: get\n  operationId:\
  \ getPriceSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/best-offer-prices\n  method: get\n  operationId: getBestOfferPrices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account/usage\n  method: get\n  operationId: getAccountUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/bulk-search\n  method: post\n  operationId: bulkSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/bulk-search/{runId}/download.csv\n\
  \  method: get\n  operationId: downloadBulkSearchCsv\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cards/batch\n  method: post\n  operationId: submitCardBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/cards/batch/{jobId}\n  method: get\n  operationId: getCardBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cards/batch/{jobId}\n  method: delete\n  operationId: cancelCardBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/scrape/max\n  method: post\n  operationId: startMaxSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/scrape/max/results/{jobId}\n  method: get\n  operationId: getMaxSearchResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/scrape/max/{jobId}\n  method: delete\n  operationId: cancelMaxSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/scrape/max/{jobId}/download.csv\n  method: get\n  operationId: downloadMaxSearchCsv\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/poshmark/sold\n  method: get\n  operationId: searchPoshmarkSold\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/mercari\n  method: get\n  operationId: searchMercariListings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/shipping/rates\n  method: post\n  operationId: getShippingRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/shipping/usage\n\
  \  method: get\n  operationId: getShippingRateUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/compsniper-com/agentic-access/compsniper-com-agentic-access.yml
summary_line: 28 operations · 5 acting
tags:
- Company
- Marketplace
- E-Commerce
- Data
- Collectibles
---
