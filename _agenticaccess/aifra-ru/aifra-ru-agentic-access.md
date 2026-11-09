---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 6
api_specs:
- filename: aifra-ru-analytics-api-openapi.yml
  format: yaml
  label: AIfra Analytics API
  slug: aifra-ru-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aifra-ru/openapi/aifra-ru-analytics-api-openapi.yml
- filename: aifra-ru-health-api-openapi.yml
  format: yaml
  label: AIfra Health API
  slug: aifra-ru-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aifra-ru/openapi/aifra-ru-health-api-openapi.yml
- filename: aifra-ru-mcp-api-openapi.yml
  format: yaml
  label: AIfra MCP API
  slug: aifra-ru-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aifra-ru/openapi/aifra-ru-mcp-api-openapi.yml
- filename: aifra-ru-previews-api-openapi.yml
  format: yaml
  label: AIfra Previews API
  slug: aifra-ru-previews-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aifra-ru/openapi/aifra-ru-previews-api-openapi.yml
- filename: aifra-ru-ready-api-openapi.yml
  format: yaml
  label: AIfra Ready API
  slug: aifra-ru-ready-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aifra-ru/openapi/aifra-ru-ready-api-openapi.yml
- filename: aifra-ru-remote-api-openapi.yml
  format: yaml
  label: AIfra Remote API
  slug: aifra-ru-remote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aifra-ru/openapi/aifra-ru-remote-api-openapi.yml
consequence_counts:
  read: 6
  safety-critical: 1
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Aifra Ru Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/analytics
operation_count: 12
overview: 'AIfra exposes 12 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 5 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AIfra
provider_slug: aifra-ru
slug: aifra-ru-agentic-access
source_filename: aifra-ru-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/aifra-ru-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    acting: 6\n    connected: 6\n  by_consequence:\n    safety-critical: 1\n    read: 6\n    write: 5\n  human_in_the_loop_required: 1\noperations:\n- path: /v1/analytics\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/health\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ready\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/previews\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/previews/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/previews/{id}\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/previews/{id}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /remote/aliases/{alias}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /remote/session\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /remote/operations/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /remote/operations/{id}/confirm\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/aifra-ru/agentic-access/aifra-ru-agentic-access.yml
summary_line: 12 operations · 6 acting · 1 human-in-the-loop
tags:
- Software-as-a-Service
- Static-Previews
- Artificial Intelligence
- CLI
- REST
---
