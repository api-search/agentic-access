---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 5
api_specs:
- filename: d-wave-account-api-openapi.yml
  format: yaml
  label: D-Wave Account API
  slug: d-wave-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-wave/refs/heads/main/openapi/d-wave-account-api-openapi.yml
- filename: d-wave-hybrid-api-openapi.yml
  format: yaml
  label: D-Wave Hybrid API
  slug: d-wave-hybrid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-wave/refs/heads/main/openapi/d-wave-hybrid-api-openapi.yml
- filename: d-wave-regions-api-openapi.yml
  format: yaml
  label: D-Wave Regions API
  slug: d-wave-regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-wave/refs/heads/main/openapi/d-wave-regions-api-openapi.yml
consequence_counts:
  read: 5
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: D Wave Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'D-Wave exposes 6 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: D-Wave
provider_slug: d-wave
slug: d-wave-agentic-access
source_filename: d-wave-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: generated\nsource: openapi/d-wave-account-api-openapi.yml, openapi/d-wave-hybrid-api-openapi.yml, openapi/d-wave-regions-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 5\n    acting: 1\n  by_consequence:\n    read: 5\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /account/active_project/oauth/\n  method: get\n  operationId: getActiveProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/projects/oauth/\n  method: get\n  operationId: listProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/token/oauth/\n  method: get\n  operationId: getProjectToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /problems/\n  method: post\n  operationId: submitHybridProblem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /regions/\n  method: get\n  operationId: listRegions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /regions/{code}\n  method: get\n  operationId: getRegion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/d-wave/refs/heads/main/agentic-access/d-wave-agentic-access.yml
summary_line: 6 operations · 1 acting
tags:
- Quantum Computing
- Quantum Annealing
- Optimization
- Hybrid Quantum-Classical
- Ising
- QUBO
- Industrial Optimization
- Sampling
- Leap
- Ocean SDK
- SAPI
---
