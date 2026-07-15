---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 6
api_specs:
- filename: Business_Process_Service.yaml
  format: yaml
  label: Workday Business Process API
  slug: workday-business-process-api
  spec_type: OpenAPI
  url: https://community.workday.com/sites/default/files/file-hosting/productionapi/Business_Process_Service/v41.1/Business_Process_Service.yaml
consequence_counts:
  read: 6
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Workday Business Processes Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'Workday Business Processes exposes 10 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Workday Business Processes
provider_slug: workday-business-processes
slug: workday-business-processes-agentic-access
source_filename: workday-business-processes-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/workday-business-processes-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 6\n    acting: 4\n  by_consequence:\n    read: 6\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /businessProcessDefinitions\n  method: get\n  operationId: listBusinessProcessDefinitions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /businessProcessDefinitions/{definitionId}\n  method: get\n  operationId: getBusinessProcessDefinition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n \
  \   token:\n      max-ttl: 3600\n    audit: none\n- path: /processInstances\n  method: get\n  operationId: listProcessInstances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /processInstances\n  method: post\n  operationId: initiateProcess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /processInstances/{instanceId}\n  method: get\n  operationId: getProcessInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /processInstances/{instanceId}/cancel\n  method: post\n  operationId: cancelProcessInstance\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inboxItems\n  method: get\n  operationId: listInboxItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inboxItems/{itemId}/approve\n  method: post\n  operationId: approveInboxItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inboxItems/{itemId}/deny\n  method: post\n  operationId: denyInboxItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /processInstances/{instanceId}/steps\n  method: get\n  operationId: listProcessSteps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-business-processes/refs/heads/main/agentic-access/workday-business-processes-agentic-access.yml
summary_line: 10 operations · 4 acting
tags: []
---
