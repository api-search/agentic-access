---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 8
api_specs:
- filename: 4dayweek-io-4dayweek-io-public-api-api-openapi.yml
  format: yaml
  label: 4dayweek-io 4dayweek.io Public API
  slug: 4dayweek-io-4dayweek-io-public-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/4dayweek-io/openapi/4dayweek-io-4dayweek-io-public-api-api-openapi.yml
- filename: 4dayweek-io-jobs-api-openapi.yml
  format: yaml
  label: 4dayweek-io Jobs API
  slug: 4dayweek-io-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/4dayweek-io/openapi/4dayweek-io-jobs-api-openapi.yml
- filename: 4dayweek-io-mcp-api-openapi.yml
  format: yaml
  label: 4dayweek-io MCP API
  slug: 4dayweek-io-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/4dayweek-io/openapi/4dayweek-io-mcp-api-openapi.yml
consequence_counts:
  read: 8
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: 4Dayweek Io Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: '4dayweek-io exposes 10 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: 4dayweek-io
provider_slug: 4dayweek-io
slug: 4dayweek-io-agentic-access
source_filename: 4dayweek-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/4dayweek-io-openapi.yaml, openapi/4dayweek-io.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 8\n    acting: 2\n  by_consequence:\n    read: 8\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/jobs\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/jobs/{slug}\n  method: get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/jobs\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/jobs/{slug}\n  method: get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/4dayweek-io/agentic-access/4dayweek-io-agentic-access.yml
summary_line: 10 operations · 2 acting
tags:
- Remote Jobs
- Flexible Schedule
- Work-Life Balance
- Recruiting
---
