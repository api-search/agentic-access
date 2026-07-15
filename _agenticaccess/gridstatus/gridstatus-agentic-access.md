---
acting_count: 0
action_class_counts:
  connected: 25
api_specs:
- filename: gridstatus-openapi.yml
  format: yaml
  label: Grid Status Datasets API
  slug: gridstatus-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridstatus/refs/heads/main/openapi/gridstatus-openapi.yml
- filename: gridstatus-openapi.yml
  format: yaml
  label: Grid Status Dataset Query API
  slug: gridstatus-dataset-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridstatus/refs/heads/main/openapi/gridstatus-openapi.yml
- filename: gridstatus-openapi.yml
  format: yaml
  label: Grid Status Pricing Locations API
  slug: gridstatus-pricing-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridstatus/refs/heads/main/openapi/gridstatus-openapi.yml
- filename: gridstatus-openapi.yml
  format: yaml
  label: Grid Status Constraints API
  slug: gridstatus-constraints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridstatus/refs/heads/main/openapi/gridstatus-openapi.yml
- filename: gridstatus-openapi.yml
  format: yaml
  label: Grid Status Reports and Block Pricing API
  slug: gridstatus-reports-block-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridstatus/refs/heads/main/openapi/gridstatus-openapi.yml
- filename: gridstatus-openapi.yml
  format: yaml
  label: Grid Status Bulk Exports and Usage API
  slug: gridstatus-bulk-exports-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridstatus/refs/heads/main/openapi/gridstatus-openapi.yml
consequence_counts:
  read: 25
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Gridstatus Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 25
overview: 'Grid Status exposes 25 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 25 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Grid Status
provider_slug: gridstatus
slug: gridstatus-agentic-access
source_filename: gridstatus-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/gridstatus-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 25\n  by_action_class:\n    connected: 25\n  by_consequence:\n    read: 25\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: apiInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets\n  method: get\n  operationId: listDatasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets/{dataset_id}\n  method: get\n  operationId: getDatasetMetadata\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets/{dataset_id}/audit\n  method: get\n  operationId: getDatasetAudit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets/{dataset_id}/query\n  method: get\n  operationId: queryDataset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets/{dataset_id}/query/{filter_column_id}/{filter_value_path}\n  method: get\n  operationId: queryDatasetByColumnValue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dataset-updates/{dataset_id}\n  method: get\n  operationId: getDatasetUpdates\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /block-pricing/{iso}\n  method: get\n  operationId: getBlockPricing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/daily_peak/{iso}\n  method: get\n  operationId: getDailyPeakReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pricing_locations\n  method: get\n  operationId: listPricingLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pricing_locations/nearby\n  method: get\n  operationId: listNearbyPricingLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /pricing_locations/{gs_entity_id}\n  method: get\n  operationId: getPricingLocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /constraints\n  method: get\n  operationId: listConstraints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /constraints/contingencies\n  method: get\n  operationId: listContingencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /constraints/binding\n  method: get\n  operationId: listConstraintBindingRows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /constraints/binding/counts\n  method: get\n  operationId:\
  \ listConstraintBindingCounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /constraints/binding/costs\n  method: get\n  operationId: listConstraintBindingCosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /constraints/binding/heat_map\n  method: get\n  operationId: getConstraintBindingHeatMap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /constraints/{gs_entity_id}\n  method: get\n  operationId: getConstraint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /constraints/{constraint_id}/shift-factors\n  method: get\n  operationId: listShiftFactors\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /constraints/{constraint_id}/stats\n  method: get\n  operationId: listConstraintStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /constraints/locations/{location_gs_entity_id}/shift-factors\n  method: get\n  operationId: listShiftFactorsForLocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /csv-exports/{dataset_id}\n  method: get\n  operationId: listCsvExports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /csv-exports/{dataset_id}/{export_date}\n  method: get\n  operationId: getCsvExportUrl\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api_usage\n  method: get\n  operationId: getApiUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gridstatus/refs/heads/main/agentic-access/gridstatus-agentic-access.yml
summary_line: 25 operations
tags:
- Day-Ahead Prices
- Electricity
- Grid Data
- Energy Markets
- LMP
- Load
- Fuel Mix
- Open Source
---
