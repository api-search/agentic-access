---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 5
api_specs:
- filename: cloudimage-openapi.yml
  format: yaml
  label: Cloudimage Image Transformation (URL API)
  slug: cloudimage-image-transformation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudimage/refs/heads/main/openapi/cloudimage-openapi.yml
- filename: cloudimage-openapi.yml
  format: yaml
  label: Cloudimage Optimization & CDN API
  slug: cloudimage-optimization-cdn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudimage/refs/heads/main/openapi/cloudimage-openapi.yml
- filename: cloudimage-openapi.yml
  format: yaml
  label: Cloudimage Video Transformation (URL API)
  slug: cloudimage-video-transformation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudimage/refs/heads/main/openapi/cloudimage-openapi.yml
- filename: cloudimage-openapi.yml
  format: yaml
  label: Filerobot DAM Upload & Asset API
  slug: filerobot-dam-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudimage/refs/heads/main/openapi/cloudimage-openapi.yml
consequence_counts:
  read: 5
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cloudimage Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'Cloudimage exposes 9 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cloudimage
provider_slug: cloudimage
slug: cloudimage-agentic-access
source_filename: cloudimage-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/cloudimage-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 5\n    acting: 4\n  by_consequence:\n    read: 5\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /{origin}\n  method: get\n  operationId: transformImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{origin}.mp4\n  method: get\n  operationId: transformVideo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /upload\n  method: post\n  operationId:\
  \ uploadFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files\n  method: get\n  operationId: listFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files\n  method: put\n  operationId: streamUploadFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files/{uuid}\n  method: get\n  operationId: getFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /files/{uuid}\n  method: delete\n  operationId: deleteFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /folders\n  method: get\n  operationId: listFolders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /folders\n  method: post\n  operationId: createFolder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudimage/refs/heads/main/agentic-access/cloudimage-agentic-access.yml
summary_line: 9 operations · 4 acting
tags:
- Image Optimization
- Image CDN
- Resizing
- Transformation
- DAM
---
