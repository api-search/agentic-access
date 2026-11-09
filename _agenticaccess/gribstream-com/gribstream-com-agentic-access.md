---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 10
api_specs:
- filename: gribstream-com-account-api-openapi.yml
  format: yaml
  label: gribstream-com Account API
  slug: gribstream-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gribstream-com/openapi/gribstream-com-account-api-openapi.yml
- filename: gribstream-com-catalog-api-openapi.yml
  format: yaml
  label: gribstream-com Catalog API
  slug: gribstream-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gribstream-com/openapi/gribstream-com-catalog-api-openapi.yml
- filename: gribstream-com-grid-coordinates-api-openapi.yml
  format: yaml
  label: gribstream-com Grid coordinates API
  slug: gribstream-com-grid-coordinates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gribstream-com/openapi/gribstream-com-grid-coordinates-api-openapi.yml
- filename: gribstream-com-weather-data-api-openapi.yml
  format: yaml
  label: gribstream-com Weather data API
  slug: gribstream-com-weather-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gribstream-com/openapi/gribstream-com-weather-data-api-openapi.yml
consequence_counts:
  read: 10
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Gribstream Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'gribstream-com exposes 13 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: gribstream-com
provider_slug: gribstream-com
slug: gribstream-com-agentic-access
source_filename: gribstream-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/gribstream-com-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 10\n    acting: 3\n  by_consequence:\n    read: 10\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v2/quota\n  method: get\n  operationId: getQuota\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/{dataset}/native-coordinates\n  method: get\n  operationId: getDatasetNativeCoordinates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/v2/{dataset}/runs\n  method: post\n  operationId: postDatasetRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/{dataset}/forecasts\n  method: post\n  operationId: postDatasetForecastsAlias\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/{dataset}/timeseries\n  method: post\n  operationId: postDatasetTimeseries\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/{dataset}/history\n  method:\
  \ post\n  operationId: postDatasetHistoryAlias\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/catalog/datasets\n  method: get\n  operationId: getCatalogDatasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/catalog/datasets/{dataset}\n  method: get\n  operationId: getCatalogDataset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/catalog/datasets/{dataset}/selectors\n  method: get\n  operationId: getCatalogDatasetSelectors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/catalog/datasets/{dataset}/parameters\n  method: get\n  operationId: getCatalogDatasetParameters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/catalog/datasets/{dataset}/parameters/{parameter}\n  method: get\n  operationId: getCatalogDatasetParameter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/catalog/shared-parameters\n  method: get\n  operationId: getCatalogSharedParameters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/catalog/shared-parameters/{parameter}\n  method: get\n  operationId: getCatalogSharedParameter\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/gribstream-com/agentic-access/gribstream-com-agentic-access.yml
summary_line: 13 operations · 3 acting
tags:
- Company
- Weather
- Forecast
- Data
---
