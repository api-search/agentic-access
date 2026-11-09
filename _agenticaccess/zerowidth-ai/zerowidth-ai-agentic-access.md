---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 14
api_specs:
- filename: zerowidth-ai-caliper-api-openapi.yml
  format: yaml
  label: zerowidth-ai Caliper API
  slug: zerowidth-ai-caliper-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zerowidth-ai/openapi/zerowidth-ai-caliper-api-openapi.yml
- filename: zerowidth-ai-flows-api-openapi.yml
  format: yaml
  label: zerowidth-ai Flows API
  slug: zerowidth-ai-flows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zerowidth-ai/openapi/zerowidth-ai-flows-api-openapi.yml
- filename: zerowidth-ai-knowledge-bases-api-openapi.yml
  format: yaml
  label: zerowidth-ai Knowledge Bases API
  slug: zerowidth-ai-knowledge-bases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zerowidth-ai/openapi/zerowidth-ai-knowledge-bases-api-openapi.yml
- filename: zerowidth-ai-ledger-api-openapi.yml
  format: yaml
  label: zerowidth-ai Ledger API
  slug: zerowidth-ai-ledger-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zerowidth-ai/openapi/zerowidth-ai-ledger-api-openapi.yml
- filename: zerowidth-ai-shims-api-openapi.yml
  format: yaml
  label: zerowidth-ai Shims API
  slug: zerowidth-ai-shims-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zerowidth-ai/openapi/zerowidth-ai-shims-api-openapi.yml
- filename: zerowidth-ai-tasks-api-openapi.yml
  format: yaml
  label: zerowidth-ai Tasks API
  slug: zerowidth-ai-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zerowidth-ai/openapi/zerowidth-ai-tasks-api-openapi.yml
consequence_counts:
  physical: 2
  read: 14
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Zerowidth Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /1.0/caliper/feedback
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /1.0/caliper/traces
operation_count: 26
overview: 'zerowidth-ai exposes 26 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read, 10 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: zerowidth-ai
provider_slug: zerowidth-ai
slug: zerowidth-ai-agentic-access
source_filename: zerowidth-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/zerowidth-ai-caliper-api-openapi.yml, openapi/zerowidth-ai-flows-api-openapi.yml,\n  openapi/zerowidth-ai-knowledge-bases-api-openapi.yml, openapi/zerowidth-ai-ledger-api-openapi.yml,\n  openapi/zerowidth-ai-shims-api-openapi.yml, openapi/zerowidth-ai-tasks-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 26\n  by_action_class:\n    connected: 14\n    acting: 12\n  by_consequence:\n    read: 14\n    write: 10\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /1.0/caliper/evals\n  method: get\n  operationId: get_1_0_caliper_evals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /1.0/caliper/evals\n  method: post\n  operationId: post_1_0_caliper_evals\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /1.0/caliper/evals/{id}\n  method: get\n  operationId: get_1_0_caliper_evals_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1.0/caliper/evals/{id}/runs\n  method: post\n  operationId: post_1_0_caliper_evals_id_runs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /1.0/caliper/evals/{id}/runs/{runid}\n  method: get\n  operationId: get_1_0_caliper_evals_id_runs_runid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1.0/caliper/feedback\n  method: post\n  operationId: post_1_0_caliper_feedback\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /1.0/caliper/traces\n  method: post\n  operationId: post_1_0_caliper_traces\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /1.0/flows\n  method: post\n  operationId: post_1_0_flows\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /1.0/flows/{flowuuid}/fork\n  method: post\n  operationId: post_1_0_flows_flowuuid_fork\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /1.0/flows/{flowuuid}/runs\n  method: post\n  operationId: post_1_0_flows_flowuuid_runs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /1.0/flows/public\n  method: get\n  operationId: get_1_0_flows_public\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1.0/flows/public\n  method: post\n  operationId: post_1_0_flows_public\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /1.0/flows/public/{flowuuid}\n  method: get\n  operationId: get_1_0_flows_public_flowuuid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /1.0/knowledge-bases\n  method: get\n  operationId: get_1_0_knowledge_bases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1.0/knowledge-bases\n  method: post\n  operationId: post_1_0_knowledge_bases\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /1.0/knowledge-bases/{id}\n  method: get\n  operationId: get_1_0_knowledge_bases_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1.0/knowledge-bases/{id}/documents\n  method: post\n  operationId: post_1_0_knowledge_bases_id_documents\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /1.0/knowledge-bases/{id}/search\n  method: post\n  operationId: post_1_0_knowledge_bases_id_search\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /1.0/ledger/metrics\n  method: get\n  operationId: get_1_0_ledger_metrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1.0/ledger/metrics/{id}/readings\n  method: get\n  operationId: get_1_0_ledger_metrics_id_readings\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1.0/shims\n  method: get\n  operationId: get_1_0_shims\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1.0/shims/{id}\n  method: get\n  operationId: get_1_0_shims_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1.0/shims/{id}/weights\n  method: get\n  operationId: get_1_0_shims_id_weights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1.0/tasks\n  method: get\n  operationId: get_1_0_tasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1.0/tasks/{taskid}/runs\n\
  \  method: post\n  operationId: post_1_0_tasks_taskid_runs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /1.0/tasks/{taskid}/runs/{runid}\n  method: get\n  operationId: get_1_0_tasks_taskid_runs_runid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/zerowidth-ai/agentic-access/zerowidth-ai-agentic-access.yml
summary_line: 26 operations · 12 acting
tags:
- Artificial Intelligence
- Automation
- Consulting
- Software-as-a-Service
- Platform
---
