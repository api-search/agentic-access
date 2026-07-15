---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 2
api_specs:
- filename: instantdb-openapi.yml
  format: yaml
  label: InstantDB Admin HTTP API
  slug: instantdb-admin-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instantdb/refs/heads/main/openapi/instantdb-openapi.yml
- filename: instantdb-openapi.yml
  format: yaml
  label: InstantDB Query (InstaQL) API
  slug: instantdb-query-instaql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instantdb/refs/heads/main/openapi/instantdb-openapi.yml
- filename: instantdb-openapi.yml
  format: yaml
  label: InstantDB Transactions (InstaML) API
  slug: instantdb-transactions-instaml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instantdb/refs/heads/main/openapi/instantdb-openapi.yml
- filename: instantdb-openapi.yml
  format: yaml
  label: InstantDB Auth API
  slug: instantdb-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instantdb/refs/heads/main/openapi/instantdb-openapi.yml
- filename: instantdb-openapi.yml
  format: yaml
  label: InstantDB Storage API
  slug: instantdb-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instantdb/refs/heads/main/openapi/instantdb-openapi.yml
- filename: instantdb-asyncapi.yml
  format: yaml
  label: InstantDB Realtime Sync API
  slug: instantdb-realtime-sync-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/instantdb/refs/heads/main/asyncapi/instantdb-asyncapi.yml
consequence_counts:
  physical: 1
  read: 2
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Instantdb Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/send_magic_code
operation_count: 14
overview: 'InstantDB exposes 14 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read, 11 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: InstantDB
provider_slug: instantdb
slug: instantdb-agentic-access
source_filename: instantdb-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/instantdb-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    acting: 12\n    connected: 2\n  by_consequence:\n    write: 11\n    physical: 1\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /admin/query\n  method: post\n  operationId: adminQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/transact\n  method: post\n  operationId: adminTransact\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/refresh_tokens\n  method: post\n  operationId: adminRefreshTokens\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/magic_code\n  method: post\n  operationId: adminCreateMagicCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/send_magic_code\n  method: post\n  operationId:\
  \ adminSendMagicCode\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/verify_magic_code\n  method: post\n  operationId: adminVerifyMagicCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/users\n  method: get\n  operationId: adminGetUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/users\n  method: delete\n  operationId: adminDeleteUser\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/sign_out\n  method: post\n  operationId: adminSignOut\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /runtime/auth/verify_refresh_token\n  method: post\n  operationId: verifyRefreshToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /admin/storage/upload\n  method: put\n  operationId: adminStorageUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/storage/files\n  method: delete\n  operationId: adminStorageDeleteFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/storage/files/delete\n  method: post\n  operationId: adminStorageDeleteFiles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/rooms/presence\n  method: get\n  operationId: adminRoomPresence\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instantdb/refs/heads/main/agentic-access/instantdb-agentic-access.yml
summary_line: 14 operations · 12 acting
tags:
- Database
- Realtime
- Sync
- Backend
- Local First
---
