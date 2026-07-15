---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 5
api_specs:
- filename: uptrain-openapi.yml
  format: yaml
  label: UpTrain Evaluations API
  slug: uptrain-evaluations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptrain/refs/heads/main/openapi/uptrain-openapi.yml
- filename: uptrain-openapi.yml
  format: yaml
  label: UpTrain Log and Evaluate API
  slug: uptrain-log-and-evaluate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptrain/refs/heads/main/openapi/uptrain-openapi.yml
- filename: uptrain-openapi.yml
  format: yaml
  label: UpTrain Root Cause Analysis API
  slug: uptrain-root-cause-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptrain/refs/heads/main/openapi/uptrain-openapi.yml
- filename: uptrain-openapi.yml
  format: yaml
  label: UpTrain Runs and Datasets API
  slug: uptrain-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptrain/refs/heads/main/openapi/uptrain-openapi.yml
consequence_counts:
  read: 5
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Uptrain Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'UpTrain exposes 11 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: UpTrain
provider_slug: uptrain
slug: uptrain-agentic-access
source_filename: uptrain-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/uptrain-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 5\n    acting: 6\n  by_consequence:\n    read: 5\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /auth\n  method: get\n  operationId: checkAuth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /evaluate\n  method: post\n  operationId: evaluate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /log_and_evaluate\n  method: post\n  operationId: logAndEvaluate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /perform_root_cause_analysis\n  method: post\n  operationId: performRootCauseAnalysis\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /run\n  method: post\n  operationId: addRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /run/{run_id}\n  method: get\n  operationId: getRun\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /run/{run_id}/results\n  method: get\n  operationId: getRunResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dataset\n  method: post\n  operationId: addDataset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dataset\n  method: get\n  operationId: getDataset\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /checkset\n  method: post\n  operationId: addCheckset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /evaluation_results/{project_name}\n  method: get\n  operationId: downloadProjectEvalResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uptrain/refs/heads/main/agentic-access/uptrain-agentic-access.yml
summary_line: 11 operations · 6 acting
tags:
- AI
- LLM
- Evaluation
- LLM Evaluation
- Observability
- Open Source
---
