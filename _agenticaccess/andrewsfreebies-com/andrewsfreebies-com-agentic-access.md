---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 14
api_specs:
- filename: andrewsfreebies-com-categories-api-openapi.yml
  format: yaml
  label: Andrew’s Freebies Categories API
  slug: andrewsfreebies-com-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/andrewsfreebies-com/openapi/andrewsfreebies-com-categories-api-openapi.yml
- filename: andrewsfreebies-com-coverage-api-openapi.yml
  format: yaml
  label: Andrew’s Freebies Coverage API
  slug: andrewsfreebies-com-coverage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/andrewsfreebies-com/openapi/andrewsfreebies-com-coverage-api-openapi.yml
- filename: andrewsfreebies-com-entitlements-api-openapi.yml
  format: yaml
  label: Andrew’s Freebies Entitlements API
  slug: andrewsfreebies-com-entitlements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/andrewsfreebies-com/openapi/andrewsfreebies-com-entitlements-api-openapi.yml
- filename: andrewsfreebies-com-flags-api-openapi.yml
  format: yaml
  label: Andrew’s Freebies Flags API
  slug: andrewsfreebies-com-flags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/andrewsfreebies-com/openapi/andrewsfreebies-com-flags-api-openapi.yml
- filename: andrewsfreebies-com-freshness-api-openapi.yml
  format: yaml
  label: Andrew’s Freebies Freshness API
  slug: andrewsfreebies-com-freshness-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/andrewsfreebies-com/openapi/andrewsfreebies-com-freshness-api-openapi.yml
- filename: andrewsfreebies-com-outcomes-api-openapi.yml
  format: yaml
  label: Andrew’s Freebies Outcomes API
  slug: andrewsfreebies-com-outcomes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/andrewsfreebies-com/openapi/andrewsfreebies-com-outcomes-api-openapi.yml
- filename: andrewsfreebies-com-search-api-openapi.yml
  format: yaml
  label: Andrew’s Freebies Search API
  slug: andrewsfreebies-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/andrewsfreebies-com/openapi/andrewsfreebies-com-search-api-openapi.yml
- filename: andrewsfreebies-com-sources-api-openapi.yml
  format: yaml
  label: Andrew’s Freebies Sources API
  slug: andrewsfreebies-com-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/andrewsfreebies-com/openapi/andrewsfreebies-com-sources-api-openapi.yml
- filename: andrewsfreebies-com-stats-api-openapi.yml
  format: yaml
  label: Andrew’s Freebies Stats API
  slug: andrewsfreebies-com-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/andrewsfreebies-com/openapi/andrewsfreebies-com-stats-api-openapi.yml
- filename: andrewsfreebies-com-taxonomy-api-openapi.yml
  format: yaml
  label: Andrew’s Freebies Taxonomy API
  slug: andrewsfreebies-com-taxonomy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/andrewsfreebies-com/openapi/andrewsfreebies-com-taxonomy-api-openapi.yml
- filename: andrewsfreebies-com-trials-api-openapi.yml
  format: yaml
  label: Andrew’s Freebies Trials API
  slug: andrewsfreebies-com-trials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/andrewsfreebies-com/openapi/andrewsfreebies-com-trials-api-openapi.yml
- filename: andrewsfreebies-com-verification-api-openapi.yml
  format: yaml
  label: Andrew’s Freebies Verification API
  slug: andrewsfreebies-com-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/andrewsfreebies-com/openapi/andrewsfreebies-com-verification-api-openapi.yml
consequence_counts:
  read: 14
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Andrewsfreebies Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'Andrew’s Freebies exposes 17 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Andrew’s Freebies
provider_slug: andrewsfreebies-com
slug: andrewsfreebies-com-agentic-access
source_filename: andrewsfreebies-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/andrewsfreebies-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    connected: 14\n    acting: 3\n  by_consequence:\n    read: 14\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/trials\n  method: get\n  operationId: searchTrials\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/trials/{slug}\n  method: get\n  operationId: getTrial\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/search\n  method:\
  \ get\n  operationId: searchFreebies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/entitlements\n  method: get\n  operationId: searchEntitlements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/entitlements/{slug}\n  method: get\n  operationId: getEntitlement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/categories\n  method: get\n  operationId: listCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/taxonomy\n  method: get\n  operationId: getEntitlementTaxonomy\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sources\n  method: get\n  operationId: listSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/coverage\n  method: get\n  operationId: getPublicServiceCoverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/stats\n  method: get\n  operationId: getAggregateStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/outcomes\n  method: get\n  operationId: getOutcomeSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/outcomes\n  method: post\n\
  \  operationId: reportOfferOutcome\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/verification\n  method: get\n  operationId: getVerificationHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/verification\n  method: post\n  operationId: ingestVerificationRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/freshness\n  method: get\n  operationId: getFreshness\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/flags\n  method: get\n  operationId: listDealFlags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/flags\n  method: post\n  operationId: flagDeal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/andrewsfreebies-com/agentic-access/andrewsfreebies-com-agentic-access.yml
summary_line: 17 operations · 3 acting
tags:
- Freebies
- Savings
- Cashback
- Bonuses
- Trials
- Deals
---
