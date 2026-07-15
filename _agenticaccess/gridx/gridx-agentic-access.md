---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 6
api_specs:
- filename: gridx-openapi.yml
  format: yaml
  label: GridX Rate Engine API
  slug: gridx-rate-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridx/refs/heads/main/openapi/gridx-openapi.yml
- filename: gridx-openapi.yml
  format: yaml
  label: GridX Bill Calculation API
  slug: gridx-bill-calculation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridx/refs/heads/main/openapi/gridx-openapi.yml
- filename: gridx-openapi.yml
  format: yaml
  label: GridX Rate Analytics API
  slug: gridx-rate-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridx/refs/heads/main/openapi/gridx-openapi.yml
- filename: gridx-openapi.yml
  format: yaml
  label: GridX OpenADR Programs API
  slug: gridx-openadr-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridx/refs/heads/main/openapi/gridx-openapi.yml
consequence_counts:
  read: 6
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Gridx Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'GridX exposes 8 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: GridX
provider_slug: gridx
slug: gridx-agentic-access
source_filename: gridx-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/gridx-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 6\n    acting: 2\n  by_consequence:\n    read: 6\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /token\n  method: get\n  operationId: getToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer/info\n  method: get\n  operationId: getCustomerInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer/usage\n  method: get\n  operationId: getCustomerUsage\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getPricing\n  method: get\n  operationId: getPricing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /programs\n  method: get\n  operationId: getPrograms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions\n  method: get\n  operationId: getSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions\n  method: post\n  operationId: createSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions\n  method: delete\n  operationId: deleteSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gridx/refs/heads/main/agentic-access/gridx-agentic-access.yml
summary_line: 8 operations · 2 acting
tags:
- Energy
- Utilities
- Rate Engine
- Billing
- Rate Analytics
---
