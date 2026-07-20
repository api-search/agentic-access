---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 5
api_specs:
- filename: allium-openapi-original.json
  format: json
  label: Allium Realtime API
  slug: allium-realtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allium/refs/heads/main/openapi/allium-openapi-original.json
consequence_counts:
  read: 5
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Allium Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Allium exposes 8 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Allium
provider_slug: allium
slug: allium-agentic-access
source_filename: allium-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: generated\nsource: openapi/allium-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 3\n    connected: 5\n  by_consequence:\n    write: 3\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/explorer/queries/{query_id}/run\n  method: post\n  operationId: execute_query_api_v1_explorer_queries__query_id__run_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/explorer/queries/{query_id}/run-async\n\
  \  method: post\n  operationId: execute_query_async_api_v1_explorer_queries__query_id__run_async_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/explorer/query-runs\n  method: get\n  operationId: get_latest_query_run_handler_api_v1_explorer_query_runs_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/explorer/query-runs/{run_id}/status\n  method: get\n  operationId: get_query_run_status_api_v1_explorer_query_runs__run_id__status_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/explorer/query-runs/{run_id}/results\n\
  \  method: get\n  operationId: get_query_run_results_api_v1_explorer_query_runs__run_id__results_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/explorer/query-runs/{run_id}/cancel\n  method: post\n  operationId: cancel_query_run_api_v1_explorer_query_runs__run_id__cancel_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/polygon/nfts/\n  method: get\n  operationId: get_polygon_nfts_api_v1_polygon_nfts__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ping\n  method: get\n  operationId: ping_ping_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allium/refs/heads/main/agentic-access/allium-agentic-access.yml
summary_line: 8 operations · 3 acting
tags:
- Company
- Data Analytics
- Blockchain
- Crypto
- Web3
- Data Infrastructure
- Real-Time Data
- Stablecoins
- DeFi
- Machine Payments
---
