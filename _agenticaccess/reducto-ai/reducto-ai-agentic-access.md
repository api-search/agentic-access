---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 7
api_specs:
- filename: reducto-ai-classify-api-openapi.yml
  format: yaml
  label: reducto-ai Classify API
  slug: reducto-ai-classify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-ai-classify-api-openapi.yml
- filename: reducto-ai-edit-api-openapi.yml
  format: yaml
  label: reducto-ai Edit API
  slug: reducto-ai-edit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-ai-edit-api-openapi.yml
- filename: reducto-ai-extract-api-openapi.yml
  format: yaml
  label: reducto-ai Extract API
  slug: reducto-ai-extract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-ai-extract-api-openapi.yml
- filename: reducto-ai-jobs-api-openapi.yml
  format: yaml
  label: reducto-ai Jobs API
  slug: reducto-ai-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-ai-jobs-api-openapi.yml
- filename: reducto-ai-parse-api-openapi.yml
  format: yaml
  label: reducto-ai Parse API
  slug: reducto-ai-parse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-ai-parse-api-openapi.yml
- filename: reducto-ai-pipeline-api-openapi.yml
  format: yaml
  label: reducto-ai Pipeline API
  slug: reducto-ai-pipeline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-ai-pipeline-api-openapi.yml
- filename: reducto-ai-platform-api-openapi.yml
  format: yaml
  label: reducto-ai Platform API
  slug: reducto-ai-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-ai-platform-api-openapi.yml
- filename: reducto-ai-split-api-openapi.yml
  format: yaml
  label: reducto-ai Split API
  slug: reducto-ai-split-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-ai-split-api-openapi.yml
- filename: reducto-ai-upload-api-openapi.yml
  format: yaml
  label: reducto-ai Upload API
  slug: reducto-ai-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-ai-upload-api-openapi.yml
- filename: reducto-ai-webhooks-api-openapi.yml
  format: yaml
  label: reducto-ai Webhooks API
  slug: reducto-ai-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/openapi/reducto-ai-webhooks-api-openapi.yml
consequence_counts:
  read: 7
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Reducto Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 22
overview: 'Reducto exposes 22 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 15 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Reducto
provider_slug: reducto-ai
slug: reducto-ai-agentic-access
source_filename: reducto-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/reducto-classify-api-openapi.yml, openapi/reducto-edit-api-openapi.yml, openapi/reducto-extract-api-openapi.yml,\n  openapi/reducto-jobs-api-openapi.yml, openapi/reducto-parse-api-openapi.yml, openapi/reducto-pipeline-api-openapi.yml,\n  openapi/reducto-platform-api-openapi.yml, openapi/reducto-split-api-openapi.yml, openapi/reducto-upload-api-openapi.yml,\n  openapi/reducto-webhooks-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    acting: 15\n    connected: 7\n  by_consequence:\n    write: 15\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /classify\n  method: post\n  operationId: classify_classify_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cite\n  method: post\n  operationId: cite_cite_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit\n  method: post\n  operationId: edit_edit_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit_async\n  method: post\n  operationId: edit_async_edit_async_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /extract\n  method: post\n  operationId: extract_extract_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /extract_async\n  method: post\n  operationId: extract_async_extract_async_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /job/{job_id}\n  method: get\n  operationId: retrieve_parse_job__job_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cancel/{job_id}\n  method: post\n  operationId: cancel_job_cancel__job_id__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs\n  method: get\n  operationId: get_jobs_jobs_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /parse\n  method: post\n  operationId: parse_parse_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n     \
  \ max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /parse_async\n  method: post\n  operationId: async_parse_parse_async_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pipeline\n  method: post\n  operationId: pipeline_pipeline_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pipeline_async\n  method: post\n  operationId: pipeline_async_pipeline_async_post\n  x-agentic-access:\n    action-class: acting\n  \
  \  consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /health\n  method: get\n  operationId: health_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /version\n  method: get\n  operationId: get_version_version_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /prometheus\n  method: get\n  operationId: prometheus_metrics_prometheus_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics\n  method: get\n  operationId: metrics_metrics_get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /streaq_metrics\n  method: get\n  operationId: streaq_metrics_streaq_metrics_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /split\n  method: post\n  operationId: split_split_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /split_async\n  method: post\n  operationId: split_async_split_async_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /upload\n  method: post\n  operationId: upload_upload_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /configure_webhook\n  method: post\n  operationId: webhook_portal_configure_webhook_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reducto-ai/refs/heads/main/agentic-access/reducto-ai-agentic-access.yml
summary_line: 22 operations · 15 acting
tags: []
---
