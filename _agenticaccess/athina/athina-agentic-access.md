---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 4
api_specs:
- filename: athina-openapi.yml
  format: yaml
  label: Athina Logging & Inferences API
  slug: athina-logging-inferences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athina/refs/heads/main/openapi/athina-openapi.yml
- filename: athina-openapi.yml
  format: yaml
  label: Athina Datasets API
  slug: athina-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athina/refs/heads/main/openapi/athina-openapi.yml
- filename: athina-openapi.yml
  format: yaml
  label: Athina Evaluations API
  slug: athina-evaluations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athina/refs/heads/main/openapi/athina-openapi.yml
- filename: athina-openapi.yml
  format: yaml
  label: Athina Prompts API
  slug: athina-prompts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athina/refs/heads/main/openapi/athina-openapi.yml
- filename: athina-openapi.yml
  format: yaml
  label: Athina Experiments API
  slug: athina-experiments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athina/refs/heads/main/openapi/athina-openapi.yml
consequence_counts:
  read: 4
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Athina Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 18
overview: 'Athina AI exposes 18 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 14 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Athina AI
provider_slug: athina
slug: athina-agentic-access
source_filename: athina-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/athina-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    acting: 14\n    connected: 4\n  by_consequence:\n    write: 14\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /log/inference\n  method: post\n  operationId: logInference\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /logs/{log_id}\n  method: put\n  operationId: updateLogById\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /logs/external/{external_reference_id}\n  method: put\n  operationId: updateLogByExternalReferenceId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /trace/\n  method: post\n  operationId: createTrace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /trace/{trace_id}\n  method: get\n  operationId: getTrace\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trace/{trace_id}\n  method: put\n  operationId: updateTrace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /trace/{trace_id}/spans\n  method: post\n  operationId: createSpan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /trace/{trace_id}/spans/{span_id}\n  method: get\n  operationId: getSpan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trace/{trace_id}/spans/{span_id}\n  method: put\n  operationId: updateSpan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dataset_v2\n  method: post\n  operationId: createDataset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dataset_v2/{dataset_id}\n  method: get\n  operationId: getDataset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /dataset_v2/{dataset_id}\n  method: delete\n  operationId: deleteDataset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dataset_v2/{dataset_id}/add-rows\n  method: post\n  operationId: addDatasetRows\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dataset_v2/{dataset_id}/cell\n  method: post\n  operationId: updateDatasetCell\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /eval/run\n  method: post\n  operationId: runEval\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /prompt/{prompt_slug}\n  method: put\n  operationId: createPromptTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /prompt/{prompt_slug}/default\n  method: get\n  operationId: getDefaultPrompt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /prompt/{prompt_slug}/run\n  method: post\n  operationId: runPrompt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/athina/refs/heads/main/agentic-access/athina-agentic-access.yml
summary_line: 18 operations · 14 acting
tags:
- AI
- LLM
- Observability
- Evaluation
- Monitoring
---
