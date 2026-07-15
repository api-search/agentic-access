---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 20
api_specs:
- filename: lightly-ai-openapi.yml
  format: yaml
  label: Lightly Datasets API
  slug: lightly-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightly-ai/refs/heads/main/openapi/lightly-ai-openapi.yml
- filename: lightly-ai-openapi.yml
  format: yaml
  label: Lightly Samples and Embeddings API
  slug: lightly-samples-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightly-ai/refs/heads/main/openapi/lightly-ai-openapi.yml
- filename: lightly-ai-openapi.yml
  format: yaml
  label: Lightly Datasources API
  slug: lightly-datasources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightly-ai/refs/heads/main/openapi/lightly-ai-openapi.yml
- filename: lightly-ai-openapi.yml
  format: yaml
  label: Lightly Selection and Active Learning API
  slug: lightly-selection-active-learning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightly-ai/refs/heads/main/openapi/lightly-ai-openapi.yml
- filename: lightly-ai-openapi.yml
  format: yaml
  label: Lightly Jobs and Tags API
  slug: lightly-jobs-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightly-ai/refs/heads/main/openapi/lightly-ai-openapi.yml
consequence_counts:
  read: 20
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Lightly Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 31
overview: 'Lightly exposes 31 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 read and 11 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Lightly
provider_slug: lightly-ai
slug: lightly-ai-agentic-access
source_filename: lightly-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/lightly-ai-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 31\n  by_action_class:\n    connected: 20\n    acting: 11\n  by_consequence:\n    read: 20\n    write: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/datasets\n  method: get\n  operationId: getDatasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/datasets\n  method: post\n  operationId: createDataset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/datasets/{datasetId}\n  method: get\n  operationId: getDatasetById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/datasets/{datasetId}\n  method: put\n  operationId: updateDatasetById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/datasets/{datasetId}\n  method: delete\n  operationId: deleteDatasetById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/datasets/{datasetId}/children\n  method: get\n  operationId: getChildrenOfDatasetById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/datasets/query/name/{datasetName}\n  method: get\n  operationId: getDatasetsQueryByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/datasets/{datasetId}/registerDatasetUpload\n  method: put\n  operationId: registerDatasetUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/datasets/{datasetId}/samples\n  method: get\n  operationId: getSamplesByDatasetId\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/datasets/{datasetId}/samples\n  method: post\n  operationId: createSampleByDatasetId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/datasets/{datasetId}/samples/{sampleId}\n  method: get\n  operationId: getSampleById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/datasets/{datasetId}/samples/{sampleId}\n  method: put\n  operationId: updateSampleById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/datasets/{datasetId}/samples/{sampleId}/readurl\n  method: get\n  operationId: getSampleImageReadUrlById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/datasets/{datasetId}/samples/{sampleId}/writeurl\n  method: get\n  operationId: getSampleImageWriteUrlById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/datasets/{datasetId}/embeddings\n  method: get\n  operationId: getEmbeddingsByDatasetId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/datasets/{datasetId}/embeddings/{embeddingId}\n  method: delete\n  operationId:\
  \ deleteEmbeddingById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/datasets/{datasetId}/embeddings/writeCSVUrl\n  method: get\n  operationId: getEmbeddingsCSVWriteUrlById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/datasets/{datasetId}/embeddings/{embeddingId}/readCSVUrl\n  method: get\n  operationId: getEmbeddingsCSVReadUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/datasets/{datasetId}/embeddings/{embeddingId}/trigger2dEmbeddingsJob\n  method: post\n  operationId: trigger2dEmbeddingsJob\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/datasets/{datasetId}/datasource\n  method: get\n  operationId: getDatasourceByDatasetId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/datasets/{datasetId}/datasource/processedUntilTimestamp\n  method: get\n  operationId: getDatasourceProcessedUntilTimestampByDatasetId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/datasets/{datasetId}/datasource/list\n  method: get\n  operationId: getListOfRawSamplesFromDatasource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/docker/worker/default\n  method: get\n  operationId: getDockerWorkerRegistryEntries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/datasets/{datasetId}/docker/worker/schedule\n  method: post\n  operationId: createDockerWorkerScheduleByDatasetId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/docker/runs\n  method: get\n  operationId: getDockerRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/docker/runs/{runId}/artifacts/{artifactId}\n  method: get\n  operationId: getDockerRunArtifactReadUrl\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs\n  method: get\n  operationId: getJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/{jobId}\n  method: get\n  operationId: getJobStatusById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/datasets/{datasetId}/tags\n  method: post\n  operationId: createTagByDatasetId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/datasets/{datasetId}/tags/{tagId}\n  method: delete\n\
  \  operationId: deleteTagByTagId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/datasets/{datasetId}/tags/{tagId}/export/LabelStudio/tasks\n  method: get\n  operationId: exportTagToLabelStudioTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightly-ai/refs/heads/main/agentic-access/lightly-ai-agentic-access.yml
summary_line: 31 operations · 11 acting
tags:
- AI
- Computer Vision
- Data Curation
- Active Learning
- Embeddings
---
