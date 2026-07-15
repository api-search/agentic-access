---
acting_count: 14
action_class_counts:
  acting: 14
api_specs:
- filename: depot-dev-openapi.yml
  format: yaml
  label: Depot Project API
  slug: depot-dev-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/depot-dev/refs/heads/main/openapi/depot-dev-openapi.yml
- filename: depot-dev-openapi.yml
  format: yaml
  label: Depot Build API
  slug: depot-dev-build-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/depot-dev/refs/heads/main/openapi/depot-dev-openapi.yml
- filename: depot-dev-openapi.yml
  format: yaml
  label: Depot BuildKit API
  slug: depot-dev-buildkit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/depot-dev/refs/heads/main/openapi/depot-dev-openapi.yml
- filename: depot-dev-openapi.yml
  format: yaml
  label: Depot Tokens API
  slug: depot-dev-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/depot-dev/refs/heads/main/openapi/depot-dev-openapi.yml
consequence_counts:
  safety-critical: 1
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Depot Dev Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /depot.core.v1.ProjectService/ResetProjectCache
operation_count: 14
overview: 'Depot exposes 14 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 write and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Depot
provider_slug: depot-dev
slug: depot-dev-agentic-access
source_filename: depot-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/depot-dev-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    acting: 14\n  by_consequence:\n    write: 13\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /depot.core.v1.ProjectService/ListProjects\n  method: post\n  operationId: listProjects\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /depot.core.v1.ProjectService/CreateProject\n  method: post\n  operationId: createProject\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /depot.core.v1.ProjectService/GetProject\n  method: post\n  operationId: getProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /depot.core.v1.ProjectService/UpdateProject\n  method: post\n  operationId: updateProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /depot.core.v1.ProjectService/DeleteProject\n  method: post\n  operationId: deleteProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /depot.core.v1.ProjectService/ResetProjectCache\n  method: post\n  operationId: resetProjectCache\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /depot.core.v1.ProjectService/ListProjectTokens\n  method: post\n  operationId: listProjectTokens\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n \
  \   audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /depot.core.v1.ProjectService/CreateProjectToken\n  method: post\n  operationId: createProjectToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /depot.core.v1.ProjectService/DeleteProjectToken\n  method: post\n  operationId: deleteProjectToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /depot.build.v1.BuildService/CreateBuild\n\
  \  method: post\n  operationId: createBuild\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /depot.build.v1.BuildService/FinishBuild\n  method: post\n  operationId: finishBuild\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /depot.build.v1.BuildService/GetBuild\n  method: post\n  operationId: getBuild\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /depot.build.v1.BuildService/ListBuilds\n  method: post\n  operationId: listBuilds\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /depot.buildkit.v1.BuildKitService/GetEndpoint\n  method: post\n  operationId: getEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/depot-dev/refs/heads/main/agentic-access/depot-dev-agentic-access.yml
summary_line: 14 operations · 14 acting · 1 human-in-the-loop
tags:
- Container Builds
- Docker
- BuildKit
- Remote Cache
- CI/CD
- GitHub Actions
---
