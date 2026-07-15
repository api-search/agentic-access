---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 4
api_specs:
- filename: google-sheets-openapi.yml
  format: yaml
  label: Google Sheets API v4
  slug: google-sheets-api-v4
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/openapi/google-sheets-openapi.yml
consequence_counts:
  read: 4
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Google Sheets Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'Google Sheets exposes 17 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 13 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Google Sheets
provider_slug: google-sheets
slug: google-sheets-agentic-access
source_filename: google-sheets-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/google-sheets-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    acting: 13\n    connected: 4\n  by_consequence:\n    write: 13\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /spreadsheets\n  method: post\n  operationId: createSpreadsheet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spreadsheets/{spreadsheetId}\n  method: get\n  operationId: getSpreadsheet\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spreadsheets/{spreadsheetId}:batchUpdate\n  method: post\n  operationId: batchUpdateSpreadsheet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spreadsheets/{spreadsheetId}:getByDataFilter\n  method: post\n  operationId: getSpreadsheetByDataFilter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spreadsheets/{spreadsheetId}/values/{range}\n  method: get\n  operationId: getValues\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spreadsheets/{spreadsheetId}/values/{range}\n  method: put\n  operationId: updateValues\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spreadsheets/{spreadsheetId}/values/{range}:append\n  method: post\n  operationId: appendValues\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spreadsheets/{spreadsheetId}/values/{range}:clear\n  method: post\n  operationId: clearValues\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spreadsheets/{spreadsheetId}/values:batchGet\n  method: get\n  operationId: batchGetValues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spreadsheets/{spreadsheetId}/values:batchUpdate\n  method: post\n  operationId: batchUpdateValues\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spreadsheets/{spreadsheetId}/values:batchClear\n  method: post\n  operationId: batchClearValues\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spreadsheets/{spreadsheetId}/values:batchGetByDataFilter\n  method: post\n  operationId: batchGetValuesByDataFilter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spreadsheets/{spreadsheetId}/values:batchUpdateByDataFilter\n  method: post\n  operationId: batchUpdateValuesByDataFilter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /spreadsheets/{spreadsheetId}/values:batchClearByDataFilter\n  method: post\n  operationId: batchClearValuesByDataFilter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spreadsheets/{spreadsheetId}/sheets/{sheetId}:copyTo\n  method: post\n  operationId: copySheet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spreadsheets/{spreadsheetId}/developerMetadata/{metadataId}\n  method: get\n  operationId: getDeveloperMetadata\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spreadsheets/{spreadsheetId}/developerMetadata:search\n  method: post\n  operationId: searchDeveloperMetadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/agentic-access/google-sheets-agentic-access.yml
summary_line: 17 operations · 13 acting
tags:
- Google Workspace
- Productivity
- Spreadsheets
---
