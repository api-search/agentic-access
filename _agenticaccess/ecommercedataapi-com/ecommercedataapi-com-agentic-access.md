---
acting_count: 46
action_class_counts:
  acting: 46
api_specs:
- filename: ecommercedataapi-com-amazon-keywords-api-openapi.yml
  format: yaml
  label: ecommercedataapi-com Amazon Keywords API
  slug: ecommercedataapi-com-amazon-keywords-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecommercedataapi-com/openapi/ecommercedataapi-com-amazon-keywords-api-openapi.yml
- filename: ecommercedataapi-com-amazon-markets-api-openapi.yml
  format: yaml
  label: ecommercedataapi-com Amazon Markets API
  slug: ecommercedataapi-com-amazon-markets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecommercedataapi-com/openapi/ecommercedataapi-com-amazon-markets-api-openapi.yml
- filename: ecommercedataapi-com-amazon-products-api-openapi.yml
  format: yaml
  label: ecommercedataapi-com Amazon Products API
  slug: ecommercedataapi-com-amazon-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecommercedataapi-com/openapi/ecommercedataapi-com-amazon-products-api-openapi.yml
- filename: ecommercedataapi-com-amazon-traffic-api-openapi.yml
  format: yaml
  label: ecommercedataapi-com Amazon Traffic API
  slug: ecommercedataapi-com-amazon-traffic-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecommercedataapi-com/openapi/ecommercedataapi-com-amazon-traffic-api-openapi.yml
- filename: ecommercedataapi-com-global-trademarks-api-openapi.yml
  format: yaml
  label: ecommercedataapi-com Global Trademarks API
  slug: ecommercedataapi-com-global-trademarks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecommercedataapi-com/openapi/ecommercedataapi-com-global-trademarks-api-openapi.yml
- filename: ecommercedataapi-com-tools-api-openapi.yml
  format: yaml
  label: ecommercedataapi-com Tools API
  slug: ecommercedataapi-com-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecommercedataapi-com/openapi/ecommercedataapi-com-tools-api-openapi.yml
consequence_counts:
  physical: 5
  write: 41
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ecommercedataapi Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/amazon/keyword-order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/global/brand/detail
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/global/brand/list
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/global/brand/range
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/global/brand/stats
operation_count: 46
overview: 'ecommercedataapi-com exposes 46 API operations that an AI agent could call, of which 46 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 41 write and 5 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ecommercedataapi-com
provider_slug: ecommercedataapi-com
slug: ecommercedataapi-com-agentic-access
source_filename: ecommercedataapi-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/ecommercedataapi-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 46\n  by_action_class:\n    acting: 46\n  by_consequence:\n    write: 41\n    physical: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/amazon/product/competitor-lookup\n  method: post\n  operationId: amazonProductsSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/amazon/product/research\n  method: post\n  operationId: amazonProductsResearch\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/amazon/asin/detail\n  method: post\n  operationId: amazonProductsDetails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/amazon/product/node\n  method: post\n  operationId: amazonProductsCategories\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/amazon/asin/history\n\
  \  method: post\n  operationId: amazonProductsHistory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/amazon/review\n  method: post\n  operationId: amazonProductsReviews\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/amazon/sales/prediction/bsr\n  method: post\n  operationId: amazonProductsBsrSalesEstimate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n    \
  \  triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/amazon/sales/prediction/asin\n  method: post\n  operationId: amazonProductsSalesEstimate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/amazon/asin/coupon-trend\n  method: post\n  operationId: amazonProductsCouponTrends\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/amazon/asin/with-coupon-trend\n  method: post\n  operationId: amazonProductsDetailsWithCouponTrends\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/amazon/asin/sales-trend\n  method: post\n  operationId: amazonProductsSalesTrends\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/amazon/asin/competitor\n  method: post\n  operationId: amazonProductsCompetitors\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/amazon/keyword/miner\n  method:\
  \ post\n  operationId: amazonKeywordsMiner\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/amazon/keyword-research\n  method: post\n  operationId: amazonKeywordsResearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/amazon/keyword-research/trends\n  method: post\n  operationId: amazonKeywordsResearchTrends\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n   \
  \   triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/amazon/google/trends\n  method: post\n  operationId: amazonKeywordsGoogleTrends\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/amazon/traffic/keyword/stat\n  method: post\n  operationId: amazonKeywordsTrafficStats\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/amazon/traffic/keyword\n  method: post\n  operationId: amazonKeywordsReverseLookup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/amazon/aba/research/weekly\n  method: post\n  operationId: amazonKeywordsAbaWeekly\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/amazon/aba/research/monthly\n  method: post\n  operationId: amazonKeywordsAbaMonthly\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/amazon/keyword/conversion\n  method: post\n \
  \ operationId: amazonKeywordsConversion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/amazon/keyword-order\n  method: post\n  operationId: amazonKeywordsOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/amazon/traffic/extend\n  method: post\n  operationId: amazonKeywordsExpand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/amazon/aba/research/trends\n  method: post\n  operationId: amazonKeywordsAbaTrends\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/amazon/traffic/listing/stat\n  method: post\n  operationId: amazonTrafficRelatedProductsStats\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/amazon/traffic/listing/page\n  method: post\n  operationId: amazonTrafficRelatedProducts\n  x-agentic-access:\n    action-class: acting\n  \
  \  consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/amazon/traffic/source\n  method: post\n  operationId: amazonTrafficSources\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/amazon/market/research\n  method: post\n  operationId: amazonMarketsResearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/amazon/market/statistics\n\
  \  method: post\n  operationId: amazonMarketsStatistics\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/amazon/market/goods\n  method: post\n  operationId: amazonMarketsProductConcentration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/amazon/market/brand\n  method: post\n  operationId: amazonMarketsBrandConcentration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/amazon/market/seller\n  method: post\n  operationId: amazonMarketsSellerConcentration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/amazon/market/seller/type\n  method: post\n  operationId: amazonMarketsSellerTypeDistribution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/amazon/market/seller/location\n  method: post\n  operationId: amazonMarketsSellerCountryDistribution\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/amazon/market/performance\n  method: post\n  operationId: amazonMarketsDemandTrends\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/amazon/market/shelf/time\n  method: post\n  operationId: amazonMarketsListingAgeDistribution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/amazon/market/shelf/trend\n\
  \  method: post\n  operationId: amazonMarketsListingTrends\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/amazon/market/ratings\n  method: post\n  operationId: amazonMarketsRatingsCountDistribution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/amazon/market/rating\n  method: post\n  operationId: amazonMarketsRatingDistribution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/amazon/market/price\n  method: post\n  operationId: amazonMarketsPriceDistribution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/amazon/market/ebc\n  method: post\n  operationId: amazonMarketsContentDistribution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/global/brand/stats\n  method: post\n  operationId: globalTrademarksStatistics\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/global/brand/list\n  method: post\n  operationId: globalTrademarksSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/global/brand/detail\n  method: post\n  operationId: globalTrademarksDetails\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/global/brand/range\n  method: post\n  operationId: globalTrademarksCoverage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/image-text\n  method: post\n  operationId: toolsImageText\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/ecommercedataapi-com/agentic-access/ecommercedataapi-com-agentic-access.yml
summary_line: 46 operations · 46 acting
tags:
- Company
- E-Commerce
- Data
- Amazon
- Market Research
---
