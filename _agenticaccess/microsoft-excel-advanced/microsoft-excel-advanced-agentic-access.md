---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 9
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Microsoft Graph Excel API
  slug: microsoft-graph-excel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/msgraph-metadata/master/openapi/v1.0/openapi.yaml
consequence_counts:
  read: 9
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Microsoft Excel Advanced Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 22
overview: 'Microsoft Excel (Advanced) exposes 22 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 13 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Microsoft Excel (Advanced)
provider_slug: microsoft-excel-advanced
slug: microsoft-excel-advanced-agentic-access
source_filename: microsoft-excel-advanced-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/microsoft-excel-advanced-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    acting: 13\n    connected: 9\n  by_consequence:\n    write: 13\n    read: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /me/drive/items/{item-id}/workbook/createSession\n  method: post\n  operationId: workbook_createSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - Files.ReadWrite\n- path: /me/drive/items/{item-id}/workbook/closeSession\n\
  \  method: post\n  operationId: workbook_closeSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - Files.ReadWrite\n- path: /me/drive/items/{item-id}/workbook/worksheets\n  method: get\n  operationId: worksheets_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - Files.ReadWrite\n- path: /me/drive/items/{item-id}/workbook/worksheets\n  method: post\n  operationId: worksheets_add\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n    scope:\n    - Files.ReadWrite\n- path: /me/drive/items/{item-id}/workbook/worksheets/{worksheet-id}\n  method: get\n  operationId: worksheets_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - Files.ReadWrite\n- path: /me/drive/items/{item-id}/workbook/worksheets/{worksheet-id}\n  method: patch\n  operationId: worksheets_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - Files.ReadWrite\n- path: /me/drive/items/{item-id}/workbook/worksheets/{worksheet-id}\n  method: delete\n  operationId: worksheets_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - Files.ReadWrite\n- path: /me/drive/items/{item-id}/workbook/worksheets/{worksheet-id}/range(address='{address}')\n  method: get\n  operationId: range_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - Files.ReadWrite\n- path: /me/drive/items/{item-id}/workbook/worksheets/{worksheet-id}/range(address='{address}')\n  method: patch\n  operationId: range_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - Files.ReadWrite\n- path:\
  \ /me/drive/items/{item-id}/workbook/worksheets/{worksheet-id}/tables\n  method: get\n  operationId: tables_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - Files.ReadWrite\n- path: /me/drive/items/{item-id}/workbook/tables/add\n  method: post\n  operationId: tables_add\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - Files.ReadWrite\n- path: /me/drive/items/{item-id}/workbook/tables/{table-id}\n  method: get\n  operationId: tables_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - Files.ReadWrite\n- path: /me/drive/items/{item-id}/workbook/tables/{table-id}\n\
  \  method: patch\n  operationId: tables_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - Files.ReadWrite\n- path: /me/drive/items/{item-id}/workbook/tables/{table-id}\n  method: delete\n  operationId: tables_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - Files.ReadWrite\n- path: /me/drive/items/{item-id}/workbook/tables/{table-id}/rows\n  method: get\n  operationId: tableRows_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n    scope:\n    - Files.ReadWrite\n- path: /me/drive/items/{item-id}/workbook/tables/{table-id}/rows\n  method: post\n  operationId: tableRows_add\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - Files.ReadWrite\n- path: /me/drive/items/{item-id}/workbook/tables/{table-id}/columns\n  method: get\n  operationId: tableColumns_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - Files.ReadWrite\n- path: /me/drive/items/{item-id}/workbook/tables/{table-id}/columns\n  method: post\n  operationId: tableColumns_add\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - Files.ReadWrite\n- path: /me/drive/items/{item-id}/workbook/worksheets/{worksheet-id}/charts\n  method: get\n  operationId: charts_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - Files.ReadWrite\n- path: /me/drive/items/{item-id}/workbook/worksheets/{worksheet-id}/charts/add\n  method: post\n  operationId: charts_add\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - Files.ReadWrite\n- path: /me/drive/items/{item-id}/workbook/names\n\
  \  method: get\n  operationId: namedItems_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - Files.ReadWrite\n- path: /me/drive/items/{item-id}/workbook/functions/{function-name}\n  method: post\n  operationId: functions_invoke\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - Files.ReadWrite\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-excel-advanced/refs/heads/main/agentic-access/microsoft-excel-advanced-agentic-access.yml
summary_line: 22 operations · 13 acting
tags:
- Automation
- Business Intelligence
- Data Analysis
- Office
- Spreadsheets
---
