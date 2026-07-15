---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 16
api_specs:
- filename: propeller-aero-openapi.yml
  format: yaml
  label: Propeller Organizations API
  slug: propeller-aero-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propeller-aero/refs/heads/main/openapi/propeller-aero-openapi.yml
- filename: propeller-aero-openapi.yml
  format: yaml
  label: Propeller Sites API
  slug: propeller-aero-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propeller-aero/refs/heads/main/openapi/propeller-aero-openapi.yml
- filename: propeller-aero-openapi.yml
  format: yaml
  label: Propeller Surveys API
  slug: propeller-aero-surveys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propeller-aero/refs/heads/main/openapi/propeller-aero-openapi.yml
- filename: propeller-aero-openapi.yml
  format: yaml
  label: Propeller Workspaces API
  slug: propeller-aero-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propeller-aero/refs/heads/main/openapi/propeller-aero-openapi.yml
- filename: propeller-aero-openapi.yml
  format: yaml
  label: Propeller Shapes & Widgets API
  slug: propeller-aero-shapes-widgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propeller-aero/refs/heads/main/openapi/propeller-aero-openapi.yml
- filename: propeller-aero-openapi.yml
  format: yaml
  label: Propeller Position Monitoring API
  slug: propeller-aero-position-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propeller-aero/refs/heads/main/openapi/propeller-aero-openapi.yml
consequence_counts:
  read: 16
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Propeller Aero Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'Propeller Aero exposes 17 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Propeller Aero
provider_slug: propeller-aero
slug: propeller-aero-agentic-access
source_filename: propeller-aero-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/propeller-aero-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    connected: 16\n    acting: 1\n  by_consequence:\n    read: 16\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /organizations\n  method: get\n  operationId: listOrganizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organization_id}\n  method: get\n  operationId: getOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organization_id}/sites\n\
  \  method: get\n  operationId: listSites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organization_id}/sites/{site_id}\n  method: get\n  operationId: getSite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organization_id}/sites/{site_id}/sample_elevation\n  method: get\n  operationId: sampleSiteElevation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organization_id}/sites/{site_id}/surveys\n  method: get\n  operationId: listSurveys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organization_id}/sites/{site_id}/surveys/{survey_id}\n\
  \  method: get\n  operationId: getSurvey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organization_id}/sites/{site_id}/surveys/{survey_id}/files\n  method: get\n  operationId: listSurveyFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organization_id}/sites/{site_id}/workspaces\n  method: get\n  operationId: listWorkspaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organization_id}/sites/{site_id}/workspaces/{workspace_id}\n  method: get\n  operationId: getWorkspace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /organizations/{organization_id}/sites/{site_id}/workspaces/{workspace_id}/shapes\n  method: get\n  operationId: listShapes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organization_id}/sites/{site_id}/workspaces/{workspace_id}/shapes/{shape_id}\n  method: get\n  operationId: getShape\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organization_id}/sites/{site_id}/workspaces/{workspace_id}/shapes/{shape_id}/widgets/{widget_id}/calculate\n  method: post\n  operationId: calculateWidget\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /position_monitoring_configs\n  method: get\n  operationId: listPositionMonitoringConfigs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /position_monitoring_configs/{id}\n  method: get\n  operationId: getPositionMonitoringConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /position_monitoring_epochs\n  method: get\n  operationId: listPositionMonitoringEpochs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /position_monitoring_epochs/{id}\n  method: get\n  operationId: getPositionMonitoringEpoch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/propeller-aero/refs/heads/main/agentic-access/propeller-aero-agentic-access.yml
summary_line: 17 operations · 1 acting
tags:
- Drone Survey
- Geospatial
- Earthworks
- Construction
- Mining
- Photogrammetry
- Surveying
- Analytics
---
