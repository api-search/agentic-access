---
acting_count: 0
action_class_counts:
  connected: 7
api_specs:
- filename: finra-async-api-openapi.yml
  format: yaml
  label: FINRA Async API
  slug: finra-async-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finra/refs/heads/main/openapi/finra-async-api-openapi.yml
- filename: finra-datasets-api-openapi.yml
  format: yaml
  label: FINRA Datasets API
  slug: finra-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finra/refs/heads/main/openapi/finra-datasets-api-openapi.yml
- filename: finra-metadata-api-openapi.yml
  format: yaml
  label: FINRA Metadata API
  slug: finra-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finra/refs/heads/main/openapi/finra-metadata-api-openapi.yml
- filename: finra-partitions-api-openapi.yml
  format: yaml
  label: FINRA Partitions API
  slug: finra-partitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finra/refs/heads/main/openapi/finra-partitions-api-openapi.yml
consequence_counts:
  read: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Finra Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'FINRA exposes 7 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: FINRA
provider_slug: finra
slug: finra-agentic-access
source_filename: finra-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/finra-async-api-openapi.yml, openapi/finra-datasets-api-openapi.yml, openapi/finra-metadata-api-openapi.yml,\n  openapi/finra-partitions-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 7\n  by_consequence:\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /async-requests/group/{group}/name/{dataset}/{requestId}\n  method: get\n  operationId: getAsyncRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets\n  method: get\n  operationId: listDatasets\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/group/{group}/name/{dataset}\n  method: get\n  operationId: queryDataset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/group/{group}/name/{dataset}\n  method: post\n  operationId: queryDatasetAdvanced\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/group/{group}/name/{dataset}/id/{id}\n  method: get\n  operationId: getDatasetRecord\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metadata/group/{group}/name/{dataset}\n  method: get\n  operationId: getDatasetMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /partitions/group/{group}/name/{dataset}\n  method: get\n  operationId: getDatasetPartitions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finra/refs/heads/main/agentic-access/finra-agentic-access.yml
summary_line: 7 operations
tags:
- Compliance
- Finance
- Regulations
- Securities
- Market Data
---
