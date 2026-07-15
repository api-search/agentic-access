---
acting_count: 21
action_class_counts:
  acting: 21
  connected: 16
api_specs:
- filename: xano-openapi.yml
  format: yaml
  label: Xano Metadata Tables & Schema API
  slug: xano-metadata-tables-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xano/refs/heads/main/openapi/xano-openapi.yml
- filename: xano-openapi.yml
  format: yaml
  label: Xano Metadata Records & Content API
  slug: xano-metadata-records-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xano/refs/heads/main/openapi/xano-openapi.yml
- filename: xano-openapi.yml
  format: yaml
  label: Xano Metadata Files API
  slug: xano-metadata-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xano/refs/heads/main/openapi/xano-openapi.yml
- filename: xano-openapi.yml
  format: yaml
  label: Xano Metadata Branches & Workspace API
  slug: xano-metadata-branches-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xano/refs/heads/main/openapi/xano-openapi.yml
- filename: xano-openapi.yml
  format: yaml
  label: Xano Metadata API Groups & Endpoints API
  slug: xano-metadata-api-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xano/refs/heads/main/openapi/xano-openapi.yml
- filename: xano-openapi.yml
  format: yaml
  label: Xano Metadata Auth & Access API
  slug: xano-metadata-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xano/refs/heads/main/openapi/xano-openapi.yml
consequence_counts:
  read: 16
  write: 21
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Xano Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 37
overview: 'Xano exposes 37 API operations that an AI agent could call, of which 21 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read and 21 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Xano
provider_slug: xano
slug: xano-agentic-access
source_filename: xano-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/xano-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 37\n  by_action_class:\n    connected: 16\n    acting: 21\n  by_consequence:\n    read: 16\n    write: 21\n  human_in_the_loop_required: 0\noperations:\n- path: /auth/me\n  method: get\n  operationId: getAuthenticatedUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspace\n  method: get\n  operationId: listWorkspaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspace/{workspace_id}\n  method:\
  \ get\n  operationId: getWorkspace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspace/{workspace_id}/branch\n  method: get\n  operationId: listBranches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspace/{workspace_id}/branch/{branch_id}\n  method: delete\n  operationId: deleteBranch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspace/{workspace_id}/export-schema\n  method: post\n  operationId: exportWorkspaceSchema\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspace/{workspace_id}/export\n  method: post\n  operationId: exportWorkspace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspace/{workspace_id}/files\n  method: get\n  operationId: listFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspace/{workspace_id}/files/upload\n  method: post\n  operationId: uploadFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspace/{workspace_id}/files/{file_id}\n  method: delete\n  operationId: deleteFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspace/{workspace_id}/files/delete-batch\n  method: post\n  operationId: deleteFilesBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspace/{workspace_id}/table\n  method: get\n  operationId: listTables\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspace/{workspace_id}/table\n  method: post\n  operationId: createTable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspace/{workspace_id}/table/{table_id}\n  method: get\n  operationId: getTable\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspace/{workspace_id}/table/{table_id}\n  method: patch\n  operationId: updateTable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspace/{workspace_id}/table/{table_id}\n  method: delete\n  operationId: deleteTable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspace/{workspace_id}/table/{table_id}/schema\n  method: get\n  operationId: getTableSchema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspace/{workspace_id}/table/{table_id}/schema\n  method: put\n  operationId: replaceTableSchema\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspace/{workspace_id}/table/{table_id}/schema/{column_id}\n  method: get\n  operationId: getColumn\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspace/{workspace_id}/table/{table_id}/schema/{column_id}\n  method: patch\n  operationId: renameColumn\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspace/{workspace_id}/table/{table_id}/schema/{column_id}\n  method: delete\n  operationId: deleteColumn\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspace/{workspace_id}/table/{table_id}/index\n  method: get\n  operationId: listIndexes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspace/{workspace_id}/table/{table_id}/index\n  method: put\n  operationId: replaceIndexes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspace/{workspace_id}/table/{table_id}/content\n  method: get\n  operationId: listRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n \
  \   audit: none\n- path: /workspace/{workspace_id}/table/{table_id}/content\n  method: post\n  operationId: createRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspace/{workspace_id}/table/{table_id}/content/bulk\n  method: post\n  operationId: createRecordsBulk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspace/{workspace_id}/table/{table_id}/content/{record_id}\n  method: get\n  operationId: getRecord\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspace/{workspace_id}/table/{table_id}/content/{record_id}\n  method: patch\n  operationId: updateRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspace/{workspace_id}/table/{table_id}/content/{record_id}\n  method: delete\n  operationId: deleteRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspace/{workspace_id}/table/{table_id}/content/search\n  method: post\n  operationId: searchRecords\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspace/{workspace_id}/apigroup\n  method: get\n  operationId: listApiGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspace/{workspace_id}/apigroup\n  method: post\n  operationId: createApiGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspace/{workspace_id}/apigroup/{apigroup_id}\n  method: get\n  operationId: getApiGroup\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspace/{workspace_id}/apigroup/{apigroup_id}\n  method: delete\n  operationId: deleteApiGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspace/{workspace_id}/apigroup/{apigroup_id}/openapi\n  method: get\n  operationId: getApiGroupOpenApi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspace/{workspace_id}/apigroup/{apigroup_id}/api\n  method: get\n  operationId: listApiEndpoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspace/{workspace_id}/apigroup/{apigroup_id}/api\n\
  \  method: post\n  operationId: createApiEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xano/refs/heads/main/agentic-access/xano-agentic-access.yml
summary_line: 37 operations · 21 acting
tags:
- No Code
- Backend as a Service
- BaaS
- API Builder
- Database
- Serverless
---
