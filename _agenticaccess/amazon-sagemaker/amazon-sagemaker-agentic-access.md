---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 4
api_specs:
- filename: amazon-sagemaker-endpoints-api-openapi.yml
  format: yaml
  label: Amazon SageMaker Endpoints API
  slug: amazon-sagemaker-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-sagemaker/refs/heads/main/openapi/amazon-sagemaker-endpoints-api-openapi.yml
- filename: amazon-sagemaker-models-api-openapi.yml
  format: yaml
  label: Amazon SageMaker Models API
  slug: amazon-sagemaker-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-sagemaker/refs/heads/main/openapi/amazon-sagemaker-models-api-openapi.yml
- filename: amazon-sagemaker-notebook-instances-api-openapi.yml
  format: yaml
  label: Amazon SageMaker Notebook Instances API
  slug: amazon-sagemaker-notebook-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-sagemaker/refs/heads/main/openapi/amazon-sagemaker-notebook-instances-api-openapi.yml
- filename: amazon-sagemaker-training-jobs-api-openapi.yml
  format: yaml
  label: Amazon SageMaker Training Jobs API
  slug: amazon-sagemaker-training-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-sagemaker/refs/heads/main/openapi/amazon-sagemaker-training-jobs-api-openapi.yml
consequence_counts:
  read: 4
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Amazon Sagemaker Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'Amazon SageMaker exposes 13 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 9 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amazon SageMaker
provider_slug: amazon-sagemaker
slug: amazon-sagemaker-agentic-access
source_filename: amazon-sagemaker-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/amazon-sagemaker-endpoints-api-openapi.yml, openapi/amazon-sagemaker-models-api-openapi.yml,\n  openapi/amazon-sagemaker-notebook-instances-api-openapi.yml, openapi/amazon-sagemaker-training-jobs-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    acting: 9\n    connected: 4\n  by_consequence:\n    write: 9\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /#CreateEndpoint\n  method: post\n  operationId: CreateEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /#DescribeEndpoint\n  method: post\n  operationId: DescribeEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#ListEndpoints\n  method: post\n  operationId: ListEndpoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#CreateEndpointConfig\n  method: post\n  operationId: CreateEndpointConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /#CreateModel\n  method: post\n  operationId: CreateModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#DescribeModel\n  method: post\n  operationId: DescribeModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#ListModels\n  method: post\n  operationId: ListModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#CreateNotebookInstance\n  method: post\n  operationId: CreateNotebookInstance\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#DescribeNotebookInstance\n  method: post\n  operationId: DescribeNotebookInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#ListNotebookInstances\n  method: post\n  operationId: ListNotebookInstances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#CreateTrainingJob\n  method: post\n  operationId: CreateTrainingJob\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#DescribeTrainingJob\n  method: post\n  operationId: DescribeTrainingJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#ListTrainingJobs\n  method: post\n  operationId: ListTrainingJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-sagemaker/refs/heads/main/agentic-access/amazon-sagemaker-agentic-access.yml
summary_line: 13 operations · 9 acting
tags:
- Artificial Intelligence
- Inference
- Machine Learning
- MLOps
- Training
---
