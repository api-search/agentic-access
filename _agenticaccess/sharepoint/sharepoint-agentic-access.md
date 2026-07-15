---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 10
api_specs:
- filename: sharepoint-rest-openapi.json
  format: json
  label: SharePoint REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://example.com/sharepoint-rest-openapi.json
- filename: graph-sharepoint-openapi.json
  format: json
  label: Microsoft Graph API (SharePoint)
  slug: graph-api-sharepoint
  spec_type: OpenAPI
  url: https://example.com/graph-sharepoint-openapi.json
consequence_counts:
  read: 10
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sharepoint Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'Microsoft SharePoint exposes 15 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Microsoft SharePoint
provider_slug: sharepoint
slug: sharepoint-agentic-access
source_filename: sharepoint-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/sharepoint-rest-api.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 10\n    acting: 5\n  by_consequence:\n    read: 10\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /web\n  method: get\n  operationId: getWeb\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /web/title\n  method: get\n  operationId: getWebTitle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /web/lists\n  method: get\n  operationId: getLists\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /web/lists\n  method: post\n  operationId: createList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /web/lists/getbytitle('{list_title}')\n  method: get\n  operationId: getListByTitle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /web/lists/getbytitle('{list_title}')/items\n  method: get\n  operationId: getListItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /web/lists/getbytitle('{list_title}')/items\n\
  \  method: post\n  operationId: createListItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /web/lists/getbytitle('{list_title}')/items({item_id})\n  method: get\n  operationId: getListItemById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /web/lists/getbytitle('{list_title}')/items({item_id})\n  method: post\n  operationId: updateListItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /web/lists/getbytitle('{list_title}')/items({item_id})\n\
  \  method: delete\n  operationId: deleteListItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /web/getfolderbyserverrelativeurl('{folder_url}')/files\n  method: get\n  operationId: getFilesInFolder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /web/getfolderbyserverrelativeurl('{folder_url}')/files/add(url='{file_name}',overwrite=true)\n  method: post\n  operationId: uploadFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /web/getfilebyserverrelativeurl('{file_url}')/$value\n  method: get\n  operationId: downloadFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/query\n  method: get\n  operationId: searchQuery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /SP.UserProfiles.PeopleManager/GetMyProperties\n  method: get\n  operationId: getMyUserProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sharepoint/refs/heads/main/agentic-access/sharepoint-agentic-access.yml
summary_line: 15 operations · 5 acting
tags:
- Collaboration
- Document Management
- Enterprise Content Management
- Intranet
- Microsoft
---
