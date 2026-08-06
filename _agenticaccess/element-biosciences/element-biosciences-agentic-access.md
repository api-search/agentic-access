---
acting_count: 0
action_class_counts:
  connected: 16
api_specs:
- filename: element-biosciences-cloud-api-openapi-original.yml
  format: yaml
  label: Element Biosciences Cloud API
  slug: cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/element-biosciences/refs/heads/main/openapi/element-biosciences-cloud-api-openapi-original.yml
consequence_counts:
  read: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Element Biosciences Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'Element Biosciences exposes 16 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Element Biosciences
provider_slug: element-biosciences
slug: element-biosciences-agentic-access
source_filename: element-biosciences-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: generated\nsource: openapi/element-biosciences-cloud-api-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 16\n  by_consequence:\n    read: 16\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/auth\n  method: get\n  operationId: AuthService_GetAuth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/executions\n  method: get\n  operationId: ExecutionService_ListExecutions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/executions/{execution_id}/credentials\n\
  \  method: get\n  operationId: ExecutionService_GetExecutionDownloadCredentials\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/executions/{execution_id}/files\n  method: get\n  operationId: ExecutionService_ListExecutionFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/executions/{execution_id}/logs\n  method: get\n  operationId: ExecutionService_GetExecutionLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/executions/{id}\n  method: get\n  operationId: ExecutionService_GetExecution\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/instruments\n\
  \  method: get\n  operationId: InstrumentService_ListInstruments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/instruments/{serial_number}\n  method: get\n  operationId: InstrumentService_GetInstrument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/runs\n  method: get\n  operationId: RunService_ListRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/runs/{id}\n  method: get\n  operationId: RunService_GetRun\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/runs/{run_id}/credentials\n  method: get\n  operationId: RunService_GetRunDownloadCredentials\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/runs/{run_id}/files\n  method: get\n  operationId: RunService_ListRunFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/storage-connections\n  method: get\n  operationId: StorageConnectionService_ListStorageConnections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/storage-connections/{id}\n  method: get\n  operationId: StorageConnectionService_GetStorageConnection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/storage-connections/{storage_connection_id}/credentials\n  method: get\n  operationId: StorageConnectionService_GetDownloadCredentials\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/storage-connections/{storage_connection_id}/files\n  method: get\n  operationId: StorageConnectionService_ListFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/element-biosciences/refs/heads/main/agentic-access/element-biosciences-agentic-access.yml
summary_line: 16 operations
tags:
- Company
- Genomics
- DNA Sequencing
- Life Sciences
- Bioinformatics
- Multiomics
- Laboratory
- Scientific Instruments
- Cloud Storage
- Biotechnology
---
