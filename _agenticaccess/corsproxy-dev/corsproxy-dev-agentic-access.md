---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 3
api_specs:
- filename: corsproxy-dev-health-api-openapi.yml
  format: yaml
  label: corsproxy-dev Health API
  slug: corsproxy-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corsproxy-dev/openapi/corsproxy-dev-health-api-openapi.yml
- filename: corsproxy-dev-mcp-api-openapi.yml
  format: yaml
  label: corsproxy-dev MCP API
  slug: corsproxy-dev-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corsproxy-dev/openapi/corsproxy-dev-mcp-api-openapi.yml
- filename: corsproxy-dev-proxy-api-openapi.yml
  format: yaml
  label: corsproxy-dev Proxy API
  slug: corsproxy-dev-proxy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corsproxy-dev/openapi/corsproxy-dev-proxy-api-openapi.yml
consequence_counts:
  read: 3
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Corsproxy Dev Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'corsproxy-dev exposes 6 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: corsproxy-dev
provider_slug: corsproxy-dev
slug: corsproxy-dev-agentic-access
source_filename: corsproxy-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/corsproxy-dev-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 3\n    acting: 3\n  by_consequence:\n    read: 3\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/health\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /proxy\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /proxy\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/proxy\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/proxy\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/corsproxy-dev/agentic-access/corsproxy-dev-agentic-access.yml
summary_line: 6 operations · 3 acting
tags:
- Company
- CORS
- Proxy
- Developer Tools
- Open Source
---
