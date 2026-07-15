---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 12
api_specs:
- filename: open-source
  format: yaml
  label: Kestra Flows API
  slug: flows-api
  spec_type: OpenAPI
  url: https://kestra.io/docs/api-reference/open-source
- filename: open-source
  format: yaml
  label: Kestra Executions API
  slug: executions-api
  spec_type: OpenAPI
  url: https://kestra.io/docs/api-reference/open-source
- filename: open-source
  format: yaml
  label: Kestra Namespaces API
  slug: namespaces-api
  spec_type: OpenAPI
  url: https://kestra.io/docs/api-reference/open-source
- filename: open-source
  format: yaml
  label: Kestra Key-Value Store API
  slug: kv-store-api
  spec_type: OpenAPI
  url: https://kestra.io/docs/api-reference/open-source
- filename: open-source
  format: yaml
  label: Kestra Namespace Files API
  slug: namespace-files-api
  spec_type: OpenAPI
  url: https://kestra.io/docs/api-reference/open-source
consequence_counts:
  read: 12
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Kestra Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 19
overview: 'Kestra exposes 19 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Kestra
provider_slug: kestra
slug: kestra-agentic-access
source_filename: kestra-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/kestra-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    connected: 12\n    acting: 7\n  by_consequence:\n    read: 12\n    write: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/flows\n  method: get\n  operationId: searchFlows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/flows\n  method: post\n  operationId: createFlow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/flows/{namespace}/{id}\n  method: get\n  operationId: getFlow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/flows/{namespace}/{id}\n  method: put\n  operationId: updateFlow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/flows/{namespace}/{id}\n  method: delete\n  operationId: deleteFlow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/v1/executions\n  method: get\n  operationId: searchExecutions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/executions/trigger/{namespace}/{flowId}\n  method: post\n  operationId: triggerExecution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/executions/{executionId}\n  method: get\n  operationId: getExecution\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/executions/{executionId}/logs\n  method: get\n  operationId: getExecutionLogs\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/namespaces\n  method: get\n  operationId: listNamespaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/namespaces/{namespace}\n  method: get\n  operationId: getNamespace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/triggers\n  method: get\n  operationId: searchTriggers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/namespaces/{namespace}/kv\n  method: get\n  operationId: listKv\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/v1/namespaces/{namespace}/kv/{key}\n  method: get\n  operationId: getKv\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/namespaces/{namespace}/kv/{key}\n  method: put\n  operationId: setKv\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/namespaces/{namespace}/kv/{key}\n  method: delete\n  operationId: deleteKv\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/namespaces/{namespace}/files\n\
  \  method: get\n  operationId: listNamespaceFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/namespaces/{namespace}/files/file\n  method: get\n  operationId: downloadNamespaceFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/namespaces/{namespace}/files/file\n  method: post\n  operationId: uploadNamespaceFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kestra/refs/heads/main/agentic-access/kestra-agentic-access.yml
summary_line: 19 operations · 7 acting
tags:
- Automation
- Data Pipelines
- Event-Driven
- Orchestration
- Workflows
---
