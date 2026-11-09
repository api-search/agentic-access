---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 5
api_specs:
- filename: claw-link-dev-discovery-api-openapi.yml
  format: yaml
  label: ClawLink Discovery API
  slug: claw-link-dev-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/claw-link-dev/openapi/claw-link-dev-discovery-api-openapi.yml
- filename: claw-link-dev-execution-api-openapi.yml
  format: yaml
  label: ClawLink Execution API
  slug: claw-link-dev-execution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/claw-link-dev/openapi/claw-link-dev-execution-api-openapi.yml
- filename: claw-link-dev-mcp-api-openapi.yml
  format: yaml
  label: ClawLink MCP API
  slug: claw-link-dev-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/claw-link-dev/openapi/claw-link-dev-mcp-api-openapi.yml
- filename: claw-link-dev-registration-api-openapi.yml
  format: yaml
  label: ClawLink Registration API
  slug: claw-link-dev-registration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/claw-link-dev/openapi/claw-link-dev-registration-api-openapi.yml
consequence_counts:
  read: 5
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Claw Link Dev Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'ClawLink exposes 10 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ClawLink
provider_slug: claw-link-dev
slug: claw-link-dev-agentic-access
source_filename: claw-link-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/claw-link-dev-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 5\n    acting: 5\n  by_consequence:\n    read: 5\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /api/tools\n  method: get\n  operationId: listTools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tools/search\n  method: get\n  operationId: searchTools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tools/{name}\n  method: get\n \
  \ operationId: describeTool\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tools/{name}/execute\n  method: post\n  operationId: executeTool\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp\n  method: get\n  operationId: describeMcpSurface\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - openid\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp\n  method: post\n  operationId: mcpJsonRpc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - openid\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/server-card\n  method: get\n  operationId: getMcpServerCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/openclaw/pair/start\n  method: post\n  operationId: startPairing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/openclaw/pair/sessions/{token}/exchange\n  method: post\n  operationId: exchangePairing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/hermes/bootstrap-sessions\n  method: post\n  operationId: createBootstrapSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/claw-link-dev/agentic-access/claw-link-dev-agentic-access.yml
summary_line: 10 operations · 5 acting
tags:
- Artificial Intelligence
- Integration
- Automation
- Productivity
- Developer Tools
---
