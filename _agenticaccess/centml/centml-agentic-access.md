---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 8
api_specs:
- filename: centml-openapi.yml
  format: yaml
  label: CentML Serverless Inference (Chat Completions) API
  slug: centml-serverless-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centml/refs/heads/main/openapi/centml-openapi.yml
- filename: centml-openapi.yml
  format: yaml
  label: CentML Models API
  slug: centml-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centml/refs/heads/main/openapi/centml-openapi.yml
- filename: centml-openapi.yml
  format: yaml
  label: CentML Deployments / Endpoints API
  slug: centml-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centml/refs/heads/main/openapi/centml-openapi.yml
- filename: centml-openapi.yml
  format: yaml
  label: CentML Clusters API
  slug: centml-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centml/refs/heads/main/openapi/centml-openapi.yml
consequence_counts:
  physical: 4
  read: 8
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Centml Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /deployments/compute
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /deployments/inference
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /deployments/inference
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /deployments/status/{deployment_id}
operation_count: 14
overview: 'CentML exposes 14 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 2 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CentML
provider_slug: centml
slug: centml-agentic-access
source_filename: centml-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/centml-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    acting: 6\n    connected: 8\n  by_consequence:\n    write: 2\n    read: 8\n    physical: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /chat/completions\n  method: post\n  operationId: createChatCompletion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /completions\n  method: post\n  operationId: createCompletion\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /models\n  method: get\n  operationId: listModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /models/{model}\n  method: get\n  operationId: retrieveModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deployments\n  method: get\n  operationId: listDeployments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deployments/inference\n  method: post\n  operationId: createInferenceDeployment\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deployments/inference\n  method: put\n  operationId: updateInferenceDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deployments/inference/{deployment_id}\n  method: get\n  operationId: getInferenceDeployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deployments/compute\n  method:\
  \ post\n  operationId: createComputeDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deployments/status/{deployment_id}\n  method: get\n  operationId: getDeploymentStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deployments/status/{deployment_id}\n  method: put\n  operationId: updateDeploymentStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n     \
  \ - abnormal\n      - high-value\n    audit: required\n- path: /deployments/logs/{deployment_id}\n  method: get\n  operationId: getDeploymentLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clusters\n  method: get\n  operationId: getClusters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /capacity\n  method: get\n  operationId: listCapacity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/centml/refs/heads/main/agentic-access/centml-agentic-access.yml
summary_line: 14 operations · 6 acting
tags:
- AI
- LLM
- Inference
- Serverless
- GPU
---
