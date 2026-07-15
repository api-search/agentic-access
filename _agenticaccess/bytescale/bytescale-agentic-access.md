---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 2
api_specs:
- filename: bytescale-openapi.yml
  format: yaml
  label: Bytescale File Upload API
  slug: bytescale-file-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytescale/refs/heads/main/openapi/bytescale-openapi.yml
- filename: bytescale-openapi.yml
  format: yaml
  label: Bytescale Files Management API
  slug: bytescale-files-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytescale/refs/heads/main/openapi/bytescale-openapi.yml
- filename: bytescale-openapi.yml
  format: yaml
  label: Bytescale Image / Video Processing API
  slug: bytescale-image-video-processing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytescale/refs/heads/main/openapi/bytescale-openapi.yml
- filename: bytescale-openapi.yml
  format: yaml
  label: Bytescale CDN / Serving API
  slug: bytescale-cdn-serving-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytescale/refs/heads/main/openapi/bytescale-openapi.yml
consequence_counts:
  read: 2
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bytescale Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'Bytescale exposes 9 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bytescale
provider_slug: bytescale
slug: bytescale-agentic-access
source_filename: bytescale-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/bytescale-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    acting: 7\n    connected: 2\n  by_consequence:\n    write: 7\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/accounts/{accountId}/uploads/binary\n  method: post\n  operationId: basicUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{accountId}/uploads/form_data\n  method: post\n  operationId: formDataUpload\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{accountId}/uploads/url\n  method: post\n  operationId: uploadFromUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{accountId}/files/details\n  method: get\n  operationId: getFileDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{accountId}/files\n  method: delete\n  operationId: deleteFile\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{accountId}/files/copy\n  method: post\n  operationId: copyFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{accountId}/folders/list\n  method: get\n  operationId: listFolder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{accountId}/folders\n  method: put\n  operationId: putFolder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{accountId}/folders\n  method: delete\n  operationId: deleteFolder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bytescale/refs/heads/main/agentic-access/bytescale-agentic-access.yml
summary_line: 9 operations · 7 acting
tags:
- File Upload
- Storage
- Image Processing
- CDN
- Media
---
