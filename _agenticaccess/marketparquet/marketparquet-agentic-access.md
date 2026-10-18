---
acting_count: 0
action_class_counts:
  connected: 4
api_specs:
- filename: marketparquet-api-v1-api-openapi.yml
  format: yaml
  label: MarketParquet API V1 API
  slug: marketparquet-api-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketparquet/refs/heads/main/openapi/marketparquet-api-v1-api-openapi.yml
consequence_counts:
  read: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Marketparquet Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 4
overview: 'MarketParquet exposes 4 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: MarketParquet
provider_slug: marketparquet
slug: marketparquet-agentic-access
source_filename: marketparquet-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: generated\nsource: openapi/marketparquet-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    connected: 4\n  by_consequence:\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/assets\n  method: get\n  operationId: list_assets_api_v1_assets_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/dates/{asset_type}\n  method: get\n  operationId: list_dates_api_v1_dates__asset_type__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/download/{asset_type}/{date_str}\n\
  \  method: get\n  operationId: download_file_api_v1_download__asset_type___date_str__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/manifest/{asset_type}\n  method: get\n  operationId: download_manifest_api_v1_manifest__asset_type__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marketparquet/refs/heads/main/agentic-access/marketparquet-agentic-access.yml
summary_line: 4 operations
tags:
- Company
- Finance
- Data
- MarketData
- APIs
---
