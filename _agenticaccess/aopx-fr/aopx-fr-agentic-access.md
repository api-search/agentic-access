---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 3
api_specs:
- filename: aopx-fr-aopx-recommend-v0-api-openapi.yml
  format: yaml
  label: aopx-fr AOPX Recommend v0 API
  slug: aopx-fr-aopx-recommend-v0-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aopx-fr/openapi/aopx-fr-aopx-recommend-v0-api-openapi.yml
consequence_counts:
  read: 3
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Aopx Fr Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'aopx-fr exposes 5 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: aopx-fr
provider_slug: aopx-fr
slug: aopx-fr-agentic-access
source_filename: aopx-fr-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/aopx-fr-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 3\n    acting: 2\n  by_consequence:\n    read: 3\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/health\n  method: get\n  operationId: recommend_health_v1_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/recommend\n  method: post\n  operationId: recommend_v1_recommend_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/outcome\n  method: post\n  operationId: outcome_v1_outcome_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public/outcomes\n  method: get\n  operationId: public_outcomes_v1_public_outcomes_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public/stats\n  method: get\n  operationId: public_stats_v1_public_stats_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/aopx-fr/agentic-access/aopx-fr-agentic-access.yml
summary_line: 5 operations · 2 acting
tags:
- Search
- Artificial Intelligence
- Routing
- Benchmarks
- Evidence
---
