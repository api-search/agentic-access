---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 13
api_specs:
- filename: databento-openapi.yml
  format: yaml
  label: Databento Historical Timeseries API
  slug: databento-historical-timeseries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/databento/refs/heads/main/openapi/databento-openapi.yml
- filename: databento-openapi.yml
  format: yaml
  label: Databento Metadata API
  slug: databento-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/databento/refs/heads/main/openapi/databento-openapi.yml
- filename: databento-openapi.yml
  format: yaml
  label: Databento Symbology API
  slug: databento-symbology-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/databento/refs/heads/main/openapi/databento-openapi.yml
- filename: databento-openapi.yml
  format: yaml
  label: Databento Batch API
  slug: databento-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/databento/refs/heads/main/openapi/databento-openapi.yml
- filename: databento-openapi.yml
  format: yaml
  label: Databento Reference API
  slug: databento-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/databento/refs/heads/main/openapi/databento-openapi.yml
consequence_counts:
  read: 13
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Databento Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 20
overview: 'Databento exposes 20 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Databento
provider_slug: databento
slug: databento-agentic-access
source_filename: databento-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/databento-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    connected: 13\n    acting: 7\n  by_consequence:\n    read: 13\n    write: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /metadata.list_publishers\n  method: get\n  operationId: listPublishers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metadata.list_datasets\n  method: get\n  operationId: listDatasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metadata.list_schemas\n\
  \  method: get\n  operationId: listSchemas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metadata.list_fields\n  method: get\n  operationId: listFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metadata.list_unit_prices\n  method: get\n  operationId: listUnitPrices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metadata.get_dataset_condition\n  method: get\n  operationId: getDatasetCondition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metadata.get_dataset_range\n  method: get\n  operationId: getDatasetRange\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metadata.get_record_count\n  method: get\n  operationId: getRecordCount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metadata.get_billable_size\n  method: get\n  operationId: getBillableSize\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metadata.get_cost\n  method: get\n  operationId: getCost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /timeseries.get_range\n  method: get\n  operationId: timeseriesGetRange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /timeseries.get_range\n  method: post\n  operationId: timeseriesGetRangePost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /symbology.resolve\n  method: post\n  operationId: symbologyResolve\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /batch.submit_job\n  method: post\n  operationId: batchSubmitJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /batch.list_jobs\n  method: get\n  operationId: batchListJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /batch.list_files\n  method: get\n  operationId: batchListFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /security_master.get_range\n  method: post\n  operationId: securityMasterGetRange\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /security_master.get_last\n  method: post\n  operationId: securityMasterGetLast\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /corporate_actions.get_range\n  method: post\n  operationId: corporateActionsGetRange\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /adjustment_factors.get_range\n  method: post\n  operationId: adjustmentFactorsGetRange\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/databento/refs/heads/main/agentic-access/databento-agentic-access.yml
summary_line: 20 operations · 7 acting
tags:
- Market Data
- Financial Data
- Reference Data
- Historical Market Data
- Trading
---
