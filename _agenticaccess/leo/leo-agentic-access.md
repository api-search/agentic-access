---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 6
api_specs:
- filename: leo-prospects-api-openapi.yml
  format: yaml
  label: LeO Public API
  slug: leo-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leo/refs/heads/main/openapi/leo-prospects-api-openapi.yml
- filename: leo-health-api-openapi.yml
  format: yaml
  label: LeO Health API
  slug: leo-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leo/refs/heads/main/openapi/leo-health-api-openapi.yml
consequence_counts:
  read: 6
  safety-critical: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Leo Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/prospects/enrich
operation_count: 7
overview: 'LeO exposes 7 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: LeO
provider_slug: leo
slug: leo-agentic-access
source_filename: leo-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: generated\nsource: openapi/leo-account-api-openapi.yml, openapi/leo-credits-api-openapi.yml, openapi/leo-health-api-openapi.yml,\n  openapi/leo-jobs-api-openapi.yml, openapi/leo-prospects-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 6\n    acting: 1\n  by_consequence:\n    read: 6\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /v1/account\n  method: get\n  operationId: AccountController_getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/credits/balance\n  method: get\n  operationId: CreditsController_getCreditBalance\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: AppController_health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/{taskId}\n  method: get\n  operationId: JobsController_getJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/prospects/search\n  method: post\n  operationId: ProspectsController_search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/prospects/{prospectId}\n  method: get\n  operationId: ProspectsController_getById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/prospects/enrich\n  method: post\n  operationId: ProspectsController_enrich\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leo/refs/heads/main/agentic-access/leo-agentic-access.yml
summary_line: 7 operations · 1 acting · 1 human-in-the-loop
tags:
- Company
- Insurance
- Commercial Insurance
- Property and Casualty
- Employee Benefits
- Insurtech
- Artificial Intelligence
- Sales
- Lead Generation
- Prospecting
- Data Enrichment
- Sales Intelligence
- Non-Profit
- Trucking
- MCP
- Agent-Native
---
