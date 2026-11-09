---
acting_count: 0
action_class_counts:
  connected: 7
api_specs:
- filename: filings-tools-account-api-openapi.yml
  format: yaml
  label: filings.tools Account API
  slug: filings-tools-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filings-tools/openapi/filings-tools-account-api-openapi.yml
- filename: filings-tools-filings-api-openapi.yml
  format: yaml
  label: filings.tools Filings API
  slug: filings-tools-filings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filings-tools/openapi/filings-tools-filings-api-openapi.yml
consequence_counts:
  read: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Filings Tools Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'filings.tools exposes 7 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: filings.tools
provider_slug: filings-tools
slug: filings-tools-agentic-access
source_filename: filings-tools-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: generated\nsource: openapi/filings-tools-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 7\n  by_consequence:\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/filings\n  method: get\n  operationId: listFilings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/filings/{id}/sections\n  method: get\n  operationId: getFilingSections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/filings/{id}/facts\n  method: get\n\
  \  operationId: getFilingFacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/filings/{id}/diff\n  method: get\n  operationId: compareFiling\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/filings/{id}/tables\n  method: get\n  operationId: getFilingTables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sections\n  method: get\n  operationId: getSectionAcrossCompanies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/me\n  method: get\n  operationId: getStanding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/filings-tools/agentic-access/filings-tools-agentic-access.yml
summary_line: 7 operations
tags:
- SEC Filings
- 10-K
- 10-Q
- 8-K
- Risk Factors
- Financial Documents
- Diff
- MCP
- Developer API
---
