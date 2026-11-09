---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 6
api_specs:
- filename: wapiworld-com-instances-api-openapi.yml
  format: yaml
  label: wapiworld-com Instances API
  slug: wapiworld-com-instances-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wapiworld-com/openapi/wapiworld-com-instances-api-openapi.yml
- filename: wapiworld-com-messages-api-openapi.yml
  format: yaml
  label: wapiworld-com Messages API
  slug: wapiworld-com-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wapiworld-com/openapi/wapiworld-com-messages-api-openapi.yml
- filename: wapiworld-com-projects-api-openapi.yml
  format: yaml
  label: wapiworld-com Projects API
  slug: wapiworld-com-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wapiworld-com/openapi/wapiworld-com-projects-api-openapi.yml
- filename: wapiworld-com-webhook-subscriptions-api-openapi.yml
  format: yaml
  label: wapiworld-com Webhook subscriptions API
  slug: wapiworld-com-webhook-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wapiworld-com/openapi/wapiworld-com-webhook-subscriptions-api-openapi.yml
consequence_counts:
  physical: 2
  read: 6
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Wapiworld Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/instances/{instanceId}/action/send-message-idempotent
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/instances/{instanceId}/action/{action}
operation_count: 14
overview: 'wapiworld-com exposes 14 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 6 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: wapiworld-com
provider_slug: wapiworld-com
slug: wapiworld-com-agentic-access
source_filename: wapiworld-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/wapiworld-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 6\n    acting: 8\n  by_consequence:\n    read: 6\n    write: 6\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/instances\n  method: get\n  operationId: getApiInstances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/instances\n  method: post\n  operationId: postApiInstances\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/instances/{instanceId}\n  method: get\n  operationId: getApiInstancesInstanceId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/instances/{instanceId}\n  method: put\n  operationId: putApiInstancesInstanceId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/instances/{instanceId}\n  method: delete\n  operationId: deleteApiInstancesInstanceId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/instances/{instanceId}/action/send-message-idempotent\n  method: post\n  operationId: postApiInstancesInstanceIdActionSendMessageIdempotent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/instances/{instanceId}/action/{action}\n  method: post\n  operationId: postApiInstancesInstanceIdActionAction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /api/messages\n  method: get\n  operationId: getApiMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/projects\n  method: get\n  operationId: getApiProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/projects/{projectId}\n  method: get\n  operationId: getApiProjectsProjectId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/webhooksubscriptions\n  method: get\n  operationId: getApiWebhooksubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/webhooksubscriptions\n  method: post\n  operationId:\
  \ postApiWebhooksubscriptions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/webhooksubscriptions/{webhookSubscriptionId}\n  method: put\n  operationId: putApiWebhooksubscriptionsWebhookSubscriptionId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/webhooksubscriptions/{webhookSubscriptionId}\n  method: delete\n  operationId: deleteApiWebhooksubscriptionsWebhookSubscriptionId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/wapiworld-com/agentic-access/wapiworld-com-agentic-access.yml
summary_line: 14 operations · 8 acting
tags:
- Messaging
- WhatsApp
- Developer Platform
- Communications
---
