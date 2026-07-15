---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 6
api_specs:
- filename: amazon-bedrock-openapi.yml
  format: yaml
  label: Amazon Bedrock API
  slug: amazon-bedrock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-bedrock/refs/heads/main/openapi/amazon-bedrock-openapi.yml
- filename: amazon-bedrock-runtime-openapi.yml
  format: yaml
  label: Amazon Bedrock Runtime API
  slug: amazon-bedrock-runtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-bedrock/refs/heads/main/openapi/amazon-bedrock-runtime-openapi.yml
consequence_counts:
  physical: 1
  read: 6
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Amazon Bedrock Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /provisioned-model-throughput
operation_count: 12
overview: 'Amazon Bedrock exposes 12 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 5 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amazon Bedrock
provider_slug: amazon-bedrock
slug: amazon-bedrock-agentic-access
source_filename: amazon-bedrock-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/amazon-bedrock-openapi.yml, openapi/amazon-bedrock-runtime-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 6\n    acting: 6\n  by_consequence:\n    read: 6\n    write: 5\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /foundation-models\n  method: get\n  operationId: ListFoundationModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /foundation-models/{modelIdentifier}\n  method: get\n  operationId: GetFoundationModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /model-customization-jobs\n  method: post\n  operationId: CreateModelCustomizationJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /model-customization-jobs\n  method: get\n  operationId: ListModelCustomizationJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /model-customization-jobs/{jobIdentifier}\n  method: get\n  operationId: GetModelCustomizationJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /custom-models\n  method: get\n  operationId: ListCustomModels\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provisioned-model-throughput\n  method: post\n  operationId: CreateProvisionedModelThroughput\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provisioned-model-throughput\n  method: get\n  operationId: ListProvisionedModelThroughputs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /model/{modelId}/invoke\n  method: post\n  operationId: InvokeModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /model/{modelId}/invoke-with-response-stream\n  method: post\n  operationId: InvokeModelWithResponseStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /model/{modelId}/converse\n  method: post\n  operationId: Converse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /model/{modelId}/converse-stream\n  method: post\n  operationId:\
  \ ConverseStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-bedrock/refs/heads/main/agentic-access/amazon-bedrock-agentic-access.yml
summary_line: 12 operations · 6 acting
tags:
- AI
- Foundation Models
- Generative AI
- LLM
- Machine Learning
- RAG
- Agents
- Responsible AI
---
