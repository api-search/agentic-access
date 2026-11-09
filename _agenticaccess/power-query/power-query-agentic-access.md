---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 3
api_specs:
- filename: power-query-items-api-openapi.yml
  format: yaml
  label: Power Query Items API
  slug: power-query-items-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/power-query/openapi/power-query-items-api-openapi.yml
- filename: power-query-background-jobs-api-openapi.yml
  format: yaml
  label: Power Query Background Jobs API
  slug: power-query-background-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/power-query/openapi/power-query-background-jobs-api-openapi.yml
- filename: power-query-query-execution-api-openapi.yml
  format: yaml
  label: Power Query Query Execution API
  slug: power-query-query-execution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/power-query/openapi/power-query-query-execution-api-openapi.yml
consequence_counts:
  read: 3
  safety-critical: 1
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Power Query Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /workspaces/{workspaceId}/dataflows/{dataflowId}/updateDefinition
operation_count: 13
overview: 'Power Query exposes 13 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read, 9 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Power Query
provider_slug: power-query
slug: power-query-agentic-access
source_filename: power-query-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/power-query-background-jobs-api-openapi.yml, openapi/power-query-items-api-openapi.yml,\n  openapi/power-query-query-execution-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    acting: 10\n    connected: 3\n  by_consequence:\n    write: 9\n    read: 3\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /workspaces/{workspaceId}/dataflows/{dataflowId}/jobs/execute/schedules\n  method: post\n  operationId: BackgroundJobs_ScheduleExecute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/dataflows/{dataflowId}/jobs/applyChanges/schedules\n  method: post\n  operationId: BackgroundJobs_ScheduleApplyChanges\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/dataflows/{dataflowId}/jobs/execute/instances\n  method: post\n  operationId: BackgroundJobs_RunOnDemandExecute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/dataflows/{dataflowId}/jobs/applyChanges/instances\n\
  \  method: post\n  operationId: BackgroundJobs_RunOnDemandApplyChanges\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/dataflows\n  method: get\n  operationId: Items_ListDataflows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}/dataflows\n  method: post\n  operationId: Items_CreateDataflow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/dataflows/{dataflowId}\n\
  \  method: get\n  operationId: Items_GetDataflow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}/dataflows/{dataflowId}\n  method: patch\n  operationId: Items_UpdateDataflow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/dataflows/{dataflowId}\n  method: delete\n  operationId: Items_DeleteDataflow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/dataflows/{dataflowId}/getDefinition\n\
  \  method: post\n  operationId: Items_GetDataflowDefinition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/dataflows/{dataflowId}/updateDefinition\n  method: post\n  operationId: Items_UpdateDataflowDefinition\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /workspaces/{workspaceId}/dataflows/{dataflowId}/parameters\n  method: get\n  operationId: Items_DiscoverDataflowParameters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n   \
  \ subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}/dataflows/{dataflowId}/executeQuery\n  method: post\n  operationId: QueryExecution_ExecuteQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/power-query/agentic-access/power-query-agentic-access.yml
summary_line: 13 operations · 10 acting · 1 human-in-the-loop
tags:
- Business Intelligence
- Data Integration
- Data Transformation
- ETL
- Microsoft
- Microsoft Fabric
- Power BI
- Dataflows
- M Language
- Data Connectors
- Self-Service ETL
---
