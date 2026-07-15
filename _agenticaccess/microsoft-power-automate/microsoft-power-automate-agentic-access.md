---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 9
api_specs:
- filename: microsoft-power-automate-management-api.yaml
  format: yaml
  label: Power Automate Management API
  slug: power-automate-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-automate/refs/heads/main/openapi/microsoft-power-automate-management-api.yaml
consequence_counts:
  read: 9
  safety-critical: 1
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Microsoft Power Automate Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /providers/Microsoft.ProcessSimple/environments/{environmentName}/flows/{flowName}/stop
operation_count: 18
overview: 'Microsoft Power Automate exposes 18 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 8 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Microsoft Power Automate
provider_slug: microsoft-power-automate
slug: microsoft-power-automate-agentic-access
source_filename: microsoft-power-automate-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/microsoft-power-automate-management-api.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    connected: 9\n    acting: 9\n  by_consequence:\n    read: 9\n    write: 8\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /providers/Microsoft.ProcessSimple/environments\n  method: get\n  operationId: listEnvironments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /providers/Microsoft.ProcessSimple/environments/{environmentName}/flows\n  method: get\n  operationId: listFlows\n  x-agentic-access:\n    action-class: connected\n \
  \   consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /providers/Microsoft.ProcessSimple/environments/{environmentName}/flows\n  method: post\n  operationId: createFlow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /providers/Microsoft.ProcessSimple/environments/{environmentName}/flows/{flowName}\n  method: get\n  operationId: getFlow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /providers/Microsoft.ProcessSimple/environments/{environmentName}/flows/{flowName}\n  method: patch\n  operationId: updateFlow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /providers/Microsoft.ProcessSimple/environments/{environmentName}/flows/{flowName}\n  method: delete\n  operationId: deleteFlow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /providers/Microsoft.ProcessSimple/environments/{environmentName}/flows/{flowName}/start\n  method: post\n  operationId: turnOnFlow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /providers/Microsoft.ProcessSimple/environments/{environmentName}/flows/{flowName}/stop\n  method: post\n  operationId: turnOffFlow\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /providers/Microsoft.ProcessSimple/environments/{environmentName}/flows/{flowName}/runs\n  method: get\n  operationId: listFlowRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /providers/Microsoft.ProcessSimple/environments/{environmentName}/flows/{flowName}/runs/{runId}\n  method: get\n  operationId: getFlowRun\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /providers/Microsoft.ProcessSimple/environments/{environmentName}/flows/{flowName}/runs/{runId}/cancel\n  method: post\n  operationId: cancelFlowRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /providers/Microsoft.ProcessSimple/environments/{environmentName}/flows/{flowName}/runs/{runId}/resubmit\n  method: post\n  operationId: resubmitFlowRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /providers/Microsoft.ProcessSimple/environments/{environmentName}/flows/{flowName}/owners\n\
  \  method: get\n  operationId: listFlowOwners\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /providers/Microsoft.ProcessSimple/environments/{environmentName}/flows/{flowName}/owners\n  method: post\n  operationId: modifyFlowOwners\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /providers/Microsoft.ProcessSimple/environments/{environmentName}/flows/{flowName}/listCallbackUrl\n  method: post\n  operationId: listCallbackUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /providers/Microsoft.ProcessSimple/environments/{environmentName}/apis\n  method: get\n  operationId: listConnectors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /providers/Microsoft.ProcessSimple/environments/{environmentName}/apis/{apiName}\n  method: get\n  operationId: getConnector\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /providers/Microsoft.ProcessSimple/environments/{environmentName}/connections\n  method: get\n  operationId: listConnections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-automate/refs/heads/main/agentic-access/microsoft-power-automate-agentic-access.yml
summary_line: 18 operations · 9 acting · 1 human-in-the-loop
tags:
- Automation
- Business Process
- Integration
- Low-Code
- Microsoft
- Power Platform
- RPA
- Workflow
---
