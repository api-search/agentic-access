---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 13
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Canva Connect API
  slug: canva-connect-api
  spec_type: OpenAPI
  url: https://www.canva.com/developers/docs/connect-api/openapi/
consequence_counts:
  read: 13
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Canva Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 22
overview: 'Canva exposes 22 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read and 9 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Canva
provider_slug: canva
slug: canva-agentic-access
source_filename: canva-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/canva-connect-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 13\n    acting: 9\n  by_consequence:\n    read: 13\n    write: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /designs\n  method: get\n  operationId: listDesigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - design:meta:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /designs\n  method: post\n  operationId: createDesign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - design:content:write\n    audience: null\n \
  \   token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /designs/{designId}\n  method: get\n  operationId: getDesign\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - design:meta:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/{assetId}\n  method: get\n  operationId: getAsset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - asset:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/{assetId}\n  method: delete\n  operationId: deleteAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - asset:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n \
  \     - high-value\n    audit: required\n- path: /asset-uploads\n  method: post\n  operationId: createAssetUploadJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - asset:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /asset-uploads/{jobId}\n  method: get\n  operationId: getAssetUploadJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - asset:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /folders/{folderId}\n  method: get\n  operationId: getFolder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - folder:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /folders/{folderId}/items\n  method: get\n  operationId: listFolderItems\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - folder:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /folders/{folderId}/items:move\n  method: post\n  operationId: moveFolderItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - folder:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /exports\n  method: post\n  operationId: createDesignExportJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - design:content:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /exports/{exportId}\n  method:\
  \ get\n  operationId: getDesignExportJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - design:content:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /comments\n  method: post\n  operationId: createComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - comment:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /comments/{commentId}/replies\n  method: post\n  operationId: createReply\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - comment:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /users/me\n  method: get\n  operationId: getUsersMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /brand-templates\n  method: get\n  operationId: listBrandTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - brandtemplate:meta:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /brand-templates/{brandTemplateId}\n  method: get\n  operationId: getBrandTemplate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - brandtemplate:meta:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /brand-templates/{brandTemplateId}/dataset\n  method: get\n  operationId: getBrandTemplateDataset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - brandtemplate:content:read\n   \
  \ token:\n      max-ttl: 3600\n    audit: none\n- path: /autofills\n  method: post\n  operationId: createDesignAutofillJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - design:content:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /autofills/{jobId}\n  method: get\n  operationId: getDesignAutofillJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - design:content:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resizes\n  method: post\n  operationId: createDesignResizeJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - design:content:read\n    - design:content:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /resizes/{jobId}\n  method: get\n  operationId: getDesignResizeJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - design:content:read\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/agentic-access/canva-agentic-access.yml
summary_line: 22 operations · 9 acting
tags:
- Apps
- Automation
- Brand Management
- Collaboration
- Design
- Graphics
- Marketing
- Print
- Templates
- Visual Content
---
