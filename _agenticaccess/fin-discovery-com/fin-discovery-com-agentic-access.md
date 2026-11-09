---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 4
api_specs:
- filename: fin-discovery-com-call-tool-api-openapi.yml
  format: yaml
  label: Fintel Discovery Call Tool API
  slug: fin-discovery-com-call-tool-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fin-discovery-com/openapi/fin-discovery-com-call-tool-api-openapi.yml
- filename: fin-discovery-com-fastapi-api-openapi.yml
  format: yaml
  label: Fintel Discovery Fast API
  slug: fin-discovery-com-fastapi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fin-discovery-com/openapi/fin-discovery-com-fastapi-api-openapi.yml
- filename: fin-discovery-com-getatoken-api-openapi.yml
  format: yaml
  label: Fintel Discovery Get A Token API
  slug: fin-discovery-com-getatoken-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fin-discovery-com/openapi/fin-discovery-com-getatoken-api-openapi.yml
- filename: fin-discovery-com-login-api-openapi.yml
  format: yaml
  label: Fintel Discovery Login API
  slug: fin-discovery-com-login-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fin-discovery-com/openapi/fin-discovery-com-login-api-openapi.yml
- filename: fin-discovery-com-tool-endpoint-api-openapi.yml
  format: yaml
  label: Fintel Discovery Tool Endpoint API
  slug: fin-discovery-com-tool-endpoint-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fin-discovery-com/openapi/fin-discovery-com-tool-endpoint-api-openapi.yml
consequence_counts:
  read: 4
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Fin Discovery Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Fintel Discovery exposes 5 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Fintel Discovery
provider_slug: fin-discovery-com
slug: fin-discovery-com-agentic-access
source_filename: fin-discovery-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: generated\nsource: openapi/fin-discovery-com-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 4\n    acting: 1\n  by_consequence:\n    read: 4\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: root__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /login\n  method: get\n  operationId: login_login_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getAToken\n  method: get\n  operationId: authorized_getAToken_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tool-endpoint\n  method: get\n  operationId: tool_endpoint_tool_endpoint_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /call-tool/{tool_name}\n  method: post\n  operationId: call_tool_call_tool__tool_name__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/fin-discovery-com/agentic-access/fin-discovery-com-agentic-access.yml
summary_line: 5 operations · 1 acting
tags:
- Financial Services
- Regulatory Data
- Broker Check
- SEC EDGAR
- Market Data
- MCP Server
- AI Agents
- Compliance
---
