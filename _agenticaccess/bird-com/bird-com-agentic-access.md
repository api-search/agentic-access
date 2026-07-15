---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 11
api_specs:
- filename: bird-com-openapi.yml
  format: yaml
  label: Bird Channels / Messaging API
  slug: bird-channels-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bird-com/refs/heads/main/openapi/bird-com-openapi.yml
- filename: bird-com-openapi.yml
  format: yaml
  label: Bird Contacts API
  slug: bird-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bird-com/refs/heads/main/openapi/bird-com-openapi.yml
- filename: bird-com-openapi.yml
  format: yaml
  label: Bird Conversations API
  slug: bird-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bird-com/refs/heads/main/openapi/bird-com-openapi.yml
- filename: bird-com-openapi.yml
  format: yaml
  label: Bird Numbers API
  slug: bird-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bird-com/refs/heads/main/openapi/bird-com-openapi.yml
- filename: bird-com-openapi.yml
  format: yaml
  label: Legacy MessageBird REST API
  slug: bird-legacy-messagebird-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bird-com/refs/heads/main/openapi/bird-com-openapi.yml
consequence_counts:
  physical: 4
  read: 11
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bird Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /messages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /verify
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /workspaces/{workspaceId}/channels/{channelId}/messages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /workspaces/{workspaceId}/conversations/{conversationId}/messages
operation_count: 21
overview: 'Bird exposes 21 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 6 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bird
provider_slug: bird-com
slug: bird-com-agentic-access
source_filename: bird-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/bird-com-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    acting: 10\n    connected: 11\n  by_consequence:\n    physical: 4\n    read: 11\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /workspaces/{workspaceId}/channels/{channelId}/messages\n  method: post\n  operationId: sendChannelMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /workspaces/{workspaceId}/channels/{channelId}/messages\n  method: get\n  operationId: listChannelMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}/channel-media/presigned-upload\n  method: post\n  operationId: createPresignedUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/channels\n  method: get\n  operationId: listChannels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}/channels/{channelId}\n  method: get\n  operationId: getChannel\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}/contacts\n  method: post\n  operationId: createContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/contacts\n  method: get\n  operationId: listContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}/contacts/{contactId}\n  method: get\n  operationId: getContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}/contacts/{contactId}\n\
  \  method: patch\n  operationId: updateContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/contacts/{contactId}\n  method: delete\n  operationId: deleteContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/conversations\n  method: post\n  operationId: createConversation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/conversations/{conversationId}/messages\n  method: post\n  operationId: createConversationMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/conversations/{conversationId}/messages/{messageId}\n  method: get\n  operationId: getConversationMessage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}/numbers\n  method: get\n  operationId: listNumbers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}/network-lookup\n  method: post\n  operationId: numberLookup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages\n  method: post\n  operationId: legacyCreateMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages\n  method: get\n  operationId: legacyListMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /messages/{id}\n  method: get\n  operationId: legacyGetMessage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lookup/{phoneNumber}\n  method: get\n  operationId: legacyLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /verify\n  method: post\n  operationId: legacyCreateVerify\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /voicemessages\n  method: get\n  operationId: legacyListVoiceMessages\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bird-com/refs/heads/main/agentic-access/bird-com-agentic-access.yml
summary_line: 21 operations · 10 acting
tags:
- CRM
- Messaging
- SMS
- WhatsApp
- Email
- Voice
- Omnichannel
- CPaaS
---
