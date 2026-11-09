---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 7
api_specs:
- filename: toolaby-app-analytics-api-openapi.yml
  format: yaml
  label: toolaby-app Analytics API
  slug: toolaby-app-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/toolaby-app/openapi/toolaby-app-analytics-api-openapi.yml
- filename: toolaby-app-customers-api-openapi.yml
  format: yaml
  label: toolaby-app Customers API
  slug: toolaby-app-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/toolaby-app/openapi/toolaby-app-customers-api-openapi.yml
- filename: toolaby-app-grants-api-openapi.yml
  format: yaml
  label: toolaby-app Grants API
  slug: toolaby-app-grants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/toolaby-app/openapi/toolaby-app-grants-api-openapi.yml
- filename: toolaby-app-uses-api-openapi.yml
  format: yaml
  label: toolaby-app Uses API
  slug: toolaby-app-uses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/toolaby-app/openapi/toolaby-app-uses-api-openapi.yml
consequence_counts:
  read: 7
  safety-critical: 1
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Toolaby App Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/tools/{slug}/grants/{id}
operation_count: 9
overview: 'toolaby-app exposes 9 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read, 1 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: toolaby-app
provider_slug: toolaby-app
slug: toolaby-app-agentic-access
source_filename: toolaby-app-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/toolaby-app-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 7\n    acting: 2\n  by_consequence:\n    read: 7\n    write: 1\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /api/v1/tools/{slug}/customers\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tools/{slug}/customers/{email}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tools/{slug}/grants\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tools/{slug}/grants\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/{slug}/grants/{id}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/tools/{slug}/analytics\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tools/{slug}/analytics/{table}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tools/{slug}/uses\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tools/{slug}/uses\n  method: post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/toolaby-app/agentic-access/toolaby-app-agentic-access.yml
summary_line: 9 operations · 2 acting · 1 human-in-the-loop
tags:
- Company
- Payments
- Chrome Extension
- Stripe
- Licensing
---
