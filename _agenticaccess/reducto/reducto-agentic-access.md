---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 3
api_specs:
- filename: reducto-cancel-api-openapi.yml
  format: yaml
  label: Reducto Cancel API
  slug: reducto-cancel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-cancel-api-openapi.yml
- filename: reducto-classify-api-openapi.yml
  format: yaml
  label: Reducto Classify API
  slug: reducto-classify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-classify-api-openapi.yml
- filename: reducto-configure-webhook-api-openapi.yml
  format: yaml
  label: Reducto Configure Webhook API
  slug: reducto-configure-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-configure-webhook-api-openapi.yml
- filename: reducto-edit-api-openapi.yml
  format: yaml
  label: Reducto Edit API
  slug: reducto-edit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-edit-api-openapi.yml
- filename: reducto-edit-async-api-openapi.yml
  format: yaml
  label: Reducto Edit Async API
  slug: reducto-edit-async-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-edit-async-api-openapi.yml
- filename: reducto-extract-api-openapi.yml
  format: yaml
  label: Reducto Extract API
  slug: reducto-extract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-extract-api-openapi.yml
- filename: reducto-extract-async-api-openapi.yml
  format: yaml
  label: Reducto Extract Async API
  slug: reducto-extract-async-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-extract-async-api-openapi.yml
- filename: reducto-job-api-openapi.yml
  format: yaml
  label: Reducto Job API
  slug: reducto-job-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-job-api-openapi.yml
- filename: reducto-jobs-api-openapi.yml
  format: yaml
  label: Reducto Jobs API
  slug: reducto-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-jobs-api-openapi.yml
- filename: reducto-parse-api-openapi.yml
  format: yaml
  label: Reducto Parse API
  slug: reducto-parse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-parse-api-openapi.yml
- filename: reducto-parse-async-api-openapi.yml
  format: yaml
  label: Reducto Parse Async API
  slug: reducto-parse-async-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-parse-async-api-openapi.yml
- filename: reducto-pipeline-api-openapi.yml
  format: yaml
  label: Reducto Pipeline API
  slug: reducto-pipeline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-pipeline-api-openapi.yml
- filename: reducto-pipeline-async-api-openapi.yml
  format: yaml
  label: Reducto Pipeline Async API
  slug: reducto-pipeline-async-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-pipeline-async-api-openapi.yml
- filename: reducto-split-api-openapi.yml
  format: yaml
  label: Reducto Split API
  slug: reducto-split-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-split-api-openapi.yml
- filename: reducto-split-async-api-openapi.yml
  format: yaml
  label: Reducto Split Async API
  slug: reducto-split-async-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-split-async-api-openapi.yml
- filename: reducto-upload-api-openapi.yml
  format: yaml
  label: Reducto Upload API
  slug: reducto-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-upload-api-openapi.yml
- filename: reducto-version-api-openapi.yml
  format: yaml
  label: Reducto Version API
  slug: reducto-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/openapi/reducto-version-api-openapi.yml
consequence_counts:
  read: 3
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Reducto Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'Reducto exposes 17 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 14 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Reducto
provider_slug: reducto
slug: reducto-agentic-access
source_filename: reducto-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/reducto-document-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    acting: 14\n    connected: 3\n  by_consequence:\n    write: 14\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /parse\n  method: post\n  operationId: parse_parse_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /parse_async\n  method: post\n  operationId: async_parse_parse_async_post\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /extract\n  method: post\n  operationId: extract_extract_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /extract_async\n  method: post\n  operationId: extract_async_extract_async_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /split\n  method: post\n  operationId:\
  \ split_split_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /split_async\n  method: post\n  operationId: split_async_split_async_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit\n  method: post\n  operationId: edit_edit_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /edit_async\n  method: post\n  operationId: edit_async_edit_async_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pipeline\n  method: post\n  operationId: pipeline_pipeline_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pipeline_async\n  method: post\n  operationId: pipeline_async_pipeline_async_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n    \
  \  triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /classify\n  method: post\n  operationId: classify_classify_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /job/{job_id}\n  method: get\n  operationId: retrieve_parse_job__job_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cancel/{job_id}\n  method: post\n  operationId: cancel_job_cancel__job_id__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /jobs\n  method: get\n  operationId: get_jobs_jobs_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /upload\n  method: post\n  operationId: upload_upload_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /configure_webhook\n  method: post\n  operationId: webhook_portal_configure_webhook_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /version\n  method: get\n  operationId:\
  \ get_version_version_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reducto/refs/heads/main/agentic-access/reducto-agentic-access.yml
summary_line: 17 operations · 14 acting
tags:
- Document Parsing
- PDF
- OCR
- Data Extraction
- AI
- Machine Learning
- Document Intelligence
- Structured Data
---
