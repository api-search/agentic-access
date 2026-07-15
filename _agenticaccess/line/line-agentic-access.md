---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 3
api_specs:
- filename: messaging-api.yml
  format: yaml
  label: LINE Messaging API
  slug: messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/line/line-openapi/main/messaging-api.yml
- filename: liff.yml
  format: yaml
  label: LINE Front-end Framework (LIFF) Server API
  slug: liff
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/line/line-openapi/main/liff.yml
- filename: channel-access-token.yml
  format: yaml
  label: LINE Channel Access Token API
  slug: channel-access-token
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/line/line-openapi/main/channel-access-token.yml
- filename: insight.yml
  format: yaml
  label: LINE Insight API
  slug: insight
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/line/line-openapi/main/insight.yml
- filename: manage-audience.yml
  format: yaml
  label: LINE Manage Audience API
  slug: manage-audience
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/line/line-openapi/main/manage-audience.yml
- filename: shop.yml
  format: yaml
  label: LINE Shop (Mission Stickers) API
  slug: shop
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/line/line-openapi/main/shop.yml
consequence_counts:
  physical: 4
  read: 3
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Line Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /message/broadcast
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /message/multicast
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /message/push
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /message/reply
operation_count: 8
overview: 'LINE exposes 8 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read, 1 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: LINE
provider_slug: line
slug: line-agentic-access
source_filename: line-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/line-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 5\n    connected: 3\n  by_consequence:\n    physical: 4\n    read: 3\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /message/reply\n  method: post\n  operationId: replyMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /message/push\n  method: post\n  operationId: pushMessage\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /message/multicast\n  method: post\n  operationId: multicastMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /message/broadcast\n  method: post\n  operationId: broadcastMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profile/{userId}\n  method: get\n  operationId: getUserProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /channel/webhook/endpoint\n  method: get\n  operationId: getWebhookEndpoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /channel/webhook/endpoint\n  method: put\n  operationId: setWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /info\n  method: get\n  operationId: getBotInfo\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/line/refs/heads/main/agentic-access/line-agentic-access.yml
summary_line: 8 operations · 5 acting
tags:
- Messaging
- Chatbots
- Social Login
- Mini Apps
- Marketing
- Japan
---
