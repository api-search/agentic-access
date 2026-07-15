---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 15
api_specs:
- filename: google-cloud-dataflow-api-openapi.yml
  format: yaml
  label: Google Cloud Dataflow API
  slug: google-cloud-dataflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-dataflow/refs/heads/main/openapi/google-cloud-dataflow-api-openapi.yml
consequence_counts:
  physical: 1
  read: 15
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Google Cloud Dataflow Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1b3/projects/{projectId}/locations/{location}/jobs/{jobId}/debug/sendCapture
operation_count: 29
overview: 'Google Cloud Dataflow exposes 29 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read, 13 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Google Cloud Dataflow
provider_slug: google-cloud-dataflow
slug: google-cloud-dataflow-agentic-access
source_filename: google-cloud-dataflow-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/google-cloud-dataflow-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 29\n  by_action_class:\n    connected: 15\n    acting: 14\n  by_consequence:\n    read: 15\n    write: 13\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1b3/projects/{projectId}/jobs:aggregated\n  method: get\n  operationId: listAggregatedJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1b3/projects/{projectId}/jobs\n  method: get\n  operationId: listProjectJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /v1b3/projects/{projectId}/jobs\n  method: post\n  operationId: createProjectJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1b3/projects/{projectId}/jobs/{jobId}\n  method: get\n  operationId: getProjectJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1b3/projects/{projectId}/jobs/{jobId}\n  method: put\n  operationId: updateProjectJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1b3/projects/{projectId}/jobs/{jobId}:snapshot\n  method: post\n  operationId: snapshotProjectJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1b3/projects/{projectId}/jobs/{jobId}/metrics\n  method: get\n  operationId: getProjectJobMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1b3/projects/{projectId}/jobs/{jobId}/messages\n  method: get\n  operationId: listProjectJobMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1b3/projects/{projectId}/locations/{location}/jobs\n  method: get\n \
  \ operationId: listLocationJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1b3/projects/{projectId}/locations/{location}/jobs\n  method: post\n  operationId: createLocationJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1b3/projects/{projectId}/locations/{location}/jobs/{jobId}\n  method: get\n  operationId: getLocationJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1b3/projects/{projectId}/locations/{location}/jobs/{jobId}\n  method: put\n  operationId: updateLocationJob\n  x-agentic-access:\n    action-class: acting\n   \
  \ consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1b3/projects/{projectId}/locations/{location}/jobs/{jobId}:snapshot\n  method: post\n  operationId: snapshotLocationJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1b3/projects/{projectId}/locations/{location}/jobs/{jobId}/metrics\n  method: get\n  operationId: getLocationJobMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1b3/projects/{projectId}/locations/{location}/jobs/{jobId}/messages\n  method:\
  \ get\n  operationId: listLocationJobMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1b3/projects/{projectId}/locations/{location}/jobs/{jobId}/executionDetails\n  method: get\n  operationId: getLocationJobExecutionDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1b3/projects/{projectId}/locations/{location}/jobs/{jobId}/stages/{stageId}/executionDetails\n  method: get\n  operationId: getLocationJobStageExecutionDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1b3/projects/{projectId}/locations/{location}/snapshots/{snapshotId}\n  method: get\n  operationId: getLocationSnapshot\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1b3/projects/{projectId}/locations/{location}/snapshots/{snapshotId}\n  method: delete\n  operationId: deleteLocationSnapshot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1b3/projects/{projectId}/locations/{location}/snapshots\n  method: get\n  operationId: listLocationSnapshots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1b3/projects/{projectId}/locations/{location}/jobs/{jobId}/debug/getConfig\n  method: post\n  operationId: getLocationJobDebugConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1b3/projects/{projectId}/locations/{location}/jobs/{jobId}/debug/sendCapture\n  method: post\n  operationId: sendLocationJobDebugCapture\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1b3/projects/{projectId}/locations/{location}/flexTemplates:launch\n  method: post\n  operationId: launchLocationFlexTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1b3/projects/{projectId}/locations/{location}/templates\n  method: post\n  operationId: createLocationJobFromTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1b3/projects/{projectId}/locations/{location}/templates:get\n  method: get\n  operationId: getLocationTemplate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1b3/projects/{projectId}/locations/{location}/templates:launch\n  method: post\n  operationId: launchLocationTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1b3/projects/{projectId}/templates\n  method: post\n  operationId: createProjectJobFromTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1b3/projects/{projectId}/templates:get\n  method: get\n  operationId: getProjectTemplate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1b3/projects/{projectId}/templates:launch\n  method: post\n  operationId: launchProjectTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-dataflow/refs/heads/main/agentic-access/google-cloud-dataflow-agentic-access.yml
summary_line: 29 operations · 14 acting
tags:
- Apache Beam
- Batch Processing
- Big Data
- Data Processing
- ETL
- Stream Processing
---
