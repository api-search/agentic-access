---
acting_count: 0
action_class_counts:
  connected: 6
api_specs:
- filename: dynamical-org-analyses-api-openapi.yml
  format: yaml
  label: Dynamical Analyses API
  slug: dynamical-org-analyses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dynamical-org/openapi/dynamical-org-analyses-api-openapi.yml
- filename: dynamical-org-data-api-openapi.yml
  format: yaml
  label: Dynamical Data API
  slug: dynamical-org-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dynamical-org/openapi/dynamical-org-data-api-openapi.yml
- filename: dynamical-org-data-products-api-openapi.yml
  format: yaml
  label: Dynamical Data Products API
  slug: dynamical-org-data-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dynamical-org/openapi/dynamical-org-data-products-api-openapi.yml
- filename: dynamical-org-forecasts-api-openapi.yml
  format: yaml
  label: Dynamical Forecasts API
  slug: dynamical-org-forecasts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dynamical-org/openapi/dynamical-org-forecasts-api-openapi.yml
consequence_counts:
  read: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Dynamical Org Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Dynamical exposes 6 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Dynamical
provider_slug: dynamical-org
slug: dynamical-org-agentic-access
source_filename: dynamical-org-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: generated\nsource: openapi/dynamical-org-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 6\n  by_consequence:\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/data-products\n  method: get\n  operationId: list_data_products_v1_data_products_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data-products/{dataProductId}\n  method: get\n  operationId: describe_data_product_v1_data_products__dataProductId__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/forecasts/runs\n  method: get\n  operationId: list_forecast_runs_v1_forecasts_runs_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/forecasts\n  method: post\n  operationId: query_forecasts_v1_forecasts_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/analyses\n  method: post\n  operationId: query_analyses_v1_analyses_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data/{dataProductId}/{snapshotId}/points/{gridIndices}\n  method: get\n  operationId: query_canonical_point_v1_data__dataProductId___snapshotId__points__gridIndices__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/dynamical-org/agentic-access/dynamical-org-agentic-access.yml
summary_line: 6 operations
tags:
- Weather
- Climate
- Open Data
- Research
- Not-for-profit
---
