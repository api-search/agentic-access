---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 8
api_specs:
- filename: acrcloud-openapi.yml
  format: yaml
  label: ACRCloud Identification API
  slug: identification
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acrcloud/refs/heads/main/openapi/acrcloud-openapi.yml
- filename: acrcloud-openapi.yml
  format: yaml
  label: ACRCloud File Scanning API
  slug: file-scanning
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acrcloud/refs/heads/main/openapi/acrcloud-openapi.yml
- filename: acrcloud-openapi.yml
  format: yaml
  label: ACRCloud Broadcast Monitoring API
  slug: broadcast-monitoring
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acrcloud/refs/heads/main/openapi/acrcloud-openapi.yml
- filename: acrcloud-openapi.yml
  format: yaml
  label: ACRCloud Buckets & Metadata API
  slug: buckets-metadata
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acrcloud/refs/heads/main/openapi/acrcloud-openapi.yml
- filename: acrcloud-openapi.yml
  format: yaml
  label: ACRCloud Console API
  slug: console
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acrcloud/refs/heads/main/openapi/acrcloud-openapi.yml
consequence_counts:
  read: 8
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Acrcloud Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 21
overview: 'ACRCloud exposes 21 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 13 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ACRCloud
provider_slug: acrcloud
slug: acrcloud-agentic-access
source_filename: acrcloud-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/acrcloud-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    acting: 13\n    connected: 8\n  by_consequence:\n    write: 13\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/identify\n  method: post\n  operationId: identify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/buckets\n  method: get\n  operationId: listBuckets\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/buckets\n  method: post\n  operationId: createBucket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/buckets/{id}\n  method: get\n  operationId: getBucket\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/buckets/{id}\n  method: put\n  operationId: updateBucket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/buckets/{id}\n\
  \  method: delete\n  operationId: deleteBucket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/buckets/{bucket_id}/files\n  method: get\n  operationId: listAudioFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/buckets/{bucket_id}/files\n  method: post\n  operationId: uploadAudioFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/buckets/{bucket_id}/files/{ids}\n  method: get\n  operationId: getAudioFiles\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/buckets/{bucket_id}/files/{ids}\n  method: delete\n  operationId: deleteAudioFiles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/fs-containers\n  method: get\n  operationId: listFileScanningContainers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/fs-containers\n  method: post\n  operationId: createFileScanningContainer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/fs-containers/{container_id}\n  method: get\n  operationId: getFileScanningContainer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/fs-containers/{container_id}\n  method: put\n  operationId: updateFileScanningContainer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/fs-containers/{container_id}\n  method: delete\n  operationId: deleteFileScanningContainer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/bm-bd-projects\n  method: get\n  operationId: listBroadcastProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/bm-bd-projects\n  method: post\n  operationId: createBroadcastProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/bm-bd-projects/{id}\n  method: put\n  operationId: updateBroadcastProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/bm-bd-projects/{id}\n  method: delete\n  operationId: deleteBroadcastProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/bm-bd-projects/{id}/result-callback\n  method: post\n  operationId: setResultCallback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/external-metadata/tracks\n  method: get\n  operationId: getExternalMetadataTracks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acrcloud/refs/heads/main/agentic-access/acrcloud-agentic-access.yml
summary_line: 21 operations · 13 acting
tags:
- Audio
- Music Recognition
- Audio Fingerprinting
- Broadcast Monitoring
- Metadata
---
