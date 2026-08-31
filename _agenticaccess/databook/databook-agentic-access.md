---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 5
api_specs:
- filename: databook-batch-create-api-openapi.yml
  format: yaml
  label: Databook batch - create API
  slug: databook-batch-create-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/databook/refs/heads/main/openapi/databook-batch-create-api-openapi.yml
- filename: databook-batch-query-api-openapi.yml
  format: yaml
  label: Databook batch - query API
  slug: databook-batch-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/databook/refs/heads/main/openapi/databook-batch-query-api-openapi.yml
- filename: databook-chat-api-openapi.yml
  format: yaml
  label: Databook Chat API
  slug: databook-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/databook/refs/heads/main/openapi/databook-chat-api-openapi.yml
- filename: databook-reasoning-api-openapi.yml
  format: yaml
  label: Databook Reasoning API
  slug: databook-reasoning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/databook/refs/heads/main/openapi/databook-reasoning-api-openapi.yml
consequence_counts:
  read: 5
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Databook Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Databook exposes 8 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Databook
provider_slug: databook
slug: databook-agentic-access
source_filename: databook-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: generated\nsource: openapi/databook-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 3\n    connected: 5\n  by_consequence:\n    write: 3\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/batch/job\n  method: post\n  operationId: create_job_v1_batch_job_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/batch/job\n  method: get\n  operationId: list_job_v1_batch_job_get\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/batch/job/input-csv-template\n  method: get\n  operationId: get_job_input_csv_template_v1_batch_job_input_csv_template_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/batch/job/{job_id}\n  method: get\n  operationId: get_job_by_id_v1_batch_job__job_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/batch/job/{job_id}/result\n  method: get\n  operationId: get_job_result_by_id_v1_batch_job__job_id__result_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chat\n  method: post\n  operationId: chat_v1_chat_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/insights\n  method: get\n  operationId: list_insights_v1_insights_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reasoning\n  method: post\n  operationId: run_reasoning_v1_reasoning_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/databook/refs/heads/main/agentic-access/databook-agentic-access.yml
summary_line: 8 operations · 3 acting
tags:
- Company
- Vertical Software
- Sales Intelligence
- Account Intelligence
- Sales Enablement
- Enterprise Sales
- Artificial Intelligence
- Revenue Operations
- REST API
- OpenAPI
- Batch Processing
- Agents
- Reasoning
- Company Data
---
