---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 4
api_specs:
- filename: cloud-storage-openapi.yml
  format: yaml
  label: Cloud Storage JSON API
  slug: cloud-storage-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-storage/refs/heads/main/openapi/cloud-storage-openapi.yml
consequence_counts:
  read: 4
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Google Cloud Storage Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'Google Cloud Storage exposes 10 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Google Cloud Storage
provider_slug: google-cloud-storage
slug: google-cloud-storage-agentic-access
source_filename: google-cloud-storage-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/cloud-storage-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 4\n    acting: 6\n  by_consequence:\n    read: 4\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /b\n  method: get\n  operationId: listBuckets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/devstorage.read_only\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /b\n  method: post\n  operationId: insertBucket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/devstorage.read_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /b/{bucket}\n  method: get\n  operationId: getBucket\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/devstorage.read_only\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /b/{bucket}\n  method: put\n  operationId: updateBucket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/devstorage.full_control\n    audience: null\n    token:\n      max-ttl: 900\n   \
  \ escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /b/{bucket}\n  method: delete\n  operationId: deleteBucket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/devstorage.full_control\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /b/{bucket}/o\n  method: get\n  operationId: listObjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/devstorage.read_only\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /b/{bucket}/o\n  method: post\n  operationId: insertObject\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/devstorage.read_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /b/{bucket}/o/{object}\n  method: get\n  operationId: getObject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/devstorage.read_only\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /b/{bucket}/o/{object}\n  method: put\n  operationId: updateObject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/devstorage.full_control\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /b/{bucket}/o/{object}\n  method: delete\n  operationId: deleteObject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/devstorage.full_control\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-storage/refs/heads/main/agentic-access/google-cloud-storage-agentic-access.yml
summary_line: 10 operations · 6 acting
tags:
- Buckets
- Cloud
- Google Cloud
- Objects
- Storage
---
