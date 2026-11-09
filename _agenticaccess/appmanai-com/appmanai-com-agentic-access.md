---
acting_count: 0
action_class_counts:
  connected: 7
api_specs:
- filename: appmanai-com-app-metadata-api-openapi.yml
  format: yaml
  label: AppManAi App Metadata API
  slug: appmanai-com-app-metadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmanai-com/openapi/appmanai-com-app-metadata-api-openapi.yml
- filename: appmanai-com-app-metrics-api-openapi.yml
  format: yaml
  label: AppManAi App Metrics API
  slug: appmanai-com-app-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmanai-com/openapi/appmanai-com-app-metrics-api-openapi.yml
- filename: appmanai-com-app-reviews-api-openapi.yml
  format: yaml
  label: AppManAi App Reviews API
  slug: appmanai-com-app-reviews-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmanai-com/openapi/appmanai-com-app-reviews-api-openapi.yml
- filename: appmanai-com-app-search-api-openapi.yml
  format: yaml
  label: AppManAi App Search API
  slug: appmanai-com-app-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmanai-com/openapi/appmanai-com-app-search-api-openapi.yml
consequence_counts:
  read: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Appmanai Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'AppManAi exposes 7 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AppManAi
provider_slug: appmanai-com
slug: appmanai-com-agentic-access
source_filename: appmanai-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/appmanai-com-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 7\n  by_consequence:\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /apps/metrics/metadata\n  method: get\n  operationId: appMetricsMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps/metrics/metadata/batch\n  method: get\n  operationId: appMetricsMetadataBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps/search\n  method:\
  \ get\n  operationId: appSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps/similar\n  method: get\n  operationId: appSimilar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps/metrics/ratings/worldwide\n  method: get\n  operationId: appMetricsRatingsWorldwide\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps/metrics/ratings/history\n  method: get\n  operationId: appMetricsRatingsHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps/reviews\n  method: get\n  operationId: appReviews\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/appmanai-com/agentic-access/appmanai-com-agentic-access.yml
summary_line: 7 operations
tags:
- App Store Data
- Google Play Data
- ASO
- Data API
- App Intelligence
---
