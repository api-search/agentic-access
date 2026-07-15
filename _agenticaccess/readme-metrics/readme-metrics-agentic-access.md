---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 4
api_specs:
- filename: 6733983cabaf62002c7b16d9
  format: yaml
  label: ReadMe API
  slug: readme-api
  spec_type: OpenAPI
  url: https://spec.readme.com/openapi/6733983cabaf62002c7b16d9
- filename: readme-metrics-openapi.yml
  format: yaml
  label: ReadMe Metrics
  slug: readme-metrics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/readme-metrics/refs/heads/main/openapi/readme-metrics-openapi.yml
consequence_counts:
  read: 4
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Readme Metrics Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'ReadMe Metrics exposes 5 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ReadMe Metrics
provider_slug: readme-metrics
slug: readme-metrics-agentic-access
source_filename: readme-metrics-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/readme-metrics-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 4\n    acting: 1\n  by_consequence:\n    read: 4\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api-specification\n  method: get\n  operationId: getAPISpecifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api-specification\n  method: post\n  operationId: uploadAPISpecification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api-registry/{uuid}\n  method: get\n  operationId: getAPIRegistry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /changelogs\n  method: get\n  operationId: getChangelogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /docs/{slug}\n  method: get\n  operationId: getDoc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/readme-metrics/refs/heads/main/agentic-access/readme-metrics-agentic-access.yml
summary_line: 5 operations · 1 acting
tags:
- API Analytics
- API Documentation
- API Logs
- API Metrics
- API Usage
- Developer Experience
- Developer Hubs
---
