---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 11
api_specs:
- filename: microsoft-planner-openapi.yml
  format: yaml
  label: Microsoft Planner API
  slug: microsoft-planner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-planner/refs/heads/main/openapi/microsoft-planner-openapi.yml
- filename: microsoft-planner-openapi.yml
  format: yaml
  label: Microsoft Graph Plans API
  slug: microsoft-graph-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-planner/refs/heads/main/openapi/microsoft-planner-openapi.yml
- filename: microsoft-planner-openapi.yml
  format: yaml
  label: Microsoft Graph Tasks API
  slug: microsoft-graph-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-planner/refs/heads/main/openapi/microsoft-planner-openapi.yml
- filename: microsoft-planner-openapi.yml
  format: yaml
  label: Microsoft Graph Buckets API
  slug: microsoft-graph-buckets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-planner/refs/heads/main/openapi/microsoft-planner-openapi.yml
consequence_counts:
  read: 11
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Microsoft Planner Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 22
overview: 'Microsoft Planner exposes 22 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 11 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Microsoft Planner
provider_slug: microsoft-planner
slug: microsoft-planner-agentic-access
source_filename: microsoft-planner-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/microsoft-planner-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    acting: 11\n    connected: 11\n  by_consequence:\n    write: 11\n    read: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /planner/plans\n  method: post\n  operationId: createPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - Group.Read.All\n    - Group.ReadWrite.All\n    - Tasks.Read\n    - Tasks.ReadWrite\n- path: /planner/plans/{plan-id}\n\
  \  method: get\n  operationId: getPlan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - Group.Read.All\n    - Group.ReadWrite.All\n    - Tasks.Read\n    - Tasks.ReadWrite\n- path: /planner/plans/{plan-id}\n  method: patch\n  operationId: updatePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - Group.Read.All\n    - Group.ReadWrite.All\n    - Tasks.Read\n    - Tasks.ReadWrite\n- path: /planner/plans/{plan-id}\n  method: delete\n  operationId: deletePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - Group.Read.All\n    - Group.ReadWrite.All\n    - Tasks.Read\n    - Tasks.ReadWrite\n- path: /planner/plans/{plan-id}/tasks\n  method: get\n  operationId: listPlanTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - Group.Read.All\n    - Group.ReadWrite.All\n    - Tasks.Read\n    - Tasks.ReadWrite\n- path: /planner/plans/{plan-id}/buckets\n  method: get\n  operationId: listPlanBuckets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - Group.Read.All\n    - Group.ReadWrite.All\n    - Tasks.Read\n    - Tasks.ReadWrite\n- path: /planner/plans/{plan-id}/details\n  method: get\n  operationId: getPlanDetails\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - Group.Read.All\n    - Group.ReadWrite.All\n    - Tasks.Read\n    - Tasks.ReadWrite\n- path: /planner/plans/{plan-id}/details\n  method: patch\n  operationId: updatePlanDetails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - Group.Read.All\n    - Group.ReadWrite.All\n    - Tasks.Read\n    - Tasks.ReadWrite\n- path: /planner/tasks\n  method: post\n  operationId: createTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n    scope:\n    - Group.Read.All\n    - Group.ReadWrite.All\n    - Tasks.Read\n    - Tasks.ReadWrite\n- path: /planner/tasks/{task-id}\n  method: get\n  operationId: getTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - Group.Read.All\n    - Group.ReadWrite.All\n    - Tasks.Read\n    - Tasks.ReadWrite\n- path: /planner/tasks/{task-id}\n  method: patch\n  operationId: updateTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - Group.Read.All\n    - Group.ReadWrite.All\n    - Tasks.Read\n    - Tasks.ReadWrite\n- path: /planner/tasks/{task-id}\n  method: delete\n  operationId: deleteTask\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - Group.Read.All\n    - Group.ReadWrite.All\n    - Tasks.Read\n    - Tasks.ReadWrite\n- path: /planner/tasks/{task-id}/details\n  method: get\n  operationId: getTaskDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - Group.Read.All\n    - Group.ReadWrite.All\n    - Tasks.Read\n    - Tasks.ReadWrite\n- path: /planner/tasks/{task-id}/details\n  method: patch\n  operationId: updateTaskDetails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n    scope:\n    - Group.Read.All\n    - Group.ReadWrite.All\n    - Tasks.Read\n    - Tasks.ReadWrite\n- path: /planner/buckets\n  method: post\n  operationId: createBucket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - Group.Read.All\n    - Group.ReadWrite.All\n    - Tasks.Read\n    - Tasks.ReadWrite\n- path: /planner/buckets/{bucket-id}\n  method: get\n  operationId: getBucket\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - Group.Read.All\n    - Group.ReadWrite.All\n    - Tasks.Read\n    - Tasks.ReadWrite\n- path: /planner/buckets/{bucket-id}\n  method: patch\n  operationId: updateBucket\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - Group.Read.All\n    - Group.ReadWrite.All\n    - Tasks.Read\n    - Tasks.ReadWrite\n- path: /planner/buckets/{bucket-id}\n  method: delete\n  operationId: deleteBucket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - Group.Read.All\n    - Group.ReadWrite.All\n    - Tasks.Read\n    - Tasks.ReadWrite\n- path: /planner/buckets/{bucket-id}/tasks\n  method: get\n  operationId: listBucketTasks\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - Group.Read.All\n    - Group.ReadWrite.All\n    - Tasks.Read\n    - Tasks.ReadWrite\n- path: /groups/{group-id}/planner/plans\n  method: get\n  operationId: listGroupPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - Group.Read.All\n    - Group.ReadWrite.All\n    - Tasks.Read\n    - Tasks.ReadWrite\n- path: /me/planner/tasks\n  method: get\n  operationId: listMyTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - Group.Read.All\n    - Group.ReadWrite.All\n    - Tasks.Read\n    - Tasks.ReadWrite\n- path: /users/{user-id}/planner/tasks\n  method: get\n  operationId: listUserTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - Group.Read.All\n    - Group.ReadWrite.All\n    - Tasks.Read\n    - Tasks.ReadWrite\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-planner/refs/heads/main/agentic-access/microsoft-planner-agentic-access.yml
summary_line: 22 operations · 11 acting
tags:
- Collaboration
- Microsoft 365
- Productivity
- Project Management
- Task Management
---
