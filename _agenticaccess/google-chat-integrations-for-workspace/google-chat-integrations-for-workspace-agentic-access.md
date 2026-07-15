---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 5
api_specs:
- filename: google-chat-integrations-for-workspace-openapi.yml
  format: yaml
  label: Google Chat API
  slug: chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-chat-integrations-for-workspace/refs/heads/main/openapi/google-chat-integrations-for-workspace-openapi.yml
consequence_counts:
  physical: 1
  read: 5
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Google Chat Integrations For Workspace Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/{parent}/members
operation_count: 10
overview: 'Google Chat Integrations for Workspace exposes 10 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read, 4 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Google Chat Integrations for Workspace
provider_slug: google-chat-integrations-for-workspace
slug: google-chat-integrations-for-workspace-agentic-access
source_filename: google-chat-integrations-for-workspace-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/google-chat-integrations-for-workspace-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    acting: 5\n    connected: 5\n  by_consequence:\n    write: 4\n    read: 5\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/spaces\n  method: post\n  operationId: createSpace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - chat.messages\n    - chat.spaces\n- path: /v1/spaces\n  method: get\n\
  \  operationId: listSpaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - chat.messages\n    - chat.spaces\n- path: /v1/{name}\n  method: get\n  operationId: getSpace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - chat.messages\n    - chat.spaces\n- path: /v1/{parent}/messages\n  method: post\n  operationId: createMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - chat.messages\n    - chat.spaces\n- path: /v1/{parent}/messages\n  method: get\n  operationId: listMessages\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - chat.messages\n    - chat.spaces\n- path: /v1/{name}/message\n  method: delete\n  operationId: deleteMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - chat.messages\n    - chat.spaces\n- path: /v1/{parent}/members\n  method: post\n  operationId: createMembership\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - chat.messages\n\
  \    - chat.spaces\n- path: /v1/{parent}/members\n  method: get\n  operationId: listMemberships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - chat.messages\n    - chat.spaces\n- path: /v1/{parent}/reactions\n  method: post\n  operationId: createReaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - chat.messages\n    - chat.spaces\n- path: /v1/customEmojis\n  method: get\n  operationId: listCustomEmojis\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - chat.messages\n    - chat.spaces\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-chat-integrations-for-workspace/refs/heads/main/agentic-access/google-chat-integrations-for-workspace-agentic-access.yml
summary_line: 10 operations · 5 acting
tags:
- Google Workspace
- Team Chat
- Messaging
- Collaboration
- Chat Apps
- Spaces
- Slash Commands
- Bots
---
