---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 5
api_specs:
- filename: findefend-com-alerts-api-openapi.yml
  format: yaml
  label: FinDefend Alerts API
  slug: findefend-com-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findefend-com/openapi/findefend-com-alerts-api-openapi.yml
- filename: findefend-com-export-api-openapi.yml
  format: yaml
  label: FinDefend Export API
  slug: findefend-com-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findefend-com/openapi/findefend-com-export-api-openapi.yml
- filename: findefend-com-health-api-openapi.yml
  format: yaml
  label: FinDefend Health API
  slug: findefend-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findefend-com/openapi/findefend-com-health-api-openapi.yml
- filename: findefend-com-summary-api-openapi.yml
  format: yaml
  label: FinDefend Summary API
  slug: findefend-com-summary-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findefend-com/openapi/findefend-com-summary-api-openapi.yml
- filename: findefend-com-vendors-api-openapi.yml
  format: yaml
  label: FinDefend Vendors API
  slug: findefend-com-vendors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findefend-com/openapi/findefend-com-vendors-api-openapi.yml
consequence_counts:
  read: 5
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Findefend Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'FinDefend exposes 7 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: FinDefend
provider_slug: findefend-com
slug: findefend-com-agentic-access
source_filename: findefend-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: generated\nsource: openapi/findefend-com-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 5\n    acting: 2\n  by_consequence:\n    read: 5\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /health\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/vendors\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/vendors/{id}\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/alerts\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/alerts/{id}/acknowledge\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/summary\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/export\n  method: get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/findefend-com/agentic-access/findefend-com-agentic-access.yml
summary_line: 7 operations · 2 acting
tags:
- FinTech
- SaaS
- SubscriptionManagement
- ExpenseTracking
- Automation
---
