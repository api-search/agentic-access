---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 4
api_specs:
- filename: amazon-lookout-for-equipment-datasets-api-openapi.yml
  format: yaml
  label: Amazon Lookout for Equipment Datasets API
  slug: amazon-lookout-for-equipment-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-lookout-for-equipment/openapi/amazon-lookout-for-equipment-datasets-api-openapi.yml
- filename: amazon-lookout-for-equipment-data-ingestion-job-api-openapi.yml
  format: yaml
  label: Amazon Lookout for Equipment Lookout For Equipment Data Ingestion Job API
  slug: amazon-lookout-for-equipment-data-ingestion-job-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-lookout-for-equipment/openapi/amazon-lookout-for-equipment-data-ingestion-job-api-openapi.yml
- filename: amazon-lookout-for-equipment-inference-scheduler-api-openapi.yml
  format: yaml
  label: Amazon Lookout for Equipment Lookout For Equipment Inference Scheduler API
  slug: amazon-lookout-for-equipment-inference-scheduler-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-lookout-for-equipment/openapi/amazon-lookout-for-equipment-inference-scheduler-api-openapi.yml
- filename: amazon-lookout-for-equipment-label-api-openapi.yml
  format: yaml
  label: Amazon Lookout for Equipment Lookout For Equipment Label API
  slug: amazon-lookout-for-equipment-label-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-lookout-for-equipment/openapi/amazon-lookout-for-equipment-label-api-openapi.yml
- filename: amazon-lookout-for-equipment-label-group-api-openapi.yml
  format: yaml
  label: Amazon Lookout for Equipment Lookout For Equipment Label Group API
  slug: amazon-lookout-for-equipment-label-group-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-lookout-for-equipment/openapi/amazon-lookout-for-equipment-label-group-api-openapi.yml
- filename: amazon-lookout-for-equipment-model-version-api-openapi.yml
  format: yaml
  label: Amazon Lookout for Equipment Lookout For Equipment Model Version API
  slug: amazon-lookout-for-equipment-model-version-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-lookout-for-equipment/openapi/amazon-lookout-for-equipment-model-version-api-openapi.yml
- filename: amazon-lookout-for-equipment-operations-api-openapi.yml
  format: yaml
  label: Amazon Lookout for Equipment Lookout For Equipment Operations API
  slug: amazon-lookout-for-equipment-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-lookout-for-equipment/openapi/amazon-lookout-for-equipment-operations-api-openapi.yml
- filename: amazon-lookout-for-equipment-resource-policy-api-openapi.yml
  format: yaml
  label: Amazon Lookout for Equipment Lookout For Equipment Resource Policy API
  slug: amazon-lookout-for-equipment-resource-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-lookout-for-equipment/openapi/amazon-lookout-for-equipment-resource-policy-api-openapi.yml
- filename: amazon-lookout-for-equipment-retraining-scheduler-api-openapi.yml
  format: yaml
  label: Amazon Lookout for Equipment Lookout For Equipment Retraining Scheduler API
  slug: amazon-lookout-for-equipment-retraining-scheduler-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-lookout-for-equipment/openapi/amazon-lookout-for-equipment-retraining-scheduler-api-openapi.yml
consequence_counts:
  read: 4
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Amazon Lookout For Equipment Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Amazon Lookout for Equipment exposes 8 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amazon Lookout for Equipment
provider_slug: amazon-lookout-for-equipment
slug: amazon-lookout-for-equipment-agentic-access
source_filename: amazon-lookout-for-equipment-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/amazon-lookout-for-equipment-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 4\n    connected: 4\n  by_consequence:\n    write: 4\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /datasets\n  method: post\n  operationId: CreateDataset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets\n  method: get\n  operationId: ListDatasets\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets/{DatasetName}\n  method: get\n  operationId: DescribeDataset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets/{DatasetName}\n  method: delete\n  operationId: DeleteDataset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /models\n  method: post\n  operationId: CreateModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n \
  \   audit: required\n- path: /models\n  method: get\n  operationId: ListModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /models/{ModelName}\n  method: get\n  operationId: DescribeModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inference-schedulers/{InferenceSchedulerName}/start\n  method: post\n  operationId: StartInferenceScheduler\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/amazon-lookout-for-equipment/agentic-access/amazon-lookout-for-equipment-agentic-access.yml
summary_line: 8 operations · 4 acting
tags:
- Amazon Web Services
- Equipment Monitoring
- Industrial IoT
- Machine Learning
- Predictive Maintenance
---
