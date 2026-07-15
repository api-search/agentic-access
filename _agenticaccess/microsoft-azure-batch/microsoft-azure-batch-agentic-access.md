---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 4
api_specs:
- filename: microsoft-azure-batch-openapi.yml
  format: yaml
  label: Azure Batch REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-batch/refs/heads/main/openapi/microsoft-azure-batch-openapi.yml
consequence_counts:
  read: 4
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Microsoft Azure Batch Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'microsoft-azure-batch exposes 8 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: microsoft-azure-batch
provider_slug: microsoft-azure-batch
slug: microsoft-azure-batch-agentic-access
source_filename: microsoft-azure-batch-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/microsoft-azure-batch-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 4\n    acting: 4\n  by_consequence:\n    read: 4\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /pools\n  method: get\n  operationId: listPools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - user_impersonation\n- path: /pools\n  method: post\n  operationId: addPool\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - user_impersonation\n- path: /pools/{poolId}\n  method: get\n  operationId: getPool\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - user_impersonation\n- path: /pools/{poolId}\n  method: delete\n  operationId: deletePool\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - user_impersonation\n- path: /jobs\n  method: get\n  operationId: listJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n\
  \    - user_impersonation\n- path: /jobs\n  method: post\n  operationId: addJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - user_impersonation\n- path: /jobs/{jobId}/tasks\n  method: get\n  operationId: listTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - user_impersonation\n- path: /jobs/{jobId}/tasks\n  method: post\n  operationId: addTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n   \
  \ scope:\n    - user_impersonation\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-batch/refs/heads/main/agentic-access/microsoft-azure-batch-agentic-access.yml
summary_line: 8 operations · 4 acting
tags: []
---
