---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 6
api_specs:
- filename: cflow-openapi.yml
  format: yaml
  label: Cflow Workflow API
  slug: cflow
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cflow/refs/heads/main/openapi/cflow-openapi.yml
consequence_counts:
  read: 6
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cflow Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Cflow exposes 12 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cflow
provider_slug: cflow
slug: cflow-agentic-access
source_filename: cflow-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/cflow-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 6\n    acting: 6\n  by_consequence:\n    read: 6\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /integromat/api/cflow/getworkflows\n  method: get\n  operationId: getWorkflows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integromat/api/cflow/workflows/{workflowId}\n  method: get\n  operationId: getWorkflow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /integromat/api/cflow/workflows/{workflowId}/requests\n  method: get\n  operationId: listRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integromat/api/cflow/workflows/{workflowId}/requests\n  method: post\n  operationId: createRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integromat/api/cflow/workflows/{workflowId}/requests/{requestId}\n  method: get\n  operationId: getRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integromat/api/cflow/workflows/{workflowId}/requests/{requestId}\n  method: put\n  operationId:\
  \ updateRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integromat/api/cflow/workflows/{workflowId}/requests/{requestId}\n  method: delete\n  operationId: deleteRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integromat/api/cflow/workflows/{workflowId}/requests/{requestId}/approve\n  method: post\n  operationId: approveRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integromat/api/cflow/workflows/{workflowId}/requests/{requestId}/reject\n  method: post\n  operationId: rejectRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integromat/api/cflow/workflows/{workflowId}/drafts\n  method: post\n  operationId: createDraftRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integromat/api/cflow/users\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integromat/api/cflow/roles\n  method: get\n  operationId: listRoles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cflow/refs/heads/main/agentic-access/cflow-agentic-access.yml
summary_line: 12 operations · 6 acting
tags:
- Automations
- Business Process Automation
- Integrations
- No-Code
- Platform
- Protocols
- Rules
- Workflows
---
