---
acting_count: 0
action_class_counts:
  connected: 7
api_specs:
- filename: gatiflow-openapi.yml
  format: yaml
  label: GatiFlow Intelligence API
  slug: gatiflow-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gatiflow/refs/heads/main/openapi/gatiflow-openapi.yml
consequence_counts:
  read: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Gatiflow Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'GatiFlow exposes 7 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: GatiFlow
provider_slug: gatiflow
slug: gatiflow-agentic-access
source_filename: gatiflow-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-21'\nmethod: generated\nsource: openapi/gatiflow-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 7\n  by_consequence:\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/intelligence/report\n  method: get\n  operationId: report_api_v1_intelligence_report_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/intelligence/report-history\n  method: get\n  operationId: report_history_list_api_v1_intelligence_report_history_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/v1/intelligence/report/at/{snapshot_id}\n  method: get\n  operationId: report_at_snapshot_api_v1_intelligence_report_at__snapshot_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/intelligence/report/export\n  method: get\n  operationId: export_report_api_v1_intelligence_report_export_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/public/deep-dive\n  method: get\n  operationId: get_latest_deep_dive_api_v1_public_deep_dive_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/public/weekly-report\n  method: get\n  operationId: weekly_report_api_v1_public_weekly_report_get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/usage\n  method: get\n  operationId: get_my_usage_api_v1_usage_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gatiflow/refs/heads/main/agentic-access/gatiflow-agentic-access.yml
summary_line: 7 operations
tags:
- Market Intelligence
- Developer Signals
- Trends
- Hiring
- Open-Source
- Research
- B2B SaaS
- Artificial Intelligence
---
