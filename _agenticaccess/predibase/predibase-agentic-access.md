---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 11
api_specs:
- filename: predibase-openapi.yml
  format: yaml
  label: Predibase Inference (OpenAI-Compatible) API
  slug: predibase-inference-openai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/predibase/refs/heads/main/openapi/predibase-openapi.yml
- filename: predibase-openapi.yml
  format: yaml
  label: Predibase Prompt / Generate API
  slug: predibase-prompt-generate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/predibase/refs/heads/main/openapi/predibase-openapi.yml
- filename: predibase-openapi.yml
  format: yaml
  label: Predibase Fine-Tuning API
  slug: predibase-fine-tuning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/predibase/refs/heads/main/openapi/predibase-openapi.yml
- filename: predibase-openapi.yml
  format: yaml
  label: Predibase Adapters API
  slug: predibase-adapters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/predibase/refs/heads/main/openapi/predibase-openapi.yml
- filename: predibase-openapi.yml
  format: yaml
  label: Predibase Deployments API
  slug: predibase-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/predibase/refs/heads/main/openapi/predibase-openapi.yml
- filename: predibase-openapi.yml
  format: yaml
  label: Predibase Datasets API
  slug: predibase-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/predibase/refs/heads/main/openapi/predibase-openapi.yml
- filename: predibase-openapi.yml
  format: yaml
  label: Predibase Models API
  slug: predibase-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/predibase/refs/heads/main/openapi/predibase-openapi.yml
- filename: predibase-openapi.yml
  format: yaml
  label: Predibase Batch Inference API
  slug: predibase-batch-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/predibase/refs/heads/main/openapi/predibase-openapi.yml
consequence_counts:
  physical: 2
  read: 11
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Predibase Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /deployments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /deployments/{deploymentName}
operation_count: 23
overview: 'Predibase exposes 23 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 10 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Predibase
provider_slug: predibase
slug: predibase-agentic-access
source_filename: predibase-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/predibase-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    acting: 12\n    connected: 11\n  by_consequence:\n    write: 10\n    read: 11\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/chat/completions\n  method: post\n  operationId: createChatCompletion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/completions\n  method: post\n  operationId: createCompletion\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /generate\n  method: post\n  operationId: generate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /generate_stream\n  method: post\n  operationId: generateStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /finetuning/jobs\n  method: post\n  operationId:\
  \ createFinetuningJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /finetuning/jobs\n  method: get\n  operationId: listFinetuningJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /finetuning/jobs/{jobId}\n  method: get\n  operationId: getFinetuningJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /finetuning/jobs/{jobId}/cancel\n  method: post\n  operationId: cancelFinetuningJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /repos\n  method: post\n  operationId: createRepo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /repos\n  method: get\n  operationId: listRepos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repos/{repoName}\n  method: get\n  operationId: getRepo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repos/{repoName}\n  method: delete\n  operationId: deleteRepo\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deployments\n  method: post\n  operationId: createDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deployments\n  method: get\n  operationId: listDeployments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deployments/{deploymentName}\n  method: get\n  operationId: getDeployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deployments/{deploymentName}\n  method: delete\n  operationId: deleteDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets\n  method: post\n  operationId: createDataset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets\n  method: get\n  operationId: listDatasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n  \
  \    max-ttl: 3600\n    audit: none\n- path: /datasets/{datasetName}\n  method: get\n  operationId: getDataset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /models\n  method: get\n  operationId: listModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /batch-inference/jobs\n  method: post\n  operationId: createBatchInferenceJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /batch-inference/jobs\n  method: get\n  operationId: listBatchInferenceJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /batch-inference/jobs/{jobId}\n  method: get\n  operationId: getBatchInferenceJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/predibase/refs/heads/main/agentic-access/predibase-agentic-access.yml
summary_line: 23 operations · 12 acting
tags:
- AI
- LLM
- Fine-Tuning
- Inference
- LoRA
---
