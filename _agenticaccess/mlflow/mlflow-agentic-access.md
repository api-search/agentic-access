---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 9
api_specs:
- filename: mlflow-artifacts-api-openapi.yml
  format: yaml
  label: MLflow Artifacts API
  slug: mlflow-artifacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mlflow/refs/heads/main/openapi/mlflow-artifacts-api-openapi.yml
- filename: mlflow-experiments-api-openapi.yml
  format: yaml
  label: MLflow Experiments API
  slug: mlflow-experiments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mlflow/refs/heads/main/openapi/mlflow-experiments-api-openapi.yml
- filename: mlflow-metrics-api-openapi.yml
  format: yaml
  label: MLflow Metrics API
  slug: mlflow-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mlflow/refs/heads/main/openapi/mlflow-metrics-api-openapi.yml
- filename: mlflow-model-versions-api-openapi.yml
  format: yaml
  label: MLflow Model Versions API
  slug: mlflow-model-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mlflow/refs/heads/main/openapi/mlflow-model-versions-api-openapi.yml
- filename: mlflow-registered-models-api-openapi.yml
  format: yaml
  label: MLflow Registered Models API
  slug: mlflow-registered-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mlflow/refs/heads/main/openapi/mlflow-registered-models-api-openapi.yml
- filename: mlflow-runs-api-openapi.yml
  format: yaml
  label: MLflow Runs API
  slug: mlflow-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mlflow/refs/heads/main/openapi/mlflow-runs-api-openapi.yml
consequence_counts:
  read: 9
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Mlflow Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 23
overview: 'MLflow exposes 23 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 14 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: MLflow
provider_slug: mlflow
slug: mlflow-agentic-access
source_filename: mlflow-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/mlflow-artifacts-api-openapi.yml, openapi/mlflow-experiments-api-openapi.yml,\n  openapi/mlflow-metrics-api-openapi.yml, openapi/mlflow-model-versions-api-openapi.yml, openapi/mlflow-registered-models-api-openapi.yml,\n  openapi/mlflow-runs-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 9\n    acting: 14\n  by_consequence:\n    read: 9\n    write: 14\n  human_in_the_loop_required: 0\noperations:\n- path: /api/2.0/mlflow/artifacts/list\n  method: get\n  operationId: listArtifacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/2.0/mlflow/artifacts/presigned-upload-url\n  method: post\n  operationId: presignedUploadUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/2.0/mlflow/experiments/create\n  method: post\n  operationId: createExperiment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/2.0/mlflow/experiments/search\n  method: post\n  operationId: searchExperiments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/2.0/mlflow/experiments/get\n\
  \  method: get\n  operationId: getExperiment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/2.0/mlflow/experiments/get-by-name\n  method: get\n  operationId: getExperimentByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/2.0/mlflow/experiments/delete\n  method: post\n  operationId: deleteExperiment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/2.0/mlflow/experiments/restore\n  method: post\n  operationId: restoreExperiment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n  \
  \  audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/2.0/mlflow/experiments/update\n  method: post\n  operationId: updateExperiment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/2.0/mlflow/runs/log-metric\n  method: post\n  operationId: logMetric\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/2.0/mlflow/runs/log-parameter\n  method: post\n  operationId: logParameter\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/2.0/mlflow/runs/log-batch\n  method: post\n  operationId: logBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/2.0/mlflow/metrics/get-history\n  method: get\n  operationId: getMetricHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/2.0/mlflow/model-versions/create\n  method: post\n  operationId: createModelVersion\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/2.0/mlflow/registered-models/create\n  method: post\n  operationId: createRegisteredModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/2.0/mlflow/registered-models/get\n  method: get\n  operationId: getRegisteredModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/2.0/mlflow/registered-models/search\n  method: post\n  operationId: searchRegisteredModels\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/2.0/mlflow/runs/create\n  method: post\n  operationId: createRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/2.0/mlflow/runs/update\n  method: post\n  operationId: updateRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/2.0/mlflow/runs/get\n  method: get\n  operationId: getRun\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/2.0/mlflow/runs/search\n  method: post\n  operationId: searchRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/2.0/mlflow/runs/delete\n  method: post\n  operationId: deleteRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/2.0/mlflow/runs/restore\n  method: post\n  operationId: restoreRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mlflow/refs/heads/main/agentic-access/mlflow-agentic-access.yml
summary_line: 23 operations · 14 acting
tags:
- Machine Learning
- MLOps
- Generative AI
- Experiment Tracking
- Open Source
---
