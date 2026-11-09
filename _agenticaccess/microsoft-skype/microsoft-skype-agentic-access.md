---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 7
api_specs:
- filename: microsoft-skype-deliveryreports-api-openapi.yml
  format: yaml
  label: Microsoft Skype Delivery Reports API
  slug: microsoft-skype-deliveryreports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-skype/openapi/microsoft-skype-deliveryreports-api-openapi.yml
- filename: microsoft-skype-messages-api-openapi.yml
  format: yaml
  label: Microsoft Skype Messages API
  slug: microsoft-skype-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-skype/openapi/microsoft-skype-messages-api-openapi.yml
- filename: microsoft-skype-optoutsadd-api-openapi.yml
  format: yaml
  label: Microsoft Skype Opt Outs Add API
  slug: microsoft-skype-optoutsadd-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-skype/openapi/microsoft-skype-optoutsadd-api-openapi.yml
- filename: microsoft-skype-optoutscheck-api-openapi.yml
  format: yaml
  label: Microsoft Skype Opt Outs Check API
  slug: microsoft-skype-optoutscheck-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-skype/openapi/microsoft-skype-optoutscheck-api-openapi.yml
- filename: microsoft-skype-optoutsremove-api-openapi.yml
  format: yaml
  label: Microsoft Skype Opt Outs Remove API
  slug: microsoft-skype-optoutsremove-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-skype/openapi/microsoft-skype-optoutsremove-api-openapi.yml
- filename: microsoft-skype-participants-api-openapi.yml
  format: yaml
  label: Microsoft Skype Participants API
  slug: microsoft-skype-participants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-skype/openapi/microsoft-skype-participants-api-openapi.yml
- filename: microsoft-skype-sms-api-openapi.yml
  format: yaml
  label: Microsoft Skype Sms API
  slug: microsoft-skype-sms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-skype/openapi/microsoft-skype-sms-api-openapi.yml
- filename: microsoft-skype-threads-api-openapi.yml
  format: yaml
  label: Microsoft Skype Threads API
  slug: microsoft-skype-threads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-skype/openapi/microsoft-skype-threads-api-openapi.yml
- filename: microsoft-skype-typingnotifications-api-openapi.yml
  format: yaml
  label: Microsoft Skype Typing Notifications API
  slug: microsoft-skype-typingnotifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-skype/openapi/microsoft-skype-typingnotifications-api-openapi.yml
consequence_counts:
  physical: 5
  read: 7
  safety-critical: 1
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Microsoft Skype Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /sms/optouts:add
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /chat/threads/{chatThreadId}/messages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /chat/threads/{chatThreadId}/readReceipts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /chat/threads/{chatThreadId}/typing
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sms
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sms/optouts:check
operation_count: 21
overview: 'Microsoft Skype exposes 21 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read, 8 write, 5 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Microsoft Skype
provider_slug: microsoft-skype
slug: microsoft-skype-agentic-access
source_filename: microsoft-skype-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/microsoft-skype-chat-openapi.yml, openapi/microsoft-skype-sms-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    connected: 7\n    acting: 14\n  by_consequence:\n    read: 7\n    physical: 5\n    write: 8\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /chat/threads/{chatThreadId}/readReceipts\n  method: get\n  operationId: ChatThread_ListChatReadReceipts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chat/threads/{chatThreadId}/readReceipts\n  method: post\n  operationId: ChatThread_SendChatReadReceipt\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chat/threads/{chatThreadId}/messages\n  method: post\n  operationId: ChatThread_SendChatMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chat/threads/{chatThreadId}/messages\n  method: get\n  operationId: ChatThread_ListChatMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /chat/threads/{chatThreadId}/messages/{chatMessageId}\n  method: get\n  operationId: ChatThread_GetChatMessage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chat/threads/{chatThreadId}/messages/{chatMessageId}\n  method: patch\n  operationId: ChatThread_UpdateChatMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chat/threads/{chatThreadId}/messages/{chatMessageId}\n  method: delete\n  operationId: ChatThread_DeleteChatMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n    \
  \  triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chat/threads/{chatThreadId}/participants\n  method: get\n  operationId: ChatThread_ListChatParticipants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chat/threads/{chatThreadId}/participants/:remove\n  method: post\n  operationId: ChatThread_RemoveChatParticipant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chat/threads/{chatThreadId}/participants/:add\n  method: post\n  operationId: ChatThread_AddChatParticipants\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chat/threads\n  method: post\n  operationId: Chat_CreateChatThread\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chat/threads\n  method: get\n  operationId: Chat_ListChatThreads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chat/threads/{chatThreadId}\n  method: patch\n  operationId: ChatThread_UpdateChatThreadProperties\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chat/threads/{chatThreadId}\n  method: get\n  operationId: ChatThread_GetChatThreadProperties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chat/threads/{chatThreadId}\n  method: delete\n  operationId: Chat_DeleteChatThread\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chat/threads/{chatThreadId}/typing\n  method: post\n  operationId: ChatThread_SendTypingNotification\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n     \
  \ purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sms\n  method: post\n  operationId: Sms_Send\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sms/optouts:add\n  method: post\n  operationId: OptOuts_Add\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /sms/optouts:remove\n  method: post\n  operationId: OptOuts_Remove\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sms/optouts:check\n  method: post\n  operationId: OptOuts_Check\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deliveryReports/{outgoingMessageId}\n  method: get\n  operationId: DeliveryReports_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/microsoft-skype/agentic-access/microsoft-skype-agentic-access.yml
summary_line: 21 operations · 14 acting · 1 human-in-the-loop
tags:
- Communications
- Messaging
- Microsoft
- Video
- Voice
---
