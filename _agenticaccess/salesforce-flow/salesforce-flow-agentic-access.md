---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 6
api_specs:
- filename: salesforce-flow-rest-api-openapi.yml
  format: yaml
  label: Salesforce Flow REST API
  slug: salesforce-flow-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-flow/refs/heads/main/openapi/salesforce-flow-rest-api-openapi.yml
consequence_counts:
  read: 6
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Salesforce Flow Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'Salesforce Flow exposes 10 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Salesforce Flow
provider_slug: salesforce-flow
slug: salesforce-flow-agentic-access
source_filename: salesforce-flow-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/salesforce-flow-rest-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 6\n    acting: 4\n  by_consequence:\n    read: 6\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /sobjects/Flow\n  method: get\n  operationId: listFlows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sobjects/Flow/{flowId}\n  method: get\n  operationId: getFlow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sobjects/Flow/{flowId}\n\
  \  method: patch\n  operationId: updateFlow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sobjects/FlowInterview\n  method: post\n  operationId: createFlowInterview\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sobjects/FlowInterview/{interviewId}\n  method: get\n  operationId: getFlowInterview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sobjects/FlowInterview/{interviewId}\n  method: delete\n  operationId:\
  \ deleteFlowInterview\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /actions/custom/flow\n  method: get\n  operationId: listInvocableFlows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /actions/custom/flow/{flowApiName}\n  method: get\n  operationId: getInvocableFlowMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /actions/custom/flow/{flowApiName}\n  method: post\n  operationId: invokeFlow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /query\n  method: get\n  operationId: queryFlows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salesforce-flow/refs/heads/main/agentic-access/salesforce-flow-agentic-access.yml
summary_line: 10 operations · 4 acting
tags:
- Automation
- Business Process
- CRM
- Flow
- Process Builder
- Salesforce
- Workflow
---
