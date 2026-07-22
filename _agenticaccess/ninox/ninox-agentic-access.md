---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 8
api_specs:
- filename: ninox-public-openapi-original.json
  format: json
  label: Ninox Public API
  slug: ninox-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ninox/refs/heads/main/openapi/ninox-public-openapi-original.json
consequence_counts:
  read: 8
  safety-critical: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 15
kind: agentic-access
layout: agentic-access
method: generated
name: Ninox Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/workspace/{workspaceId}/modules
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/workspace/{workspaceId}/modules/{moduleName}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/v1/workspace/{workspaceId}/modules/{moduleName}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/workspace/{workspaceId}/modules/{moduleName}/tables
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/workspace/{workspaceId}/modules/{moduleName}/tables/{tableName}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/v1/workspace/{workspaceId}/modules/{moduleName}/tables/{tableName}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/workspace/{workspaceId}/modules/{moduleName}/tables/{tableName}/fields
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/workspace/{workspaceId}/modules/{moduleName}/tables/{tableName}/fields/batch
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/workspace/{workspaceId}/modules/{moduleName}/tables/{tableName}/fields/batch
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/workspace/{workspaceId}/modules/{moduleName}/tables/{tableName}/fields/{fieldName}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/v1/workspace/{workspaceId}/modules/{moduleName}/tables/{tableName}/fields/{fieldName}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/workspace/{workspaceId}/modules/{moduleName}/tables/{tableName}/records
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/workspace/{workspaceId}/modules/{moduleName}/tables/{tableName}/records
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/v1/workspace/{workspaceId}/modules/{moduleName}/tables/{tableName}/records
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/workspace/{workspaceId}/modules/{moduleName}/tables/{tableName}/records/import/csv
operation_count: 23
overview: 'Ninox exposes 23 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 15 safety-critical.


  15 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Ninox
provider_slug: ninox
slug: ninox-agentic-access
source_filename: ninox-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/ninox-public-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    acting: 15\n    connected: 8\n  by_consequence:\n    safety-critical: 15\n    read: 8\n  human_in_the_loop_required: 15\noperations:\n- path: /api/v1/workspace/{workspaceId}/modules/{moduleName}/tables/{tableName}/fields\n  method: post\n  operationId: FieldsV1Controller_createField\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n \
  \   audit: required\n- path: /api/v1/workspace/{workspaceId}/modules/{moduleName}/tables/{tableName}/fields\n  method: get\n  operationId: FieldsV1Controller_getFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/workspace/{workspaceId}/modules/{moduleName}/tables/{tableName}/fields/batch\n  method: post\n  operationId: FieldsV1Controller_createFieldsBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/workspace/{workspaceId}/modules/{moduleName}/tables/{tableName}/fields/batch\n  method: delete\n  operationId: FieldsV1Controller_deleteFieldsBatch\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/workspace/{workspaceId}/modules/{moduleName}/tables/{tableName}/fields/{fieldName}\n  method: delete\n  operationId: FieldsV1Controller_deleteField\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/workspace/{workspaceId}/modules/{moduleName}/tables/{tableName}/fields/{fieldName}\n  method: get\n  operationId: FieldsV1Controller_getField\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/workspace/{workspaceId}/modules/{moduleName}/tables/{tableName}/fields/{fieldName}\n  method: patch\n  operationId: FieldsV1Controller_updateField\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/workspace/{workspaceId}/modules\n  method: post\n  operationId: ModulesV1Controller_createModule\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/workspace/{workspaceId}/modules\n\
  \  method: get\n  operationId: ModulesV1Controller_getModules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/workspace/{workspaceId}/modules/{moduleName}\n  method: delete\n  operationId: ModulesV1Controller_deleteModule\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/workspace/{workspaceId}/modules/{moduleName}\n  method: get\n  operationId: ModulesV1Controller_getModule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/workspace/{workspaceId}/modules/{moduleName}\n  method: patch\n\
  \  operationId: ModulesV1Controller_updateModule\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/workspace/{workspaceId}/modules/{moduleName}/tables/{tableName}/records\n  method: post\n  operationId: RowsV1Controller_addRows\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/workspace/{workspaceId}/modules/{moduleName}/tables/{tableName}/records\n  method: delete\n  operationId: RowsV1Controller_deleteRows\n  x-agentic-access:\n   \
  \ action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/workspace/{workspaceId}/modules/{moduleName}/tables/{tableName}/records\n  method: get\n  operationId: RowsV1Controller_getRows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/workspace/{workspaceId}/modules/{moduleName}/tables/{tableName}/records\n  method: patch\n  operationId: RowsV1Controller_updateRows\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /api/v1/workspace/{workspaceId}/modules/{moduleName}/tables/{tableName}/records/import/csv\n  method: post\n  operationId: RowsV1Controller_importCSV\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/workspace/{workspaceId}/modules/{moduleName}/tables\n  method: post\n  operationId: TablesV1Controller_createTable\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/workspace/{workspaceId}/modules/{moduleName}/tables\n\
  \  method: get\n  operationId: TablesV1Controller_getTables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/workspace/{workspaceId}/modules/{moduleName}/tables/{tableName}\n  method: delete\n  operationId: TablesV1Controller_deleteTable\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/workspace/{workspaceId}/modules/{moduleName}/tables/{tableName}\n  method: get\n  operationId: TablesV1Controller_getTable\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/workspace/{workspaceId}/modules/{moduleName}/tables/{tableName}\n\
  \  method: patch\n  operationId: TablesV1Controller_updateTable\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/workspace/{workspaceId}\n  method: get\n  operationId: WorkspacesV1Controller_getWorkspace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ninox/refs/heads/main/agentic-access/ninox-agentic-access.yml
summary_line: 23 operations · 15 acting · 15 human-in-the-loop
tags:
- Company
- Low-Code
- Database
- No-Code
- Application Development
- Workflow Automation
- Business Apps
- Productivity
---
