---
acting_count: 0
action_class_counts:
  connected: 6
api_specs:
- filename: audito-lat-audit-api-openapi.yml
  format: yaml
  label: audito-lat Audit API
  slug: audito-lat-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audito-lat/openapi/audito-lat-audit-api-openapi.yml
- filename: audito-lat-deep-api-openapi.yml
  format: yaml
  label: audito-lat Deep API
  slug: audito-lat-deep-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audito-lat/openapi/audito-lat-deep-api-openapi.yml
- filename: audito-lat-report-api-openapi.yml
  format: yaml
  label: audito-lat Report API
  slug: audito-lat-report-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audito-lat/openapi/audito-lat-report-api-openapi.yml
consequence_counts:
  read: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Audito Lat Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'audito-lat exposes 6 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: audito-lat
provider_slug: audito-lat
slug: audito-lat-agentic-access
source_filename: audito-lat-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/agent-audito-lat-openapi.json, openapi/audito-lat-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 6\n  by_consequence:\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /report\n  method: get\n  operationId: reportSite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deep\n  method: get\n  operationId: deepAuditSite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /audit\n  method: get\n  operationId: auditSite\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /report\n  method: get\n  operationId: reportSite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deep\n  method: get\n  operationId: deepAuditSite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /audit\n  method: get\n  operationId: auditSite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/audito-lat/agentic-access/audito-lat-agentic-access.yml
summary_line: 6 operations
tags:
- Company
---
