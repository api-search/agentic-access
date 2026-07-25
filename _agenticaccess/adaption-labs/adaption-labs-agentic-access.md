---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 5
api_specs:
- filename: adaption-labs-datasets-api-openapi.yml
  format: yaml
  label: Adaption Labs Datasets API
  slug: adaption-labs-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adaption-labs/refs/heads/main/openapi/adaption-labs-datasets-api-openapi.yml
- filename: adaption-labs-upload-api-openapi.yml
  format: yaml
  label: Adaption Labs Upload API
  slug: adaption-labs-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adaption-labs/refs/heads/main/openapi/adaption-labs-upload-api-openapi.yml
consequence_counts:
  read: 5
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Adaption Labs Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'Adaption Labs exposes 11 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Adaption Labs
provider_slug: adaption-labs
slug: adaption-labs-agentic-access
source_filename: adaption-labs-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: generated\nsource: openapi/adaption-labs-datasets-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    acting: 6\n    connected: 5\n  by_consequence:\n    write: 6\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/datasets\n  method: post\n  operationId: createDataset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/datasets\n  method: get\n  operationId: listDatasets\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/datasets/{dataset_id}\n  method: get\n  operationId: getDataset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/datasets/{dataset_id}/status\n  method: get\n  operationId: getDatasetStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/datasets/{dataset_id}/evaluation\n  method: get\n  operationId: getDatasetEvaluation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/datasets/{dataset_id}/run\n  method: post\n  operationId: runDataset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/datasets/{dataset_id}/download\n  method: get\n  operationId: downloadDataset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/datasets/{dataset_id}/publish\n  method: post\n  operationId: publishDataset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/datasets/upload/initiate\n  method: post\n  operationId: initiateUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n \
  \     max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/datasets/upload/complete\n  method: post\n  operationId: completeUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/datasets/{dataset_id}/upload/complete\n  method: post\n  operationId: completeUploadById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adaption-labs/refs/heads/main/agentic-access/adaption-labs-agentic-access.yml
summary_line: 11 operations · 6 acting
tags:
- Company
- AI
- Machine Learning
- Training Data
- Datasets
- LLM
- Adaptive Data
- SDK
---
