---
acting_count: 21
action_class_counts:
  acting: 21
  connected: 13
api_specs:
- filename: teable-openapi.yml
  format: yaml
  label: Teable Spaces API
  slug: teable-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teable/refs/heads/main/openapi/teable-openapi.yml
- filename: teable-openapi.yml
  format: yaml
  label: Teable Bases API
  slug: teable-bases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teable/refs/heads/main/openapi/teable-openapi.yml
- filename: teable-openapi.yml
  format: yaml
  label: Teable Tables API
  slug: teable-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teable/refs/heads/main/openapi/teable-openapi.yml
- filename: teable-openapi.yml
  format: yaml
  label: Teable Fields API
  slug: teable-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teable/refs/heads/main/openapi/teable-openapi.yml
- filename: teable-openapi.yml
  format: yaml
  label: Teable Records API
  slug: teable-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teable/refs/heads/main/openapi/teable-openapi.yml
- filename: teable-openapi.yml
  format: yaml
  label: Teable Views API
  slug: teable-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teable/refs/heads/main/openapi/teable-openapi.yml
- filename: teable-openapi.yml
  format: yaml
  label: Teable Attachments API
  slug: teable-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teable/refs/heads/main/openapi/teable-openapi.yml
consequence_counts:
  read: 13
  write: 21
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Teable Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 34
overview: 'Teable exposes 34 API operations that an AI agent could call, of which 21 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read and 21 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Teable
provider_slug: teable
slug: teable-agentic-access
source_filename: teable-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/teable-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 34\n  by_action_class:\n    connected: 13\n    acting: 21\n  by_consequence:\n    read: 13\n    write: 21\n  human_in_the_loop_required: 0\noperations:\n- path: /spaces\n  method: get\n  operationId: getSpaceList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spaces\n  method: post\n  operationId: createSpace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n \
  \     triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spaces/{spaceId}\n  method: get\n  operationId: getSpace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spaces/{spaceId}\n  method: patch\n  operationId: updateSpace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spaces/{spaceId}\n  method: delete\n  operationId: deleteSpace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spaces/{spaceId}/collaborators\n\
  \  method: get\n  operationId: listSpaceCollaborators\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bases\n  method: get\n  operationId: getBaseList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bases\n  method: post\n  operationId: createBase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bases/{baseId}\n  method: get\n  operationId: getBase\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bases/{baseId}\n  method: patch\n  operationId:\
  \ updateBase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bases/{baseId}\n  method: delete\n  operationId: deleteBase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bases/{baseId}/duplicate\n  method: post\n  operationId: duplicateBase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /base/{baseId}/table\n  method: get\n  operationId: getTableList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /base/{baseId}/table\n  method: post\n  operationId: createTable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /base/{baseId}/table/{tableId}\n  method: get\n  operationId: getTable\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /base/{baseId}/table/{tableId}\n  method: delete\n  operationId: deleteTable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /table/{tableId}/field\n  method: get\n  operationId: getFieldList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /table/{tableId}/field\n  method: post\n  operationId: createField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /table/{tableId}/field/{fieldId}\n  method: get\n  operationId: getField\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /table/{tableId}/field/{fieldId}\n  method:\
  \ patch\n  operationId: updateField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /table/{tableId}/field/{fieldId}\n  method: delete\n  operationId: deleteField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /table/{tableId}/field/{fieldId}/convert\n  method: put\n  operationId: convertField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /table/{tableId}/record\n  method: get\n  operationId: getRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /table/{tableId}/record\n  method: post\n  operationId: createRecords\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /table/{tableId}/record\n  method: delete\n  operationId: deleteRecords\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /table/{tableId}/record/{recordId}\n\
  \  method: get\n  operationId: getRecord\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /table/{tableId}/record/{recordId}\n  method: patch\n  operationId: updateRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /table/{tableId}/record/{recordId}\n  method: delete\n  operationId: deleteRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /table/{tableId}/view\n  method: get\n  operationId: getViewList\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /table/{tableId}/view\n  method: post\n  operationId: createView\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /table/{tableId}/view/{viewId}\n  method: get\n  operationId: getView\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /table/{tableId}/view/{viewId}\n  method: delete\n  operationId: deleteView\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /attachments/signature\n  method: post\n  operationId: getAttachmentSignature\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /attachments/notify/{token}\n  method: post\n  operationId: notifyAttachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teable/refs/heads/main/agentic-access/teable-agentic-access.yml
summary_line: 34 operations · 21 acting
tags:
- No-Code
- Database
- Airtable Alternative
- Postgres
- Open Source
---
