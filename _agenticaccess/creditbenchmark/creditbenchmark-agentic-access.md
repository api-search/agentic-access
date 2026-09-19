---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 5
api_specs:
- filename: creditbenchmark-analytics-api-openapi.yml
  format: yaml
  label: Credit Benchmark Analytics API
  slug: creditbenchmark-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creditbenchmark/refs/heads/main/openapi/creditbenchmark-analytics-api-openapi.yml
- filename: creditbenchmark-authentication-api-openapi.yml
  format: yaml
  label: Credit Benchmark Authentication API
  slug: creditbenchmark-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creditbenchmark/refs/heads/main/openapi/creditbenchmark-authentication-api-openapi.yml
- filename: creditbenchmark-contributor-data-api-openapi.yml
  format: yaml
  label: Credit Benchmark Contributor Data API
  slug: creditbenchmark-contributor-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creditbenchmark/refs/heads/main/openapi/creditbenchmark-contributor-data-api-openapi.yml
- filename: creditbenchmark-entity-data-api-openapi.yml
  format: yaml
  label: Credit Benchmark Entity Data API
  slug: creditbenchmark-entity-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creditbenchmark/refs/heads/main/openapi/creditbenchmark-entity-data-api-openapi.yml
- filename: creditbenchmark-entity-matching-api-openapi.yml
  format: yaml
  label: Credit Benchmark Entity Matching API
  slug: creditbenchmark-entity-matching-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creditbenchmark/refs/heads/main/openapi/creditbenchmark-entity-matching-api-openapi.yml
- filename: creditbenchmark-portfolio-analytics-api-openapi.yml
  format: yaml
  label: Credit Benchmark Portfolio Analytics API
  slug: creditbenchmark-portfolio-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creditbenchmark/refs/heads/main/openapi/creditbenchmark-portfolio-analytics-api-openapi.yml
- filename: creditbenchmark-data-api-openapi.yml
  format: yaml
  label: Credit Benchmark Data API
  slug: creditbenchmark-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creditbenchmark/refs/heads/main/openapi/creditbenchmark-data-api-openapi.yml
- filename: creditbenchmark-entity-resolution-api-openapi.yml
  format: yaml
  label: Credit Benchmark Entity Resolution API
  slug: creditbenchmark-entity-resolution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creditbenchmark/refs/heads/main/openapi/creditbenchmark-entity-resolution-api-openapi.yml
- filename: creditbenchmark-metadata-api-openapi.yml
  format: yaml
  label: Credit Benchmark Metadata API
  slug: creditbenchmark-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creditbenchmark/refs/heads/main/openapi/creditbenchmark-metadata-api-openapi.yml
consequence_counts:
  read: 5
  write: 18
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Creditbenchmark Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 23
overview: 'Credit Benchmark exposes 23 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 18 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Credit Benchmark
provider_slug: creditbenchmark
slug: creditbenchmark-agentic-access
source_filename: creditbenchmark-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: generated\nsource: openapi/creditbenchmark-analytics-api-openapi.yml, openapi/creditbenchmark-authentication-api-openapi.yml,\n  openapi/creditbenchmark-contributor-data-api-openapi.yml, openapi/creditbenchmark-data-api-openapi.yml,\n  openapi/creditbenchmark-entity-data-api-openapi.yml, openapi/creditbenchmark-entity-matching-api-openapi.yml,\n  openapi/creditbenchmark-entity-resolution-api-openapi.yml, openapi/creditbenchmark-metadata-api-openapi.yml,\n  openapi/creditbenchmark-portfolio-analytics-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    acting: 18\n    connected: 5\n  by_consequence:\n    write: 18\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n\
  - path: /analytics/v2/data/aggregatetrend\n  method: post\n  operationId: aggregateTrend\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analytics/v2/data/entityratingchange\n  method: post\n  operationId: entityRatingChange\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analytics/v2/data/creditbreakdown\n  method: post\n  operationId: creditBreakdown\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n  \
  \    human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analytics/v2/data/ratingdistribution\n  method: post\n  operationId: ratingDistribution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/analytics/custom-aggregate\n  method: post\n  operationId: customAggregate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/analytics/rating-distribution\n  method: post\n  operationId: ratingDistribution\n  x-agentic-access:\n    action-class: acting\n   \
  \ consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/security/token\n  method: post\n  operationId: getToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gartan/api/token\n  method: post\n  operationId: getToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/analytics/contributor/custom-aggregate\n  method: post\n  operationId:\
  \ clientDataCustomAggregate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/analytics/contributor/rating-distribution\n  method: post\n  operationId: clientDataRatingDistribution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/analytics/contributor/portfolio-summary\n  method: post\n  operationId: clientDataPortfolioSummary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/analytics/contributor/entity-rating-change\n  method: post\n  operationId: clientDataEntityRatingChange\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analytics/v2/data/getdata\n  method: post\n  operationId: getData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/analytics/entity-rating-change\n  method: post\n  operationId: entityRatingChange\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /matching/match\n  method: post\n  operationId: matchEntities\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /matching/text/match_external\n  method: post\n  operationId: matchExternalEntities\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analytics/v2/metadata/columns\n  method: get\n  operationId: metadata_columns_v2_metadata_columns_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/v2/metadata/rating-scales\n  method: get\n  operationId: metadata_rating_scales_v2_metadata_rating_scales_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/v2/metadata/industry-schema\n  method: get\n  operationId: metadata_industry_schema_v2_metadata_industry_schema_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/v2/metadata/geography-schema\n  method: get\n  operationId: metadata_geography_schema_v2_metadata_geography_schema_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/v2/metadata/available-dates\n\
  \  method: get\n  operationId: metadata_available_dates_v2_metadata_available_dates_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/analytics/portfolio-data\n  method: post\n  operationId: portfolioData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/analytics/portfolio-summary\n  method: post\n  operationId: portfolioSummary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/creditbenchmark/refs/heads/main/agentic-access/creditbenchmark-agentic-access.yml
summary_line: 23 operations · 18 acting
tags:
- Company
- Credit Risk
- Financial Data
- Credit Ratings
- Analytics
- Risk Management
- Entity Resolution
- Consensus Data
---
