---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 4
api_specs:
- filename: openapi.yml
  format: yaml
  label: Google Cloud Workflows API
  slug: google-cloud-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-workflows/refs/heads/main/openapi/openapi.yml
consequence_counts:
  read: 4
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Google Cloud Workflows Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'Google Cloud Workflows exposes 9 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Google Cloud Workflows
provider_slug: google-cloud-workflows
slug: google-cloud-workflows-agentic-access
source_filename: google-cloud-workflows-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 4\n    acting: 5\n  by_consequence:\n    read: 4\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/projects/{project}/locations/{location}/workflows\n  method: get\n  operationId: listWorkflows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{project}/locations/{location}/workflows\n  method: post\n  operationId: createWorkflow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects/{project}/locations/{location}/workflows/{workflow}\n  method: get\n  operationId: getWorkflow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{project}/locations/{location}/workflows/{workflow}\n  method: patch\n  operationId: updateWorkflow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects/{project}/locations/{location}/workflows/{workflow}\n  method: delete\n  operationId: deleteWorkflow\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects/{project}/locations/{location}/workflows/{workflow}/executions\n  method: get\n  operationId: listExecutions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{project}/locations/{location}/workflows/{workflow}/executions\n  method: post\n  operationId: createExecution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects/{project}/locations/{location}/workflows/{workflow}/executions/{execution}\n\
  \  method: get\n  operationId: getExecution\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{project}/locations/{location}/workflows/{workflow}/executions/{execution}:cancel\n  method: post\n  operationId: cancelExecution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-workflows/refs/heads/main/agentic-access/google-cloud-workflows-agentic-access.yml
summary_line: 9 operations · 5 acting
tags:
- Automation
- Google Cloud
- Integration
- Orchestration
- Serverless
- Workflows
---
