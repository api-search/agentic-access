---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 10
api_specs:
- filename: trydatabook-com-openapi.json
  format: json
  label: DatabookAI REST API
  slug: databookai-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trydatabook-com/refs/heads/main/openapi/trydatabook-com-openapi.json
consequence_counts:
  read: 10
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Trydatabook Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'Databook exposes 14 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Databook
provider_slug: trydatabook-com
slug: trydatabook-com-agentic-access
source_filename: trydatabook-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: generated\nsource: openapi/trydatabook-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    acting: 4\n    connected: 10\n  by_consequence:\n    write: 4\n    read: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/batch/job\n  method: post\n  operationId: create_job_v1_batch_job_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/batch/job\n  method: get\n  operationId: list_job_v1_batch_job_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/batch/job/input-csv-template\n  method: get\n  operationId: get_job_input_csv_template_v1_batch_job_input_csv_template_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/batch/job/{job_id}\n  method: get\n  operationId: get_job_by_id_v1_batch_job__job_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/batch/job/{job_id}/result\n  method: get\n  operationId: get_job_result_by_id_v1_batch_job__job_id__result_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chat\n  method: post\n  operationId: chat_v1_chat_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/insights\n  method: get\n  operationId: list_insights_v1_insights_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/asset/library\n  method: get\n  operationId: list_services_v1_asset_library_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/asset/generated\n  method: get\n  operationId: list_requests_v1_asset_generated_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/asset/generated/{asset_generation_id}\n\
  \  method: get\n  operationId: get_generated_asset_v1_asset_generated__asset_generation_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/asset/generate\n  method: post\n  operationId: generate_asset_v1_asset_generate_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/asset/companies/{company_id}/professionals\n  method: get\n  operationId: list_professionals_v1_asset_companies__company_id__professionals_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/asset/companies\n  method: get\n  operationId: search_companies_v1_asset_companies_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reasoning\n  method: post\n  operationId: run_reasoning_v1_reasoning_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trydatabook-com/refs/heads/main/agentic-access/trydatabook-com-agentic-access.yml
summary_line: 14 operations · 4 acting
tags:
- Company
- Data Platform
- Business Intelligence
- APIs
- Venture-backed
---
