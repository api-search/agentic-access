---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 6
api_specs:
- filename: nectar-hr-openapi.yml
  format: yaml
  label: Nectar Users API
  slug: nectar-hr-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nectar-hr/refs/heads/main/openapi/nectar-hr-openapi.yml
- filename: nectar-hr-openapi.yml
  format: yaml
  label: Nectar Recognition API
  slug: nectar-hr-recognition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nectar-hr/refs/heads/main/openapi/nectar-hr-openapi.yml
- filename: nectar-hr-openapi.yml
  format: yaml
  label: Nectar Custom Awards API
  slug: nectar-hr-custom-awards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nectar-hr/refs/heads/main/openapi/nectar-hr-openapi.yml
- filename: nectar-hr-openapi.yml
  format: yaml
  label: Nectar Financial Analytics API
  slug: nectar-hr-financial-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nectar-hr/refs/heads/main/openapi/nectar-hr-openapi.yml
- filename: nectar-hr-openapi.yml
  format: yaml
  label: Nectar Flows API
  slug: nectar-hr-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nectar-hr/refs/heads/main/openapi/nectar-hr-openapi.yml
consequence_counts:
  physical: 1
  read: 6
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Nectar Hr Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/custom-awards/send
operation_count: 9
overview: 'Nectar exposes 9 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 2 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Nectar
provider_slug: nectar-hr
slug: nectar-hr-agentic-access
source_filename: nectar-hr-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/nectar-hr-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 6\n    acting: 3\n  by_consequence:\n    read: 6\n    physical: 1\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/analytics/financial/redemptions\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/custom-awards\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/custom-awards/send\n  method: post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/flows/trigger/{triggerId}\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /health\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/recognition/feed\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n- path: /v1/users/{userId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nectar-hr/refs/heads/main/agentic-access/nectar-hr-agentic-access.yml
summary_line: 9 operations · 3 acting
tags:
- Employee Recognition
- Rewards
- Points
- HR
- Employee Engagement
- Culture
- People Operations
---
