---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 12
api_specs:
- filename: d-wave-solvers-api-openapi.yml
  format: yaml
  label: D-Wave Solver API (SAPI) - Solvers
  slug: d-wave-solver-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-wave/refs/heads/main/openapi/d-wave-solvers-api-openapi.yml
- filename: d-wave-problems-api-openapi.yml
  format: yaml
  label: D-Wave Solver API (SAPI) - Problems
  slug: d-wave-problems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-wave/refs/heads/main/openapi/d-wave-problems-api-openapi.yml
- filename: d-wave-metadata-api-openapi.yml
  format: yaml
  label: D-Wave Metadata API - Regions
  slug: d-wave-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-wave/refs/heads/main/openapi/d-wave-metadata-api-openapi.yml
- filename: d-wave-leap-account-api-openapi.yml
  format: yaml
  label: D-Wave Leap Account API
  slug: d-wave-leap-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-wave/refs/heads/main/openapi/d-wave-leap-account-api-openapi.yml
- filename: d-wave-hybrid-solvers-openapi.yml
  format: yaml
  label: D-Wave Leap Hybrid Solvers
  slug: d-wave-hybrid-solvers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-wave/refs/heads/main/openapi/d-wave-hybrid-solvers-openapi.yml
- filename: d-wave-qpu-samplers-openapi.yml
  format: yaml
  label: D-Wave QPU Samplers (Advantage / Advantage2)
  slug: d-wave-qpu-samplers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-wave/refs/heads/main/openapi/d-wave-qpu-samplers-openapi.yml
consequence_counts:
  read: 12
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: D Wave Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'D-Wave exposes 17 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: D-Wave
provider_slug: d-wave
slug: d-wave-agentic-access
source_filename: d-wave-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/d-wave-hybrid-solvers-openapi.yml, openapi/d-wave-leap-account-api-openapi.yml,\n  openapi/d-wave-metadata-api-openapi.yml, openapi/d-wave-problems-api-openapi.yml, openapi/d-wave-qpu-samplers-openapi.yml,\n  openapi/d-wave-solvers-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    acting: 5\n    connected: 12\n  by_consequence:\n    write: 5\n    read: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /problems/\n  method: post\n  operationId: submitHybridProblem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/active_project/oauth/\n  method: get\n  operationId: getActiveProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/projects/oauth/\n  method: get\n  operationId: listProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/token/oauth/\n  method: get\n  operationId: getProjectToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /regions/\n  method: get\n  operationId: listRegions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /regions/{code}\n\
  \  method: get\n  operationId: getRegion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /problems/\n  method: get\n  operationId: listProblems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /problems/\n  method: post\n  operationId: submitProblem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /problems/\n  method: delete\n  operationId: cancelProblems\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /problems/{problem_id}\n  method: get\n  operationId: getProblem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /problems/{problem_id}\n  method: delete\n  operationId: cancelProblem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /problems/{problem_id}/info\n  method: get\n  operationId: getProblemInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /problems/{problem_id}/answer\n  method: get\n  operationId: getProblemAnswer\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /problems/{problem_id}/messages\n  method: get\n  operationId: getProblemMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /problems/\n  method: post\n  operationId: submitQpuProblem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /solvers/remote/\n  method: get\n  operationId: listSolvers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /solvers/remote/{solver_name}\n  method: get\n  operationId: getSolver\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/d-wave/refs/heads/main/agentic-access/d-wave-agentic-access.yml
summary_line: 17 operations · 5 acting
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
