---
acting_count: 26
action_class_counts:
  acting: 26
  connected: 12
api_specs:
- filename: rest
  format: yaml
  label: Google Cloud Storage JSON API
  slug: google-cloud-storage-json-api
  spec_type: OpenAPI
  url: https://storage.googleapis.com/$discovery/rest?version=v1
consequence_counts:
  read: 12
  safety-critical: 13
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 13
kind: agentic-access
layout: agentic-access
method: generated
name: Gcp Cloud Storage Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /b/{bucket}/acl
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /b/{bucket}/acl/{entity}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /b/{bucket}/acl/{entity}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /b/{bucket}/acl/{entity}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /b/{bucket}/defaultObjectAcl
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /b/{bucket}/defaultObjectAcl/{entity}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /b/{bucket}/defaultObjectAcl/{entity}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /b/{bucket}/defaultObjectAcl/{entity}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /b/{bucket}/o/{object}/acl
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /b/{bucket}/o/{object}/acl/{entity}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /b/{bucket}/o/{object}/acl/{entity}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /b/{bucket}/o/{object}/acl/{entity}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /channels/stop
operation_count: 38
overview: 'Google Cloud Storage exposes 38 API operations that an AI agent could call, of which 26 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read, 13 write, and 13 safety-critical.


  13 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Google Cloud Storage
provider_slug: gcp-cloud-storage
slug: gcp-cloud-storage-agentic-access
source_filename: gcp-cloud-storage-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/gcp-cloud-storage-json-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 38\n  by_action_class:\n    connected: 12\n    acting: 26\n  by_consequence:\n    read: 12\n    write: 13\n    safety-critical: 13\n  human_in_the_loop_required: 13\noperations:\n- path: /b\n  method: get\n  operationId: listBuckets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /b\n  method: post\n  operationId: insertBucket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n   \
  \   human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /b/{bucket}\n  method: get\n  operationId: getBucket\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /b/{bucket}\n  method: put\n  operationId: updateBucket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /b/{bucket}\n  method: patch\n  operationId: patchBucket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /b/{bucket}\n  method: delete\n  operationId: deleteBucket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /b/{bucket}/lockRetentionPolicy\n  method: post\n  operationId: lockBucketRetentionPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /b/{bucket}/iam\n  method: get\n  operationId: getBucketIamPolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /b/{bucket}/iam\n  method: put\n  operationId: setBucketIamPolicy\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /b/{bucket}/iam/testPermissions\n  method: get\n  operationId: testBucketIamPermissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /b/{bucket}/o\n  method: get\n  operationId: listObjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /b/{bucket}/o/{object}\n  method: get\n  operationId: getObject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /b/{bucket}/o/{object}\n  method: put\n\
  \  operationId: updateObject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /b/{bucket}/o/{object}\n  method: patch\n  operationId: patchObject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /b/{bucket}/o/{object}\n  method: delete\n  operationId: deleteObject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n   \
  \ audit: required\n- path: /b/{bucket}/o/{object}/compose\n  method: post\n  operationId: composeObject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /b/{bucket}/o/{object}/copyTo/b/{destinationBucket}/o/{destinationObject}\n  method: post\n  operationId: copyObject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /b/{bucket}/o/{object}/rewriteTo/b/{destinationBucket}/o/{destinationObject}\n  method: post\n  operationId: rewriteObject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /b/{bucket}/o/watchAll\n  method: post\n  operationId: watchAllObjects\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /b/{bucket}/acl\n  method: get\n  operationId: listBucketAccessControls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /b/{bucket}/acl\n  method: post\n  operationId: insertBucketAccessControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n \
  \     max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /b/{bucket}/acl/{entity}\n  method: get\n  operationId: getBucketAccessControl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /b/{bucket}/acl/{entity}\n  method: put\n  operationId: updateBucketAccessControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /b/{bucket}/acl/{entity}\n  method: patch\n  operationId: patchBucketAccessControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /b/{bucket}/acl/{entity}\n  method: delete\n  operationId: deleteBucketAccessControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /b/{bucket}/defaultObjectAcl\n  method: get\n  operationId: listDefaultObjectAccessControls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /b/{bucket}/defaultObjectAcl\n  method: post\n  operationId: insertDefaultObjectAccessControl\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /b/{bucket}/defaultObjectAcl/{entity}\n  method: get\n  operationId: getDefaultObjectAccessControl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /b/{bucket}/defaultObjectAcl/{entity}\n  method: put\n  operationId: updateDefaultObjectAccessControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /b/{bucket}/defaultObjectAcl/{entity}\n\
  \  method: patch\n  operationId: patchDefaultObjectAccessControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /b/{bucket}/defaultObjectAcl/{entity}\n  method: delete\n  operationId: deleteDefaultObjectAccessControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /b/{bucket}/o/{object}/acl\n  method: get\n  operationId: listObjectAccessControls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n   \
  \ token:\n      max-ttl: 3600\n    audit: none\n- path: /b/{bucket}/o/{object}/acl\n  method: post\n  operationId: insertObjectAccessControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /b/{bucket}/o/{object}/acl/{entity}\n  method: get\n  operationId: getObjectAccessControl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /b/{bucket}/o/{object}/acl/{entity}\n  method: put\n  operationId: updateObjectAccessControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /b/{bucket}/o/{object}/acl/{entity}\n  method: patch\n  operationId: patchObjectAccessControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /b/{bucket}/o/{object}/acl/{entity}\n  method: delete\n  operationId: deleteObjectAccessControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /channels/stop\n  method: post\n  operationId:\
  \ stopChannel\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gcp-cloud-storage/refs/heads/main/agentic-access/gcp-cloud-storage-agentic-access.yml
summary_line: 38 operations · 26 acting · 13 human-in-the-loop
tags:
- Archival
- Backup
- Blob Storage
- Cloud Storage
- Data
- File Storage
- Google Cloud
- Object Storage
- Storage
---
