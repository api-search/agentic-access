---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 11
api_specs:
- filename: freeplay-openapi.yml
  format: yaml
  label: Freeplay Prompt Templates API
  slug: prompt-templates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freeplay/refs/heads/main/openapi/freeplay-openapi.yml
- filename: freeplay-openapi.yml
  format: yaml
  label: Freeplay Recordings & Sessions API
  slug: recordings-sessions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freeplay/refs/heads/main/openapi/freeplay-openapi.yml
- filename: freeplay-openapi.yml
  format: yaml
  label: Freeplay Test Cases & Datasets API
  slug: test-cases-datasets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freeplay/refs/heads/main/openapi/freeplay-openapi.yml
- filename: freeplay-openapi.yml
  format: yaml
  label: Freeplay Test Runs & Evaluations API
  slug: test-runs-evaluations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freeplay/refs/heads/main/openapi/freeplay-openapi.yml
consequence_counts:
  physical: 1
  read: 11
  write: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Freeplay Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /projects/{project_id}/prompt-templates/id/{template_id}/versions/{version_id}/environments
operation_count: 29
overview: 'Freeplay exposes 29 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 17 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Freeplay
provider_slug: freeplay
slug: freeplay-agentic-access
source_filename: freeplay-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/freeplay-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 29\n  by_action_class:\n    connected: 11\n    acting: 18\n  by_consequence:\n    read: 11\n    write: 17\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /projects/all\n  method: get\n  operationId: listProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/prompt-templates\n  method: get\n  operationId: listPromptTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /projects/{project_id}/prompt-templates\n  method: post\n  operationId: createPromptTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/prompt-templates/all/{environment_name}\n  method: get\n  operationId: getAllPromptTemplatesInEnvironment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/prompt-templates/name/{template_name}\n  method: post\n  operationId: getPromptTemplateByName\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n \
  \     triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/prompt-templates/name/{template_name}/versions\n  method: post\n  operationId: createPromptTemplateVersionByName\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/prompt-templates/id/{template_id}/versions\n  method: post\n  operationId: createPromptTemplateVersionById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/prompt-templates/id/{template_id}/versions/{version_id}\n\
  \  method: post\n  operationId: getPromptTemplateVersionById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/prompt-templates/id/{template_id}/versions/{version_id}/environments\n  method: post\n  operationId: assignPromptTemplateVersionToEnvironments\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/sessions\n  method: get\n  operationId: listSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/sessions/{session_id}\n  method: delete\n  operationId: deleteSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/sessions/{session_id}/completions\n  method: post\n  operationId: recordCompletion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/sessions/{session_id}/traces/id/{trace_id}\n  method: post\n  operationId: recordTrace\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/completions/statistics\n  method: post\n  operationId: getCompletionStatistics\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/completions/statistics/{prompt_template_id}\n  method: post\n  operationId: getCompletionStatisticsByTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /projects/{project_id}/datasets/name/{dataset_name}\n  method: get\n  operationId: getDatasetByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/datasets/id/{dataset_id}\n  method: get\n  operationId: getDatasetById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/datasets/name/{dataset_name}/test-cases\n  method: get\n  operationId: getTestCasesByDatasetName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/datasets/id/{dataset_id}/test-cases\n  method: get\n  operationId: getTestCasesByDatasetId\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/datasets/id/{dataset_id}/test-cases\n  method: post\n  operationId: uploadTestCases\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/test-runs\n  method: get\n  operationId: listTestRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/test-runs\n  method: post\n  operationId: createTestRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n    \
  \  triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/test-runs/id/{test_run_id}\n  method: get\n  operationId: getTestRun\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/completion-feedback/id/{completion_id}\n  method: post\n  operationId: recordCompletionFeedback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/trace-feedback/id/{trace_id}\n  method: post\n  operationId: recordTraceFeedback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/search/sessions\n  method: post\n  operationId: searchSessions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/search/traces\n  method: post\n  operationId: searchTraces\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/search/completions\n  method: post\n  operationId: searchCompletions\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/agents\n  method: get\n  operationId: listAgents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freeplay/refs/heads/main/agentic-access/freeplay-agentic-access.yml
summary_line: 29 operations · 18 acting
tags:
- AI
- LLM
- Evaluation
- Observability
- Prompt Management
- Experimentation
---
