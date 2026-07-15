---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 17
api_specs:
- filename: openapi.json
  format: json
  label: Crystal Reports REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://api.sap.com/crystal/openapi.json
consequence_counts:
  read: 17
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Crystal Reports Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 20
overview: 'Crystal Reports exposes 20 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Crystal Reports
provider_slug: crystal-reports
slug: crystal-reports-agentic-access
source_filename: crystal-reports-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/crystal-reports-rest-api.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    connected: 17\n    acting: 3\n  by_consequence:\n    read: 17\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /logon/long\n  method: get\n  operationId: getLogonForm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /logon/long\n  method: post\n  operationId: logon\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /infostore\n  method: get\n  operationId: browseInfostore\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /infostore/Root%20Folder/children\n  method: get\n  operationId: listRootFolderContents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /infostore/{folderId}/children\n  method: get\n  operationId: listFolderContents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /infostore/{reportId}/rpt\n  method: get\n  operationId: getReportSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /infostore/{reportId}/rpt/structure\n  method: get\n  operationId: getReportStructure\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /infostore/{reportId}/rpt/instance\n  method: get\n  operationId: getInstanceForm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /infostore/{reportId}/rpt/instance\n  method: post\n  operationId: createReportInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /infostore/{reportId}/rpt/export\n  method: get\n  operationId: exportReport\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /infostore/{reportId}/rpt/data.svc\n  method: get\n  operationId: getODataServiceDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /infostore/{reportId}/rpt/data.svc/$metadata\n  method: get\n  operationId: getODataMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /infostore/{reportId}/rpt/data.svc/Rows\n  method: get\n  operationId: getReportDataRows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /infostore/{reportId}/rpt/data.svc/Rows\n  method: post\n  operationId: pushDataRow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /infostore/{reportId}/rpt/data.svc/Rows({index})\n  method: get\n  operationId: getReportDataRowByIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /infostore/{reportId}/rpt/data.svc/Rows({index})/{fieldName}\n  method: get\n  operationId: getRowFieldValue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /infostore/{reportId}/rpt/data.svc/Rows({index})/{fieldName}/$value\n  method: get\n  operationId: getRowFieldRawValue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /infostore/{reportId}/rpt/data.svc/GrandTotals\n\
  \  method: get\n  operationId: getGrandTotals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /infostore/{reportId}/rpt/data.svc/{GroupName}\n  method: get\n  operationId: getGroupData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /infostore/{reportId}/rpt/data.svc/{GroupName}('{groupPath}')\n  method: get\n  operationId: getGroupByPath\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/agentic-access/crystal-reports-agentic-access.yml
summary_line: 20 operations · 3 acting
tags:
- Business Intelligence
- Crystal Reports
- Data Analytics
- Enterprise Software
- Reporting
- SAP
---
