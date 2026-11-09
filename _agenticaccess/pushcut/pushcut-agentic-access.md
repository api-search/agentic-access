---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 3
api_specs:
- filename: pushcut-automation-server-api-openapi.yml
  format: yaml
  label: Pushcut Automation Server API
  slug: pushcut-automation-server-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pushcut/openapi/pushcut-automation-server-api-openapi.yml
- filename: pushcut-notifications-api-openapi.yml
  format: yaml
  label: Pushcut Notifications API
  slug: pushcut-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pushcut/openapi/pushcut-notifications-api-openapi.yml
- filename: pushcut-subscriptions-api-openapi.yml
  format: yaml
  label: Pushcut Subscriptions API
  slug: pushcut-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pushcut/openapi/pushcut-subscriptions-api-openapi.yml
consequence_counts:
  physical: 1
  read: 3
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Pushcut Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /notifications/{notificationName}
operation_count: 9
overview: 'Pushcut exposes 9 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read, 5 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Pushcut
provider_slug: pushcut
slug: pushcut-agentic-access
source_filename: pushcut-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: generated\nsource: openapi/pushcut-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 3\n    acting: 6\n  by_consequence:\n    read: 3\n    physical: 1\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /devices\n  method: get\n  operationId: GetDevices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /notifications\n  method: get\n  operationId: GetNotifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /notifications/{notificationName}\n\
  \  method: post\n  operationId: SendNotification\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /submittedNotifications/{notificationId}\n  method: delete\n  operationId: CancelNotification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions\n  method: get\n  operationId: GetSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions\n\
  \  method: post\n  operationId: ActionExecuted\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/{subscriptionId}\n  method: delete\n  operationId: DeleteSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /execute\n  method: post\n  operationId: Execute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /cancelExecution\n  method: post\n  operationId: CancelExecution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/pushcut/agentic-access/pushcut-agentic-access.yml
summary_line: 9 operations · 6 acting
tags:
- Company
- Automation
- iOS
- Shortcuts
- Webhook
- Integration
---
