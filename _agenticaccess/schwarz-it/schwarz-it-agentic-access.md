---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 2
api_specs:
- filename: schwarz-it-health-probe-api-openapi.yml
  format: yaml
  label: Schwarz IT Health Probe API
  slug: schwarz-it-health-probe-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schwarz-it/refs/heads/main/openapi/schwarz-it-health-probe-api-openapi.yml
- filename: schwarz-it-lintings-api-openapi.yml
  format: yaml
  label: Schwarz IT Lintings API
  slug: schwarz-it-lintings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schwarz-it/refs/heads/main/openapi/schwarz-it-lintings-api-openapi.yml
- filename: schwarz-it-rules-api-openapi.yml
  format: yaml
  label: Schwarz IT Rules API
  slug: schwarz-it-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schwarz-it/refs/heads/main/openapi/schwarz-it-rules-api-openapi.yml
consequence_counts:
  read: 2
  safety-critical: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Schwarz It Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api-linting/api/v1/lintings
operation_count: 3
overview: 'Schwarz IT exposes 3 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Schwarz IT
provider_slug: schwarz-it
slug: schwarz-it-agentic-access
source_filename: schwarz-it-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: generated\nsource: openapi/schwarz-it-api-linter-service-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 3\n  by_action_class:\n    connected: 2\n    acting: 1\n  by_consequence:\n    read: 2\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /api-linting/api/v1/rules\n  method: get\n  operationId: RulesController_getCompanyApiRules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api-linting/api/v1/lintings\n  method: post\n  operationId: LintingsController_createLinting\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /.well-known/live\n  method: get\n  operationId: HealthProbeController_returnLive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/schwarz-it/refs/heads/main/agentic-access/schwarz-it-agentic-access.yml
summary_line: 3 operations · 1 acting · 1 human-in-the-loop
tags:
- Company
- API Governance
- API Linting
- Spectral
- OpenAPI
- Retail
- Germany
---
