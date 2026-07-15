---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 10
api_specs:
- filename: temporal-io-openapi.yml
  format: yaml
  label: Temporal Workflow Service API
  slug: temporal-io-workflow-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temporal-io/refs/heads/main/openapi/temporal-io-openapi.yml
- filename: temporal-io-openapi.yml
  format: yaml
  label: Temporal HTTP API
  slug: temporal-io-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temporal-io/refs/heads/main/openapi/temporal-io-openapi.yml
consequence_counts:
  read: 10
  safety-critical: 2
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Temporal Io Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /namespaces/{namespace}/workflows/{workflow_execution.workflow_id}/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /namespaces/{namespace}/workflows/{workflow_execution.workflow_id}/terminate
operation_count: 17
overview: 'Temporal exposes 17 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read, 5 write, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Temporal
provider_slug: temporal-io
slug: temporal-io-agentic-access
source_filename: temporal-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/temporal-io-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    acting: 7\n    connected: 10\n  by_consequence:\n    write: 5\n    read: 10\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /namespaces/{namespace}/workflows/{workflow_id}\n  method: post\n  operationId: startWorkflowExecution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /namespaces/{namespace}/workflows/{execution.workflow_id}\n\
  \  method: get\n  operationId: describeWorkflowExecution\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /namespaces/{namespace}/workflows\n  method: get\n  operationId: listWorkflowExecutions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /namespaces/{namespace}/workflow-count\n  method: get\n  operationId: countWorkflowExecutions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /namespaces/{namespace}/archived-workflows\n  method: get\n  operationId: listArchivedWorkflowExecutions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /namespaces/{namespace}/workflows/{execution.workflow_id}/history\n\
  \  method: get\n  operationId: getWorkflowExecutionHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /namespaces/{namespace}/workflows/{execution.workflow_id}/history-reverse\n  method: get\n  operationId: getWorkflowExecutionHistoryReverse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /namespaces/{namespace}/workflows/{workflow_execution.workflow_id}/signal/{signal_name}\n  method: post\n  operationId: signalWorkflowExecution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /namespaces/{namespace}/workflows/{execution.workflow_id}/query/{query.query_type}\n\
  \  method: post\n  operationId: queryWorkflow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /namespaces/{namespace}/workflows/{workflow_execution.workflow_id}/update/{name}\n  method: post\n  operationId: updateWorkflowExecution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /namespaces/{namespace}/workflows/{workflow_execution.workflow_id}/cancel\n  method: post\n  operationId: requestCancelWorkflowExecution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /namespaces/{namespace}/workflows/{workflow_execution.workflow_id}/terminate\n  method: post\n  operationId: terminateWorkflowExecution\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /namespaces/{namespace}/workflows/{workflow_execution.workflow_id}/reset\n  method: post\n  operationId: resetWorkflowExecution\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /namespaces/{namespace}\n  method: get\n  operationId: describeNamespace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /namespaces\n  method: get\n  operationId: listNamespaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cluster-info\n  method: get\n  operationId: getClusterInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /system-info\n  method: get\n  operationId: getSystemInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/temporal-io/refs/heads/main/agentic-access/temporal-io-agentic-access.yml
summary_line: 17 operations · 7 acting · 2 human-in-the-loop
tags:
- Durable Execution
- Workflow Orchestration
- gRPC
- Workflows
- Open Source
- Temporal Cloud
---
