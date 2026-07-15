---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 8
api_specs:
- filename: tigris-data-openapi.yml
  format: yaml
  label: Tigris Object Storage (S3-Compatible) API
  slug: object-storage-s3-compatible-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tigris-data/refs/heads/main/openapi/tigris-data-openapi.yml
- filename: tigris-data-openapi.yml
  format: yaml
  label: Tigris Bucket Management API
  slug: bucket-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tigris-data/refs/heads/main/openapi/tigris-data-openapi.yml
- filename: tigris-data-openapi.yml
  format: yaml
  label: Tigris Multipart Upload API
  slug: multipart-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tigris-data/refs/heads/main/openapi/tigris-data-openapi.yml
- filename: tigris-data-openapi.yml
  format: yaml
  label: Tigris Presigned URLs API
  slug: presigned-urls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tigris-data/refs/heads/main/openapi/tigris-data-openapi.yml
- filename: tigris-data-openapi.yml
  format: yaml
  label: Tigris IAM and Access Keys API
  slug: iam-access-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tigris-data/refs/heads/main/openapi/tigris-data-openapi.yml
- filename: tigris-data-openapi.yml
  format: yaml
  label: Tigris Object Tiering API
  slug: object-tiering-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tigris-data/refs/heads/main/openapi/tigris-data-openapi.yml
consequence_counts:
  read: 8
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tigris Data Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 20
overview: 'Tigris exposes 20 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 12 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Tigris
provider_slug: tigris-data
slug: tigris-data-agentic-access
source_filename: tigris-data-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/tigris-data-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    connected: 8\n    acting: 12\n  by_consequence:\n    read: 8\n    write: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: listBuckets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{bucket}\n  method: put\n  operationId: createBucket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n   \
  \   triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{bucket}\n  method: get\n  operationId: listObjectsV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{bucket}\n  method: head\n  operationId: headBucket\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{bucket}\n  method: delete\n  operationId: deleteBucket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{bucket}/{key}\n  method: put\n  operationId: putObject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{bucket}/{key}\n  method: get\n  operationId: getObject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{bucket}/{key}\n  method: head\n  operationId: headObject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{bucket}/{key}\n  method: delete\n  operationId: deleteObject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{bucket}/{key}#tagging\n  method: put\n  operationId:\
  \ putObjectTagging\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{bucket}/{key}#tagging\n  method: get\n  operationId: getObjectTagging\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{bucket}/{key}#tagging\n  method: delete\n  operationId: deleteObjectTagging\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{bucket}#delete\n  method: post\n  operationId: deleteObjects\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{bucket}/{key}#restore\n  method: post\n  operationId: restoreObject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{bucket}/{key}#uploads\n  method: post\n  operationId: createMultipartUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{bucket}/{key}#partNumber\n  method: put\n\
  \  operationId: uploadPart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{bucket}/{key}#complete\n  method: post\n  operationId: completeMultipartUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{bucket}/{key}#complete\n  method: get\n  operationId: listParts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{bucket}/{key}#complete\n  method: delete\n  operationId: abortMultipartUpload\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{bucket}#uploads\n  method: get\n  operationId: listMultipartUploads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tigris-data/refs/heads/main/agentic-access/tigris-data-agentic-access.yml
summary_line: 20 operations · 12 acting
tags:
- Object Storage
- S3 Compatible
- Storage
- Multi-Cloud
- Globally Distributed
---
