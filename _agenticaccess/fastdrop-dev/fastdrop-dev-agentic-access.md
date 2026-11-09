---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 6
api_specs:
- filename: fastdrop-dev-health-api-openapi.yml
  format: yaml
  label: FastDrop Health API
  slug: fastdrop-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fastdrop-dev/openapi/fastdrop-dev-health-api-openapi.yml
- filename: fastdrop-dev-mcp-api-openapi.yml
  format: yaml
  label: FastDrop MCP API
  slug: fastdrop-dev-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fastdrop-dev/openapi/fastdrop-dev-mcp-api-openapi.yml
- filename: fastdrop-dev-subregistry-api-openapi.yml
  format: yaml
  label: FastDrop Subregistry API
  slug: fastdrop-dev-subregistry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fastdrop-dev/openapi/fastdrop-dev-subregistry-api-openapi.yml
consequence_counts:
  read: 6
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Fastdrop Dev Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'FastDrop exposes 7 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: FastDrop
provider_slug: fastdrop-dev
slug: fastdrop-dev-agentic-access
source_filename: fastdrop-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: generated\nsource: openapi/fastdrop-dev-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    acting: 1\n    connected: 6\n  by_consequence:\n    write: 1\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /mcp\n  method: post\n  operationId: callMcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - mcp\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp\n  method: get\n  operationId: mcpGetInfo\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/servers\n  method: get\n  operationId: listServers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/servers/{serverName}/versions\n  method: get\n  operationId: listServerVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/servers/{serverName}/versions/{version}\n  method: get\n  operationId: getServerVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/health\n  method: get\n  operationId: getSubregistryHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/fastdrop-dev/agentic-access/fastdrop-dev-agentic-access.yml
summary_line: 7 operations · 1 acting
tags:
- launch-board
- MCP
- AI-agents
- software-discovery
- free-service
---
