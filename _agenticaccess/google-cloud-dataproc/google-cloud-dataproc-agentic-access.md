---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 5
api_specs:
- filename: cloud-dataproc-openapi.yml
  format: yaml
  label: Cloud Dataproc API
  slug: cloud-dataproc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-dataproc/refs/heads/main/openapi/cloud-dataproc-openapi.yml
consequence_counts:
  read: 5
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Google Cloud Dataproc Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Google Cloud Dataproc exposes 12 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Google Cloud Dataproc
provider_slug: google-cloud-dataproc
slug: google-cloud-dataproc-agentic-access
source_filename: google-cloud-dataproc-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/cloud-dataproc-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 5\n    acting: 7\n  by_consequence:\n    read: 5\n    write: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /projects/{project}/regions/{region}/clusters\n  method: get\n  operationId: listClusters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project}/regions/{region}/clusters\n  method: post\n  operationId: createCluster\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project}/regions/{region}/clusters/{cluster}\n  method: get\n  operationId: getCluster\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project}/regions/{region}/clusters/{cluster}\n  method: patch\n  operationId: updateCluster\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project}/regions/{region}/clusters/{cluster}\n  method: delete\n  operationId: deleteCluster\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project}/regions/{region}/jobs\n  method: get\n  operationId: listJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project}/regions/{region}/jobs:submit\n  method: post\n  operationId: submitJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project}/regions/{region}/jobs/{jobId}\n  method: get\n  operationId: getJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project}/regions/{region}/jobs/{jobId}\n  method: delete\n  operationId: deleteJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /projects/{project}/regions/{region}/jobs/{jobId}:cancel\n  method: post\n  operationId: cancelJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project}/regions/{region}/workflowTemplates\n  method: get\n  operationId: listWorkflowTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project}/regions/{region}/workflowTemplates\n  method: post\n  operationId: createWorkflowTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-dataproc/refs/heads/main/agentic-access/google-cloud-dataproc-agentic-access.yml
summary_line: 12 operations · 7 acting
tags:
- Big Data
- Data Processing
- Google Cloud
- Hadoop
- Spark
---
