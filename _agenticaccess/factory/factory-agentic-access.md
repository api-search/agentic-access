---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 6
api_specs:
- filename: factory-automations-api-openapi.yml
  format: yaml
  label: Factory Automations API
  slug: factory-automations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/factory/openapi/factory-automations-api-openapi.yml
- filename: factory-computers-api-openapi.yml
  format: yaml
  label: Factory Computers API
  slug: factory-computers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/factory/openapi/factory-computers-api-openapi.yml
consequence_counts:
  read: 6
  safety-critical: 1
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Factory Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v0/automations/ci/edit
operation_count: 8
overview: 'Factory exposes 8 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 1 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Factory
provider_slug: factory
slug: factory-agentic-access
source_filename: factory-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: generated\nsource: openapi/factory-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 2\n    connected: 6\n  by_consequence:\n    safety-critical: 1\n    read: 6\n    write: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /api/v0/automations/ci/edit\n  method: post\n  operationId: PostOpenACiWorkflowPrCreateEditDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v0/automations/ci/jobs\n\
  \  method: get\n  operationId: GetListCiAutomationJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0/automations/ci/repositories\n  method: get\n  operationId: GetListCiEligibleRepositories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0/automations/ci/repository-owners\n  method: get\n  operationId: GetListCiRepositoryOwners\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0/automations/ci/runs\n  method: get\n  operationId: GetListGithubActionsRunsForCiAutomationWorkflows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0/automations/ci/scan\n\
  \  method: get\n  operationId: GetScanRepositoriesForCiWorkflows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0/computers\n  method: get\n  operationId: listComputers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0/computers\n  method: post\n  operationId: createComputer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/factory/agentic-access/factory-agentic-access.yml
summary_line: 8 operations · 2 acting · 1 human-in-the-loop
tags:
- Manufacturing
- Software-as-a-Service
- Cloud
- Automation
- Supply Chain
- Company
---
