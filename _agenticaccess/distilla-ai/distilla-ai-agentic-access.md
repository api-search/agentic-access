---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 10
api_specs:
- filename: distilla-ai-health-api-openapi.yml
  format: yaml
  label: Distilla AI Health API
  slug: distilla-ai-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/distilla-ai/openapi/distilla-ai-health-api-openapi.yml
- filename: distilla-ai-internal-api-openapi.yml
  format: yaml
  label: Distilla AI Internal API
  slug: distilla-ai-internal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/distilla-ai/openapi/distilla-ai-internal-api-openapi.yml
- filename: distilla-ai-mcp-api-openapi.yml
  format: yaml
  label: Distilla AI MCP API
  slug: distilla-ai-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/distilla-ai/openapi/distilla-ai-mcp-api-openapi.yml
- filename: distilla-ai-tools-api-openapi.yml
  format: yaml
  label: Distilla AI Tools API
  slug: distilla-ai-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/distilla-ai/openapi/distilla-ai-tools-api-openapi.yml
- filename: distilla-ai-well-known-api-openapi.yml
  format: yaml
  label: Distilla AI .well Known API
  slug: distilla-ai-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/distilla-ai/openapi/distilla-ai-well-known-api-openapi.yml
consequence_counts:
  read: 10
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Distilla Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Distilla AI exposes 12 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Distilla AI
provider_slug: distilla-ai
slug: distilla-ai-agentic-access
source_filename: distilla-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/distilla-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 10\n    acting: 2\n  by_consequence:\n    read: 10\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /health\n  method: get\n  operationId: health_check_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tools/{tool_name}\n  method: post\n  operationId: call_http_tool_tools__tool_name__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /internal/mcp-usage\n  method: get\n  operationId: get_mcp_usage_internal_mcp_usage_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /internal/screen-jobs/{job_id}/run\n  method: post\n  operationId: run_internal_screen_job_internal_screen_jobs__job_id__run_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /.well-known/oauth-protected-resource/mcp\n  method: get\n  operationId: oauth_protected_resource__well_known_oauth_protected_resource_mcp_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/oauth-protected-resource/mcp\n  method: options\n  operationId: oauth_metadata_options__well_known_oauth_protected_resource_mcp_options\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/oauth-protected-resource\n  method: get\n  operationId: oauth_protected_resource__well_known_oauth_protected_resource_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/oauth-protected-resource\n  method: options\n  operationId: oauth_metadata_options__well_known_oauth_protected_resource_options\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/oauth-authorization-server\n\
  \  method: get\n  operationId: oauth_authorization_server__well_known_oauth_authorization_server_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/oauth-authorization-server\n  method: options\n  operationId: oauth_metadata_options__well_known_oauth_authorization_server_options\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/openai-apps-challenge\n  method: get\n  operationId: openai_apps_challenge__well_known_openai_apps_challenge_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp\n  method: get\n  operationId: mcp_get_sse_mcp_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/distilla-ai/agentic-access/distilla-ai-agentic-access.yml
summary_line: 12 operations · 2 acting
tags:
- Artificial Intelligence
- Finance
- Equity Research
- Stock Market
- Investment
---
