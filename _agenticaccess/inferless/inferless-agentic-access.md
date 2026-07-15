---
acting_count: 3
action_class_counts:
  acting: 3
api_specs:
- filename: inferless-openapi.yml
  format: yaml
  label: Inferless Inference Endpoints API
  slug: inferless-inference-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inferless/refs/heads/main/openapi/inferless-openapi.yml
- filename: inferless-openapi.yml
  format: yaml
  label: Inferless Model Management API
  slug: inferless-model-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inferless/refs/heads/main/openapi/inferless-openapi.yml
- filename: inferless-openapi.yml
  format: yaml
  label: Inferless Workspaces and Deployments
  slug: inferless-workspaces-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inferless/refs/heads/main/openapi/inferless-openapi.yml
consequence_counts:
  physical: 2
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Inferless Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rest/model/logs/get/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/inference/{model_name}/infer
operation_count: 3
overview: 'Inferless exposes 3 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 write and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Inferless
provider_slug: inferless
slug: inferless-agentic-access
source_filename: inferless-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/inferless-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 3\n  by_action_class:\n    acting: 3\n  by_consequence:\n    physical: 2\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/inference/{model_name}/infer\n  method: post\n  operationId: runInference\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rest/model/settings/update/\n  method: post\n  operationId:\
  \ updateModelSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rest/model/logs/get/\n  method: post\n  operationId: getModelLogs\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inferless/refs/heads/main/agentic-access/inferless-agentic-access.yml
summary_line: 3 operations · 3 acting
tags:
- AI
- ML Inference
- Serverless GPU
- Model Deployment
- Inference
---
