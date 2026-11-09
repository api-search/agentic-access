---
acting_count: 0
action_class_counts:
  connected: 28
api_specs:
- filename: met-office-capabilities-api-openapi.yml
  format: yaml
  label: Met Office Capabilities API
  slug: met-office-capabilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/met-office/openapi/met-office-capabilities-api-openapi.yml
- filename: met-office-collection-metadata-api-openapi.yml
  format: yaml
  label: Met Office Collection Metadata API
  slug: met-office-collection-metadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/met-office/openapi/met-office-collection-metadata-api-openapi.yml
- filename: met-office-instance-data-api-openapi.yml
  format: yaml
  label: Met Office Instance Data API
  slug: met-office-instance-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/met-office/openapi/met-office-instance-data-api-openapi.yml
- filename: met-office-instance-metadata-api-openapi.yml
  format: yaml
  label: Met Office Instance Metadata API
  slug: met-office-instance-metadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/met-office/openapi/met-office-instance-metadata-api-openapi.yml
- filename: met-office-met-office-land-observations-public-api-api-openapi.yml
  format: yaml
  label: Met Office Met Office Land Observations Public API
  slug: met-office-met-office-land-observations-public-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/met-office/openapi/met-office-met-office-land-observations-public-api-api-openapi.yml
- filename: met-office-nearest-api-openapi.yml
  format: yaml
  label: Met Office Nearest API
  slug: met-office-nearest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/met-office/openapi/met-office-nearest-api-openapi.yml
- filename: met-office-objects-api-openapi.yml
  format: yaml
  label: Met Office Objects API
  slug: met-office-objects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/met-office/openapi/met-office-objects-api-openapi.yml
- filename: met-office-orders-api-openapi.yml
  format: yaml
  label: Met Office Orders API
  slug: met-office-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/met-office/openapi/met-office-orders-api-openapi.yml
- filename: met-office-point-api-openapi.yml
  format: yaml
  label: Met Office Point API
  slug: met-office-point-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/met-office/openapi/met-office-point-api-openapi.yml
- filename: met-office-runs-api-openapi.yml
  format: yaml
  label: Met Office Runs API
  slug: met-office-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/met-office/openapi/met-office-runs-api-openapi.yml
consequence_counts:
  read: 28
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Met Office Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 28
overview: 'Met Office exposes 28 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 28 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Met Office
provider_slug: met-office
slug: met-office-agentic-access
source_filename: met-office-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: generated\nsource: openapi/met-office-atmospheric-models-openapi.yml, openapi/met-office-blended-probabilistic-forecast-openapi.yml,\n  openapi/met-office-land-observations-openapi.yml, openapi/met-office-map-images-openapi.yml,\n  openapi/met-office-nswws-warnings-openapi.yml, openapi/met-office-site-specific-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 28\n  by_action_class:\n    connected: 28\n  by_consequence:\n    read: 28\n  human_in_the_loop_required: 0\noperations:\n- path: /orders\n  method: get\n  operationId: getOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{orderId}/latest\n\
  \  method: get\n  operationId: getOrderLatest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{orderId}/latest/{fileId}\n  method: get\n  operationId: getOrderLatestFileDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{orderId}/latest/{fileId}/data\n  method: get\n  operationId: getOrderLatestFileData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /runs\n  method: get\n  operationId: getAllRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /runs/{modelId}\n  method: get\n  operationId: getModelRuns\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collection_name}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collection_name}/instances\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collection_name}/instances/{instance_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collection_name}/instances/{instance_id}/locations\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collection_name}/instances/{instance_id}/locations/{location_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collection_name}/instances/{instance_id}/position\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conformance\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nearest\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{geohash}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders\n  method: get\n  operationId: getOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{orderId}/latest\n  method: get\n  operationId: getOrderLatest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{orderId}/latest/{fileId}\n  method: get\n  operationId: getOrderLatestFileDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /orders/{orderId}/latest/{fileId}/data\n  method: get\n  operationId: getOrderLatestFileData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /runs\n  method: get\n  operationId: getAllRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /objects/feed\n  method: get\n  operationId: objectsFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /objects/issued/{uuid}\n  method: get\n  operationId: objectsIssued\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /objects/updated/{uuid}\n  method: get\n  operationId: objectsUpdated\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /point/hourly\n  method: get\n  operationId: getForecastForPointUsingGET_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /point/three-hourly\n  method: get\n  operationId: getForecastForPointUsingGET_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /point/daily\n  method: get\n  operationId: getForecastForPointUsingGET_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/met-office/agentic-access/met-office-agentic-access.yml
summary_line: 28 operations
tags:
- Company
- Weather
- Climate
- Forecast
- Meteorology
- Government
- Open Data
- United Kingdom
---
