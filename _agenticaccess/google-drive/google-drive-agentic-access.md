---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 3
api_specs:
- filename: google-drive-files-api-openapi.yml
  format: yaml
  label: Google Drive Files API
  slug: google-drive-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-drive/openapi/google-drive-files-api-openapi.yml
- filename: google-drive-about-api-openapi.yml
  format: yaml
  label: Google Drive About API
  slug: google-drive-about-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-drive/openapi/google-drive-about-api-openapi.yml
- filename: google-drive-accessproposals-api-openapi.yml
  format: yaml
  label: Google Drive Accessproposals API
  slug: google-drive-accessproposals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-drive/openapi/google-drive-accessproposals-api-openapi.yml
- filename: google-drive-approvals-api-openapi.yml
  format: yaml
  label: Google Drive Approvals API
  slug: google-drive-approvals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-drive/openapi/google-drive-approvals-api-openapi.yml
- filename: google-drive-apps-api-openapi.yml
  format: yaml
  label: Google Drive Apps API
  slug: google-drive-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-drive/openapi/google-drive-apps-api-openapi.yml
- filename: google-drive-changes-api-openapi.yml
  format: yaml
  label: Google Drive Changes API
  slug: google-drive-changes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-drive/openapi/google-drive-changes-api-openapi.yml
- filename: google-drive-channels-api-openapi.yml
  format: yaml
  label: Google Drive Channels API
  slug: google-drive-channels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-drive/openapi/google-drive-channels-api-openapi.yml
- filename: google-drive-comments-api-openapi.yml
  format: yaml
  label: Google Drive Comments API
  slug: google-drive-comments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-drive/openapi/google-drive-comments-api-openapi.yml
- filename: google-drive-drives-api-openapi.yml
  format: yaml
  label: Google Drive Drives API
  slug: google-drive-drives-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-drive/openapi/google-drive-drives-api-openapi.yml
- filename: google-drive-operations-api-openapi.yml
  format: yaml
  label: Google Drive Operations API
  slug: google-drive-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-drive/openapi/google-drive-operations-api-openapi.yml
- filename: google-drive-permissions-api-openapi.yml
  format: yaml
  label: Google Drive Permissions API
  slug: google-drive-permissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-drive/openapi/google-drive-permissions-api-openapi.yml
- filename: google-drive-replies-api-openapi.yml
  format: yaml
  label: Google Drive Replies API
  slug: google-drive-replies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-drive/openapi/google-drive-replies-api-openapi.yml
- filename: google-drive-revisions-api-openapi.yml
  format: yaml
  label: Google Drive Revisions API
  slug: google-drive-revisions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-drive/openapi/google-drive-revisions-api-openapi.yml
- filename: google-drive-teamdrives-api-openapi.yml
  format: yaml
  label: Google Drive Teamdrives API
  slug: google-drive-teamdrives-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-drive/openapi/google-drive-teamdrives-api-openapi.yml
consequence_counts:
  read: 3
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Google Drive Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Google Drive exposes 8 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Google Drive
provider_slug: google-drive
slug: google-drive-agentic-access
source_filename: google-drive-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/google-drive-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 3\n    acting: 5\n  by_consequence:\n    read: 3\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /files\n  method: get\n  operationId: listFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files\n  method: post\n  operationId: createFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /files/{fileId}\n  method: get\n  operationId: getFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/{fileId}\n  method: patch\n  operationId: updateFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files/{fileId}\n  method: delete\n  operationId: deleteFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files/{fileId}/copy\n  method:\
  \ post\n  operationId: copyFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files/{fileId}/permissions\n  method: get\n  operationId: listPermissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/{fileId}/permissions\n  method: post\n  operationId: createPermission\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/google-drive/agentic-access/google-drive-agentic-access.yml
summary_line: 8 operations · 5 acting
tags:
- Cloud Storage
- Collaboration
- Document Management
- Drives
- File
- Google
- Storage
---
