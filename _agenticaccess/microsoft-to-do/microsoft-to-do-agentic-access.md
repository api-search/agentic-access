---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 8
api_specs:
- filename: microsoft-to-do-openapi.yml
  format: yaml
  label: Microsoft Graph to Do Tasks API
  slug: graph-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-to-do/refs/heads/main/openapi/microsoft-to-do-openapi.yml
consequence_counts:
  read: 8
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Microsoft To Do Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 18
overview: 'Microsoft to Do exposes 18 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 10 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Microsoft to Do
provider_slug: microsoft-to-do
slug: microsoft-to-do-agentic-access
source_filename: microsoft-to-do-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/microsoft-to-do-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    connected: 8\n    acting: 10\n  by_consequence:\n    read: 8\n    write: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /me/todo/lists\n  method: get\n  operationId: listTodoTaskLists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/todo/lists\n  method: post\n  operationId: createTodoTaskList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/todo/lists/{todoTaskListId}\n  method: get\n  operationId: getTodoTaskList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/todo/lists/{todoTaskListId}\n  method: patch\n  operationId: updateTodoTaskList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/todo/lists/{todoTaskListId}\n  method: delete\n  operationId: deleteTodoTaskList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /me/todo/lists/{todoTaskListId}/tasks\n  method: get\n  operationId: listTodoTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/todo/lists/{todoTaskListId}/tasks\n  method: post\n  operationId: createTodoTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/todo/lists/{todoTaskListId}/tasks/{todoTaskId}\n  method: get\n  operationId: getTodoTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/todo/lists/{todoTaskListId}/tasks/{todoTaskId}\n  method: patch\n  operationId:\
  \ updateTodoTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/todo/lists/{todoTaskListId}/tasks/{todoTaskId}\n  method: delete\n  operationId: deleteTodoTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/todo/lists/{todoTaskListId}/tasks/{todoTaskId}/checklistItems\n  method: get\n  operationId: listChecklistItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/todo/lists/{todoTaskListId}/tasks/{todoTaskId}/checklistItems\n\
  \  method: post\n  operationId: createChecklistItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/todo/lists/{todoTaskListId}/tasks/{todoTaskId}/checklistItems/{checklistItemId}\n  method: get\n  operationId: getChecklistItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/todo/lists/{todoTaskListId}/tasks/{todoTaskId}/checklistItems/{checklistItemId}\n  method: patch\n  operationId: updateChecklistItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /me/todo/lists/{todoTaskListId}/tasks/{todoTaskId}/checklistItems/{checklistItemId}\n  method: delete\n  operationId: deleteChecklistItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/todo/lists/{todoTaskListId}/tasks/{todoTaskId}/linkedResources\n  method: get\n  operationId: listLinkedResources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/todo/lists/{todoTaskListId}/tasks/{todoTaskId}/linkedResources\n  method: post\n  operationId: createLinkedResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n     \
  \ max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/todo/lists/{todoTaskListId}/tasks/delta\n  method: get\n  operationId: deltaTodoTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-to-do/refs/heads/main/agentic-access/microsoft-to-do-agentic-access.yml
summary_line: 18 operations · 10 acting
tags:
- Microsoft
- Microsoft 365
- Productivity
- Tasks
---
