---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 8
api_specs:
- filename: microsoft-office-management-activity-api-openapi.yml
  format: yaml
  label: Microsoft Office 365 Management Activity API
  slug: management-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-integration/refs/heads/main/openapi/microsoft-office-management-activity-api-openapi.yml
- filename: microsoft-office-service-communications-api-openapi.yml
  format: yaml
  label: Microsoft Office 365 Service Communications API
  slug: service-communications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-integration/refs/heads/main/openapi/microsoft-office-service-communications-api-openapi.yml
consequence_counts:
  read: 8
  safety-critical: 1
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Microsoft Office Integration Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /subscriptions/stop
operation_count: 10
overview: 'Microsoft Office Integration exposes 10 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 1 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Microsoft Office Integration
provider_slug: microsoft-office-integration
slug: microsoft-office-integration-agentic-access
source_filename: microsoft-office-integration-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/microsoft-office-management-activity-api-openapi.yml, openapi/microsoft-office-service-communications-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    acting: 2\n    connected: 8\n  by_consequence:\n    write: 1\n    safety-critical: 1\n    read: 8\n  human_in_the_loop_required: 1\noperations:\n- path: /subscriptions/start\n  method: post\n  operationId: startSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /subscriptions/stop\n  method: post\n  operationId: stopSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /subscriptions/list\n  method: get\n  operationId: listSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions/content\n  method: get\n  operationId: listAvailableContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions/notifications\n  method: get\n  operationId: listNotifications\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resources/dlpSensitiveTypes\n  method: get\n  operationId: listDlpSensitiveTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Services\n  method: get\n  operationId: getServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /CurrentStatus\n  method: get\n  operationId: getCurrentStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /HistoricalStatus\n  method: get\n  operationId: getHistoricalStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Messages\n  method: get\n\
  \  operationId: getMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-integration/refs/heads/main/agentic-access/microsoft-office-integration-agentic-access.yml
summary_line: 10 operations · 2 acting · 1 human-in-the-loop
tags:
- Microsoft 365
- Microsoft Office Integration
- Office 365
---
