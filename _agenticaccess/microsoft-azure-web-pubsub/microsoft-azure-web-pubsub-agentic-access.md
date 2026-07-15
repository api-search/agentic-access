---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 4
api_specs:
- filename: webpubsub.json
  format: json
  label: Azure Web PubSub Service REST API
  slug: azure-web-pubsub-service-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/webpubsub/data-plane/WebPubSub/stable/2024-01-01/webpubsub.json
- filename: microsoft-azure-web-pubsub-asyncapi.yml
  format: yaml
  label: Azure Web PubSub Client and Upstream Events
  slug: azure-web-pubsub-client-and-upstream-events
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-web-pubsub/main/asyncapi/microsoft-azure-web-pubsub-asyncapi.yml
- filename: webpubsub.json
  format: json
  label: Azure Web PubSub Management REST API
  slug: azure-web-pubsub-management-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/webpubsub/resource-manager/Microsoft.SignalRService/stable/2024-03-01/webpubsub.json
consequence_counts:
  physical: 4
  read: 4
  safety-critical: 1
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Microsoft Azure Web Pubsub Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/hubs/{hub}/permissions/{permission}/connections/{connectionId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/hubs/{hub}/:send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/hubs/{hub}/connections/{connectionId}/:send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/hubs/{hub}/groups/{group}/:send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/hubs/{hub}/users/{userId}/:send
operation_count: 19
overview: 'Azure Web PubSub exposes 19 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read, 10 write, 4 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Azure Web PubSub
provider_slug: microsoft-azure-web-pubsub
slug: microsoft-azure-web-pubsub-agentic-access
source_filename: microsoft-azure-web-pubsub-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/microsoft-azure-web-pubsub-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    acting: 15\n    connected: 4\n  by_consequence:\n    physical: 4\n    read: 4\n    write: 10\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /api/hubs/{hub}/:send\n  method: post\n  operationId: webPubSub_sendToAll\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/hubs/{hub}/connections/{connectionId}/:send\n  method: post\n  operationId: webPubSub_sendToConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/hubs/{hub}/groups/{group}/:send\n  method: post\n  operationId: webPubSub_sendToGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/hubs/{hub}/users/{userId}/:send\n  method: post\n  operationId: webPubSub_sendToUser\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/hubs/{hub}/connections/{connectionId}\n  method: head\n  operationId: webPubSub_connectionExists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/hubs/{hub}/connections/{connectionId}\n  method: delete\n  operationId: webPubSub_closeConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/hubs/{hub}/:closeConnections\n\
  \  method: post\n  operationId: webPubSub_closeAllConnections\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/hubs/{hub}/groups/{group}/:close\n  method: post\n  operationId: webPubSub_closeGroupConnections\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/hubs/{hub}/users/{userId}/:close\n  method: post\n  operationId: webPubSub_closeUserConnections\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/hubs/{hub}/groups/{group}\n  method: head\n  operationId: webPubSub_groupExists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/hubs/{hub}/users/{userId}\n  method: head\n  operationId: webPubSub_userExists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/hubs/{hub}/groups/{group}/connections/{connectionId}\n  method: put\n  operationId: webPubSub_addConnectionToGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/hubs/{hub}/groups/{group}/connections/{connectionId}\n  method: delete\n  operationId: webPubSub_removeConnectionFromGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/hubs/{hub}/groups/{group}/users/{userId}\n  method: put\n  operationId: webPubSub_addUserToGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/hubs/{hub}/groups/{group}/users/{userId}\n  method: delete\n  operationId: webPubSub_removeUserFromGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/hubs/{hub}/permissions/{permission}/connections/{connectionId}\n  method: put\n  operationId: webPubSub_grantPermission\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/hubs/{hub}/permissions/{permission}/connections/{connectionId}\n  method: delete\n  operationId: webPubSub_revokePermission\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /api/hubs/{hub}/permissions/{permission}/connections/{connectionId}\n  method: head\n  operationId: webPubSub_checkPermission\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/hubs/{hub}/:generateToken\n  method: post\n  operationId: webPubSub_generateClientToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-web-pubsub/refs/heads/main/agentic-access/microsoft-azure-web-pubsub-agentic-access.yml
summary_line: 19 operations · 15 acting · 1 human-in-the-loop
tags:
- Messaging
- Pub-Sub
- Real-Time
- Serverless
- WebSockets
---
