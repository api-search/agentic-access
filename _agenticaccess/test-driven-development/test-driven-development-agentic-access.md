---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 4
api_specs:
- filename: api.github.com.json
  format: json
  label: GitHub Actions API
  slug: github-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/github/rest-api-description/main/descriptions/api.github.com/api.github.com.json
- filename: openapi.json
  format: json
  label: CircleCI API
  slug: circleci-api
  spec_type: OpenAPI
  url: https://circleci.com/api/v2/openapi.json
consequence_counts:
  read: 4
  safety-critical: 1
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Test Driven Development Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /repos/{owner}/{repo}/actions/workflows/{workflow_id}/dispatches
operation_count: 7
overview: 'Test-Driven Development exposes 7 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read, 2 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Test-Driven Development
provider_slug: test-driven-development
slug: test-driven-development-agentic-access
source_filename: test-driven-development-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/test-driven-development-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 4\n    acting: 3\n  by_consequence:\n    read: 4\n    safety-critical: 1\n    write: 2\n  human_in_the_loop_required: 1\noperations:\n- path: /repos/{owner}/{repo}/actions/workflows\n  method: get\n  operationId: listWorkflows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repos/{owner}/{repo}/actions/workflows/{workflow_id}\n  method: get\n  operationId: getWorkflow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /repos/{owner}/{repo}/actions/workflows/{workflow_id}/dispatches\n  method: post\n  operationId: dispatchWorkflow\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /repos/{owner}/{repo}/actions/runs\n  method: get\n  operationId: listWorkflowRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repos/{owner}/{repo}/actions/runs/{run_id}\n  method: get\n  operationId: getWorkflowRun\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repos/{owner}/{repo}/actions/runs/{run_id}/rerun\n\
  \  method: post\n  operationId: rerunWorkflowRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /repos/{owner}/{repo}/actions/runs/{run_id}/cancel\n  method: post\n  operationId: cancelWorkflowRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/test-driven-development/refs/heads/main/agentic-access/test-driven-development-agentic-access.yml
summary_line: 7 operations · 3 acting · 1 human-in-the-loop
tags:
- Agile
- Best Practices
- Continuous Integration
- Extreme Programming
- Methodology
- Software Development
- Testing
---
