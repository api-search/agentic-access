---
acting_count: 16
action_class_counts:
  acting: 16
  connected: 4
api_specs:
- filename: overview
  format: yaml
  label: Parea REST API
  slug: parea-rest-api
  spec_type: OpenAPI
  url: https://docs.parea.ai/api-reference/overview
consequence_counts:
  physical: 1
  read: 4
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Parea Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/parea/v1/deployed-prompt
operation_count: 20
overview: 'Parea AI exposes 20 API operations that an AI agent could call, of which 16 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read, 15 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Parea AI
provider_slug: parea
slug: parea-agentic-access
source_filename: parea-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/parea-rest-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    connected: 4\n    acting: 16\n  by_consequence:\n    read: 4\n    write: 15\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/parea/v1/\n  method: get\n  operationId: health_check_api_parea_v1__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/parea/v1/completion\n  method: post\n  operationId: completion_api_parea_v1_completion_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/parea/v1/completion/stream\n  method: post\n  operationId: stream_completion_api_parea_v1_completion_stream_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/parea/v1/deployed-prompt\n  method: post\n  operationId: fetch_deployed_prompt_api_parea_v1_deployed_prompt_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/parea/v1/feedback\n  method: post\n  operationId: record_feedback_api_parea_v1_feedback_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/parea/v1/trace_log\n  method: put\n  operationId: update_trace_log_api_parea_v1_trace_log_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/parea/v1/trace_log\n  method: post\n  operationId: record_trace_log_api_parea_v1_trace_log_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/parea/v1/trace_log/langchain\n  method: post\n  operationId: record_langchain_trace_log_api_parea_v1_trace_log_langchain_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/parea/v1/experiment\n  method: post\n  operationId: create_experiment_api_api_parea_v1_experiment_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/parea/v1/experiment/{experiment_uuid}/stats\n\
  \  method: get\n  operationId: get_experiment_stats_api_api_parea_v1_experiment__experiment_uuid__stats_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/parea/v1/experiment/{experiment_uuid}/finished\n  method: post\n  operationId: finish_experiment_api_api_parea_v1_experiment__experiment_uuid__finished_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/parea/v1/project\n  method: post\n  operationId: create_or_get_project_api_api_parea_v1_project_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/parea/v1/collection/{test_collection_identifier}\n  method: get\n  operationId: get_test_case_collection_by_identifier_api_parea_v1_collection__test_collection_identifier__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/parea/v1/collection\n  method: post\n  operationId: create_collection_api_parea_v1_collection_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/parea/v1/testcases\n  method: post\n  operationId: create_test_cases_for_dataset_api_parea_v1_testcases_post\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/parea/v1/trace_log/{trace_id}\n  method: get\n  operationId: get_trace_log_api_api_parea_v1_trace_log__trace_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/parea/v1/experiments\n  method: post\n  operationId: list_experiments_api_api_parea_v1_experiments_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/parea/v1/experiment/{experiment_uuid}/trace_logs\n  method: post\n  operationId: get_experiment_trace_logs_api_api_parea_v1_experiment__experiment_uuid__trace_logs_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/parea/v1/get_trace_logs\n  method: post\n  operationId: get_trace_logs_api_api_parea_v1_get_trace_logs_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/parea/v1/update_test_case/{dataset_id}/{test_case_id}\n  method: post\n  operationId: update_test_case_api_parea_v1_update_test_case__dataset_id___test_case_id__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parea/refs/heads/main/agentic-access/parea-agentic-access.yml
summary_line: 20 operations · 16 acting
tags:
- LLM
- Evaluation
- Observability
- Testing
- Prompt Management
- AI Engineering
- Machine Learning
- Tracing
- Experimentation
- Human Feedback
---
