---
acting_count: 0
action_class_counts:
  connected: 32
api_specs:
- filename: hydro-quebec-catalog-api-openapi.yml
  format: yaml
  label: Hydro-Québec Catalog API
  slug: hydro-quebec-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hydro-quebec/refs/heads/main/openapi/hydro-quebec-catalog-api-openapi.yml
- filename: hydro-quebec-dataset-api-openapi.yml
  format: yaml
  label: Hydro-Québec Dataset API
  slug: hydro-quebec-dataset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hydro-quebec/refs/heads/main/openapi/hydro-quebec-dataset-api-openapi.yml
consequence_counts:
  read: 32
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Hydro Quebec Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 32
overview: 'Hydro-Québec exposes 32 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 32 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Hydro-Québec
provider_slug: hydro-quebec
slug: hydro-quebec-agentic-access
source_filename: hydro-quebec-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: generated\nsource: openapi/hydro-quebec-open-data-explore-api-v2-0-openapi.json, openapi/hydro-quebec-open-data-explore-api-v2-1-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 32\n  by_action_class:\n    connected: 32\n  by_consequence:\n    read: 32\n  human_in_the_loop_required: 0\noperations:\n- path: /catalog/datasets\n  method: get\n  operationId: getDatasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/exports\n  method: get\n  operationId: listExportFormats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /catalog/exports/{format}\n  method: get\n  operationId: exportDatasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/exports/csv\n  method: get\n  operationId: exportCatalogCSV\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/exports/dcat{dcat_ap_format}\n  method: get\n  operationId: exportCatalogDCAT\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/facets\n  method: get\n  operationId: getDatasetsFacets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/datasets/{dataset_id}/records\n  method: get\n\
  \  operationId: getRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/datasets/{dataset_id}/exports\n  method: get\n  operationId: listDatasetExportFormats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/datasets/{dataset_id}/exports/{format}\n  method: get\n  operationId: exportRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/datasets/{dataset_id}/exports/csv\n  method: get\n  operationId: exportRecordsCSV\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/datasets/{dataset_id}/exports/parquet\n  method: get\n  operationId:\
  \ exportRecordsParquet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/datasets/{dataset_id}/exports/gpx\n  method: get\n  operationId: exportRecordsGPX\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/datasets/{dataset_id}\n  method: get\n  operationId: getDataset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/datasets/{dataset_id}/facets\n  method: get\n  operationId: getRecordsFacets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/datasets/{dataset_id}/attachments\n  method: get\n  operationId: getDatasetAttachments\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/datasets/{dataset_id}/records/{record_id}\n  method: get\n  operationId: getRecord\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/datasets\n  method: get\n  operationId: getDatasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/exports\n  method: get\n  operationId: listExportFormats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/exports/{format}\n  method: get\n  operationId: exportDatasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /catalog/exports/csv\n  method: get\n  operationId: exportCatalogCSV\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/exports/dcat{dcat_ap_format}\n  method: get\n  operationId: exportCatalogDCAT\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/facets\n  method: get\n  operationId: getDatasetsFacets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/datasets/{dataset_id}/records\n  method: get\n  operationId: getRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/datasets/{dataset_id}/exports\n\
  \  method: get\n  operationId: listDatasetExportFormats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/datasets/{dataset_id}/exports/{format}\n  method: get\n  operationId: exportRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/datasets/{dataset_id}/exports/csv\n  method: get\n  operationId: exportRecordsCSV\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/datasets/{dataset_id}/exports/parquet\n  method: get\n  operationId: exportRecordsParquet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/datasets/{dataset_id}/exports/gpx\n\
  \  method: get\n  operationId: exportRecordsGPX\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/datasets/{dataset_id}\n  method: get\n  operationId: getDataset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/datasets/{dataset_id}/facets\n  method: get\n  operationId: getRecordsFacets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/datasets/{dataset_id}/attachments\n  method: get\n  operationId: getDatasetAttachments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/datasets/{dataset_id}/records/{record_id}\n  method: get\n  operationId:\
  \ getRecord\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hydro-quebec/refs/heads/main/agentic-access/hydro-quebec-agentic-access.yml
summary_line: 32 operations
tags:
- Energy
- Canada
- Utilities
- Electricity
- Grid
- Energy Markets
- Renewables
- Open Data
- Demand Response
- Carbon
---
