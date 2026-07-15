---
acting_count: 16
action_class_counts:
  acting: 16
  connected: 14
api_specs:
- filename: gooddata-openapi.yml
  format: yaml
  label: GoodData Workspaces API
  slug: gooddata-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gooddata/refs/heads/main/openapi/gooddata-openapi.yml
- filename: gooddata-openapi.yml
  format: yaml
  label: GoodData Data Sources API
  slug: gooddata-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gooddata/refs/heads/main/openapi/gooddata-openapi.yml
- filename: gooddata-openapi.yml
  format: yaml
  label: GoodData Logical Data Model API
  slug: gooddata-logical-data-model-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gooddata/refs/heads/main/openapi/gooddata-openapi.yml
- filename: gooddata-openapi.yml
  format: yaml
  label: GoodData Metrics API
  slug: gooddata-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gooddata/refs/heads/main/openapi/gooddata-openapi.yml
- filename: gooddata-openapi.yml
  format: yaml
  label: GoodData Visualizations & Dashboards API
  slug: gooddata-visualizations-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gooddata/refs/heads/main/openapi/gooddata-openapi.yml
- filename: gooddata-openapi.yml
  format: yaml
  label: GoodData Execution / AFM API
  slug: gooddata-execution-afm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gooddata/refs/heads/main/openapi/gooddata-openapi.yml
- filename: gooddata-openapi.yml
  format: yaml
  label: GoodData Users & Permissions API
  slug: gooddata-users-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gooddata/refs/heads/main/openapi/gooddata-openapi.yml
consequence_counts:
  read: 14
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Gooddata Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 30
overview: 'GoodData exposes 30 API operations that an AI agent could call, of which 16 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read and 16 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: GoodData
provider_slug: gooddata
slug: gooddata-agentic-access
source_filename: gooddata-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/gooddata-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 30\n  by_action_class:\n    connected: 14\n    acting: 16\n  by_consequence:\n    read: 14\n    write: 16\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/entities/workspaces\n  method: get\n  operationId: getWorkspaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/entities/workspaces\n  method: post\n  operationId: createWorkspace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/entities/workspaces/{workspaceId}\n  method: get\n  operationId: getWorkspace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/entities/workspaces/{workspaceId}\n  method: put\n  operationId: updateWorkspace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/entities/workspaces/{workspaceId}\n  method: delete\n  operationId: deleteWorkspace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n    \
  \  human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/entities/dataSources\n  method: get\n  operationId: getDataSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/entities/dataSources\n  method: post\n  operationId: createDataSource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/entities/dataSources/{dataSourceId}\n  method: get\n  operationId: getDataSource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/entities/dataSources/{dataSourceId}\n\
  \  method: delete\n  operationId: deleteDataSource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/actions/dataSources/{dataSourceId}/test\n  method: post\n  operationId: testDataSource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/layout/workspaces/{workspaceId}/logicalModel\n  method: get\n  operationId: getLogicalModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/layout/workspaces/{workspaceId}/logicalModel\n\
  \  method: put\n  operationId: setLogicalModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/entities/workspaces/{workspaceId}/metrics\n  method: get\n  operationId: getMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/entities/workspaces/{workspaceId}/metrics\n  method: post\n  operationId: createMetric\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/entities/workspaces/{workspaceId}/metrics/{objectId}\n\
  \  method: get\n  operationId: getMetric\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/entities/workspaces/{workspaceId}/metrics/{objectId}\n  method: delete\n  operationId: deleteMetric\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/entities/workspaces/{workspaceId}/visualizationObjects\n  method: get\n  operationId: getVisualizationObjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/entities/workspaces/{workspaceId}/visualizationObjects\n  method: post\n  operationId: createVisualizationObject\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/entities/workspaces/{workspaceId}/analyticalDashboards\n  method: get\n  operationId: getAnalyticalDashboards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/entities/workspaces/{workspaceId}/analyticalDashboards\n  method: post\n  operationId: createAnalyticalDashboard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/actions/workspaces/{workspaceId}/execution/afm/execute\n\
  \  method: post\n  operationId: computeReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/actions/workspaces/{workspaceId}/execution/afm/execute/result/{resultId}\n  method: get\n  operationId: retrieveResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/entities/users\n  method: get\n  operationId: getUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/entities/users\n  method: post\n  operationId: createUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/entities/users/{userId}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/entities/users/{userId}\n  method: delete\n  operationId: deleteUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/entities/userGroups\n  method: get\n  operationId: getUserGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/entities/userGroups\n\
  \  method: post\n  operationId: createUserGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/layout/workspaces/{workspaceId}/permissions\n  method: get\n  operationId: getWorkspacePermissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/layout/workspaces/{workspaceId}/permissions\n  method: put\n  operationId: setWorkspacePermissions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gooddata/refs/heads/main/agentic-access/gooddata-agentic-access.yml
summary_line: 30 operations · 16 acting
tags:
- Analytics
- Business Intelligence
- Embedded Analytics
- Dashboards
- Data
---
