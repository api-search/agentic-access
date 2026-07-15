---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 10
api_specs:
- filename: preset-openapi.yml
  format: yaml
  label: Preset Auth API
  slug: preset-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/preset/refs/heads/main/openapi/preset-openapi.yml
- filename: preset-openapi.yml
  format: yaml
  label: Preset Teams and Workspaces API
  slug: preset-teams-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/preset/refs/heads/main/openapi/preset-openapi.yml
- filename: preset-openapi.yml
  format: yaml
  label: Preset Superset Dashboards API
  slug: preset-superset-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/preset/refs/heads/main/openapi/preset-openapi.yml
- filename: preset-openapi.yml
  format: yaml
  label: Preset Superset Charts API
  slug: preset-superset-charts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/preset/refs/heads/main/openapi/preset-openapi.yml
- filename: preset-openapi.yml
  format: yaml
  label: Preset Superset Datasets API
  slug: preset-superset-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/preset/refs/heads/main/openapi/preset-openapi.yml
- filename: preset-openapi.yml
  format: yaml
  label: Preset Superset Databases API
  slug: preset-superset-databases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/preset/refs/heads/main/openapi/preset-openapi.yml
- filename: preset-openapi.yml
  format: yaml
  label: Preset Superset SQL Lab API
  slug: preset-superset-sqllab-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/preset/refs/heads/main/openapi/preset-openapi.yml
consequence_counts:
  read: 10
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Preset Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 21
overview: 'Preset exposes 21 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 11 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Preset
provider_slug: preset
slug: preset-agentic-access
source_filename: preset-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/preset-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    acting: 11\n    connected: 10\n  by_consequence:\n    write: 11\n    read: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/auth/\n  method: post\n  operationId: createToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/teams/\n  method: get\n  operationId: getTeams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/teams/{teamName}/workspaces/\n  method: get\n  operationId: getWorkspaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/teams/{teamName}/workspaces/\n  method: post\n  operationId: createWorkspace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/teams/{teamName}/workspaces/{workspaceName}/guest-token/\n  method: post\n  operationId: createGuestToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n     \
  \ triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/dashboard/\n  method: get\n  operationId: getDashboards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/dashboard/\n  method: post\n  operationId: createDashboard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/dashboard/{pk}\n  method: get\n  operationId: getDashboard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/dashboard/{pk}\n  method: put\n  operationId: updateDashboard\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/dashboard/{pk}\n  method: delete\n  operationId: deleteDashboard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/chart/\n  method: get\n  operationId: getCharts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/chart/\n  method: post\n  operationId: createChart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/chart/{pk}\n  method: get\n  operationId: getChart\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/chart/data\n  method: post\n  operationId: getChartData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/dataset/\n  method: get\n  operationId: getDatasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/dataset/\n  method: post\n  operationId: createDataset\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/dataset/{pk}\n  method: get\n  operationId: getDataset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/database/\n  method: get\n  operationId: getDatabases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/database/\n  method: post\n  operationId: createDatabase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/v1/database/{pk}\n  method: get\n  operationId: getDatabase\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sqllab/execute/\n  method: post\n  operationId: executeSql\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/preset/refs/heads/main/agentic-access/preset-agentic-access.yml
summary_line: 21 operations · 11 acting
tags:
- BI
- Analytics
- Superset
- Dashboards
- Data Visualization
---
