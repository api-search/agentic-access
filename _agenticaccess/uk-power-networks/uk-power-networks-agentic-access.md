---
acting_count: 0
action_class_counts:
  connected: 32
api_specs:
- filename: uk-power-networks-catalog-api-openapi.yml
  format: yaml
  label: UK Power Networks Catalog API
  slug: uk-power-networks-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uk-power-networks/refs/heads/main/openapi/uk-power-networks-catalog-api-openapi.yml
- filename: uk-power-networks-dataset-api-openapi.yml
  format: yaml
  label: UK Power Networks Dataset API
  slug: uk-power-networks-dataset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uk-power-networks/refs/heads/main/openapi/uk-power-networks-dataset-api-openapi.yml
consequence_counts:
  read: 32
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Uk Power Networks Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 32
overview: 'UK Power Networks exposes 32 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 32 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: UK Power Networks
provider_slug: uk-power-networks
slug: uk-power-networks-agentic-access
source_filename: uk-power-networks-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: generated\nsource: openapi/uk-power-networks-explore-api-v2-0-openapi.json, openapi/uk-power-networks-explore-api-v2-1-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 32\n  by_action_class:\n    connected: 32\n  by_consequence:\n    read: 32\n  human_in_the_loop_required: 0\noperations:\n- path: /catalog/datasets\n  method: get\n  operationId: getDatasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/exports\n  method: get\n  operationId: listExportFormats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /catalog/exports/{format}\n  method: get\n  operationId: exportDatasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/exports/csv\n  method: get\n  operationId: exportCatalogCSV\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/exports/dcat{dcat_ap_format}\n  method: get\n  operationId: exportCatalogDCAT\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/facets\n  method: get\n  operationId: getDatasetsFacets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/datasets/{dataset_id}/records\n  method: get\n  operationId:\
  \ getRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/datasets/{dataset_id}/exports\n  method: get\n  operationId: listDatasetExportFormats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/datasets/{dataset_id}/exports/{format}\n  method: get\n  operationId: exportRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/datasets/{dataset_id}/exports/csv\n  method: get\n  operationId: exportRecordsCSV\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/datasets/{dataset_id}/exports/parquet\n  method: get\n  operationId: exportRecordsParquet\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/datasets/{dataset_id}/exports/gpx\n  method: get\n  operationId: exportRecordsGPX\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/datasets/{dataset_id}\n  method: get\n  operationId: getDataset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/datasets/{dataset_id}/facets\n  method: get\n  operationId: getRecordsFacets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/datasets/{dataset_id}/attachments\n  method: get\n  operationId: getDatasetAttachments\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/datasets/{dataset_id}/records/{record_id}\n  method: get\n  operationId: getRecord\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/datasets\n  method: get\n  operationId: getDatasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/exports\n  method: get\n  operationId: listExportFormats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/exports/{format}\n  method: get\n  operationId: exportDatasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /catalog/exports/csv\n  method: get\n  operationId: exportCatalogCSV\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/exports/dcat{dcat_ap_format}\n  method: get\n  operationId: exportCatalogDCAT\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/facets\n  method: get\n  operationId: getDatasetsFacets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/datasets/{dataset_id}/records\n  method: get\n  operationId: getRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/datasets/{dataset_id}/exports\n  method: get\n\
  \  operationId: listDatasetExportFormats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/datasets/{dataset_id}/exports/{format}\n  method: get\n  operationId: exportRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/datasets/{dataset_id}/exports/csv\n  method: get\n  operationId: exportRecordsCSV\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/datasets/{dataset_id}/exports/parquet\n  method: get\n  operationId: exportRecordsParquet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/datasets/{dataset_id}/exports/gpx\n  method: get\n\
  \  operationId: exportRecordsGPX\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/datasets/{dataset_id}\n  method: get\n  operationId: getDataset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/datasets/{dataset_id}/facets\n  method: get\n  operationId: getRecordsFacets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/datasets/{dataset_id}/attachments\n  method: get\n  operationId: getDatasetAttachments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/datasets/{dataset_id}/records/{record_id}\n  method: get\n  operationId: getRecord\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uk-power-networks/refs/heads/main/agentic-access/uk-power-networks-agentic-access.yml
summary_line: 32 operations
tags:
- Energy
- United Kingdom
- Utilities
- Electricity
- Grid
- Distribution Network
- Open Data
- Smart Metering
- DER
- EV Charging
- Carbon
- Energy Markets
---
