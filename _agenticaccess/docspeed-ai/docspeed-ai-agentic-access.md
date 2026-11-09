---
acting_count: 34
action_class_counts:
  acting: 34
  connected: 10
api_specs:
- filename: docspeed-ai-agents-api-openapi.yml
  format: yaml
  label: Docspeed Agents API
  slug: docspeed-ai-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docspeed-ai/openapi/docspeed-ai-agents-api-openapi.yml
- filename: docspeed-ai-chat-api-openapi.yml
  format: yaml
  label: Docspeed Chat API
  slug: docspeed-ai-chat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docspeed-ai/openapi/docspeed-ai-chat-api-openapi.yml
- filename: docspeed-ai-extraction-api-openapi.yml
  format: yaml
  label: Docspeed Extraction API
  slug: docspeed-ai-extraction-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docspeed-ai/openapi/docspeed-ai-extraction-api-openapi.yml
- filename: docspeed-ai-files-api-openapi.yml
  format: yaml
  label: Docspeed Files API
  slug: docspeed-ai-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docspeed-ai/openapi/docspeed-ai-files-api-openapi.yml
- filename: docspeed-ai-generation-api-openapi.yml
  format: yaml
  label: Docspeed Generation API
  slug: docspeed-ai-generation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docspeed-ai/openapi/docspeed-ai-generation-api-openapi.yml
- filename: docspeed-ai-jobs-api-openapi.yml
  format: yaml
  label: Docspeed Jobs API
  slug: docspeed-ai-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docspeed-ai/openapi/docspeed-ai-jobs-api-openapi.yml
- filename: docspeed-ai-processing-api-openapi.yml
  format: yaml
  label: Docspeed Processing API
  slug: docspeed-ai-processing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docspeed-ai/openapi/docspeed-ai-processing-api-openapi.yml
consequence_counts:
  read: 10
  write: 34
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Docspeed Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 44
overview: 'Docspeed exposes 44 API operations that an AI agent could call, of which 34 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 34 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Docspeed
provider_slug: docspeed-ai
slug: docspeed-ai-agentic-access
source_filename: docspeed-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/docspeed-ai-openapi.json, openapi/openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 44\n  by_action_class:\n    connected: 10\n    acting: 34\n  by_consequence:\n    read: 10\n    write: 34\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/extract/files/{file_id}\n  method: get\n  operationId: get_public_file_api_v1_extract_files__file_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/extract/files/{file_id}/pages/{page_index}/image\n  method: get\n  operationId: get_public_file_page_image_api_v1_extract_files__file_id__pages__page_index__image_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/extract/agents/tools\n  method: get\n  operationId: list_agent_tools_api_v1_extract_agents_tools_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/extract/agents\n  method: post\n  operationId: create_agent_endpoint_api_v1_extract_agents_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/extract/jobs/{job_id}\n  method: get\n  operationId: get_job_api_v1_extract_jobs__job_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/extract/jobs/{job_id}/result\n  method: get\n  operationId: get_job_result_api_v1_extract_jobs__job_id__result_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/extract\n  method: post\n  operationId: extract_endpoint_api_v1_extract_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/upload\n  method: post\n  operationId: upload_public_files_api_v1_upload_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n   \
  \   triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/parse\n  method: post\n  operationId: parse_endpoint_api_v1_parse_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/layout\n  method: post\n  operationId: layout_endpoint_api_v1_layout_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/ocr\n  method: post\n  operationId: ocr_endpoint_api_v1_ocr_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/classify\n  method: post\n  operationId: classify_endpoint_api_v1_classify_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/split\n  method: post\n  operationId: split_endpoint_api_v1_split_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tables\n  method: post\n  operationId: tables_extract_endpoint_api_v1_tables_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/equations\n  method: post\n  operationId: equations_extract_endpoint_api_v1_equations_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/charts\n  method: post\n  operationId: charts_describe_endpoint_api_v1_charts_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/v1/autoschema\n  method: post\n  operationId: schema_auto_endpoint_api_v1_autoschema_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/compare\n  method: post\n  operationId: two_way_compare_endpoint_api_v1_compare_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/synthesize\n  method: post\n  operationId: synthesize_endpoint_api_v1_synthesize_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/synthesize/one\n  method: post\n  operationId: synthesize_endpoint_api_v1_synthesize_one_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/synthesize/set\n  method: post\n  operationId: synthesize_set_endpoint_api_v1_synthesize_set_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/ask\n  method: post\n\
  \  operationId: ask_endpoint_api_v1_ask_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/extract/files/{file_id}\n  method: get\n  operationId: get_public_file_api_v1_extract_files__file_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/extract/files/{file_id}/pages/{page_index}/image\n  method: get\n  operationId: get_public_file_page_image_api_v1_extract_files__file_id__pages__page_index__image_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/extract/agents/tools\n  method: get\n  operationId: list_agent_tools_api_v1_extract_agents_tools_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/extract/agents\n  method: post\n  operationId: create_agent_endpoint_api_v1_extract_agents_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/extract/jobs/{job_id}\n  method: get\n  operationId: get_job_api_v1_extract_jobs__job_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/extract/jobs/{job_id}/result\n  method: get\n  operationId: get_job_result_api_v1_extract_jobs__job_id__result_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/extract\n  method: post\n  operationId: extract_endpoint_api_v1_extract_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/upload\n  method: post\n  operationId: upload_public_files_api_v1_upload_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/parse\n  method: post\n  operationId: parse_endpoint_api_v1_parse_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/layout\n  method: post\n  operationId: layout_endpoint_api_v1_layout_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/ocr\n  method: post\n  operationId: ocr_endpoint_api_v1_ocr_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/classify\n  method: post\n  operationId: classify_endpoint_api_v1_classify_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/split\n  method: post\n  operationId: split_endpoint_api_v1_split_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tables\n  method: post\n  operationId: tables_extract_endpoint_api_v1_tables_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n \
  \   audit: required\n- path: /api/v1/equations\n  method: post\n  operationId: equations_extract_endpoint_api_v1_equations_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/charts\n  method: post\n  operationId: charts_describe_endpoint_api_v1_charts_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/autoschema\n  method: post\n  operationId: schema_auto_endpoint_api_v1_autoschema_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/compare\n  method: post\n  operationId: two_way_compare_endpoint_api_v1_compare_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/synthesize\n  method: post\n  operationId: synthesize_endpoint_api_v1_synthesize_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/synthesize/one\n  method: post\n  operationId: synthesize_endpoint_api_v1_synthesize_one_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/synthesize/set\n  method: post\n  operationId: synthesize_set_endpoint_api_v1_synthesize_set_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/ask\n  method: post\n  operationId: ask_endpoint_api_v1_ask_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n"
source_yaml_url: https://artifacts.apis.io/docspeed-ai/agentic-access/docspeed-ai-agentic-access.yml
summary_line: 44 operations · 34 acting
tags:
- AP Invoice Extraction
- BPO
- Shared Services
- Document AI
- Financial Services
- Procurement Automation
---
