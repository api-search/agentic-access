---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 9
api_specs:
- filename: amazon-lookout-for-vision-openapi-original.yaml
  format: yaml
  label: Amazon Lookout for Vision API
  slug: amazon-lookout-for-vision-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/openapi/amazon-lookout-for-vision-openapi-original.yaml
consequence_counts:
  read: 9
  safety-critical: 1
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Amazon Lookout For Vision Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /2020-11-20/projects/{projectName}/models/{modelVersion}/stop
operation_count: 22
overview: 'Amazon Lookout for Vision exposes 22 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 12 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amazon Lookout for Vision
provider_slug: amazon-lookout-for-vision
slug: amazon-lookout-for-vision-agentic-access
source_filename: amazon-lookout-for-vision-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/amazon-lookout-for-vision-openapi-original.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    acting: 13\n    connected: 9\n  by_consequence:\n    write: 12\n    read: 9\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /2020-11-20/projects/{projectName}/datasets\n  method: post\n  operationId: CreateDataset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2020-11-20/projects/{projectName}/models\n\
  \  method: post\n  operationId: CreateModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2020-11-20/projects/{projectName}/models\n  method: get\n  operationId: ListModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2020-11-20/projects\n  method: post\n  operationId: CreateProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2020-11-20/projects\n  method: get\n  operationId: ListProjects\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2020-11-20/projects/{projectName}/datasets/{datasetType}\n  method: delete\n  operationId: DeleteDataset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2020-11-20/projects/{projectName}/datasets/{datasetType}\n  method: get\n  operationId: DescribeDataset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2020-11-20/projects/{projectName}/models/{modelVersion}\n  method: delete\n  operationId: DeleteModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2020-11-20/projects/{projectName}/models/{modelVersion}\n  method: get\n  operationId: DescribeModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2020-11-20/projects/{projectName}\n  method: delete\n  operationId: DeleteProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2020-11-20/projects/{projectName}\n  method: get\n  operationId: DescribeProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /2020-11-20/projects/{projectName}/modelpackagingjobs/{jobName}\n  method: get\n  operationId: DescribeModelPackagingJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2020-11-20/projects/{projectName}/models/{modelVersion}/detect#Content-Type\n  method: post\n  operationId: DetectAnomalies\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2020-11-20/projects/{projectName}/datasets/{datasetType}/entries\n  method: get\n  operationId: ListDatasetEntries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2020-11-20/projects/{projectName}/datasets/{datasetType}/entries\n\
  \  method: patch\n  operationId: UpdateDatasetEntries\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2020-11-20/projects/{projectName}/modelpackagingjobs\n  method: get\n  operationId: ListModelPackagingJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2020-11-20/projects/{projectName}/modelpackagingjobs\n  method: post\n  operationId: StartModelPackagingJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2020-11-20/tags/{resourceArn}\n\
  \  method: get\n  operationId: ListTagsForResource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2020-11-20/tags/{resourceArn}\n  method: post\n  operationId: TagResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2020-11-20/projects/{projectName}/models/{modelVersion}/start\n  method: post\n  operationId: StartModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2020-11-20/projects/{projectName}/models/{modelVersion}/stop\n\
  \  method: post\n  operationId: StopModel\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /2020-11-20/tags/{resourceArn}#tagKeys\n  method: delete\n  operationId: UntagResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/agentic-access/amazon-lookout-for-vision-agentic-access.yml
summary_line: 22 operations · 13 acting · 1 human-in-the-loop
tags:
- Computer Vision
- Machine Learning
- Manufacturing
- Quality Inspection
- Anomaly Detection
---
