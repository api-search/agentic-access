---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 11
api_specs:
- filename: restream-openapi.yml
  format: yaml
  label: Restream API
  slug: restream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/restream/refs/heads/main/openapi/restream-openapi.yml
consequence_counts:
  read: 11
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Restream Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'Restream exposes 14 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Restream
provider_slug: restream
slug: restream-agentic-access
source_filename: restream-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/restream-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 11\n    acting: 3\n  by_consequence:\n    read: 11\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /platform/all\n  method: get\n  operationId: listPlatforms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/profile\n  method: get\n  operationId: getUserProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - profile.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/streamKey\n\
  \  method: get\n  operationId: getStreamKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - stream.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/channel/all\n  method: get\n  operationId: listChannels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - channels.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/channel/{id}\n  method: get\n  operationId: getChannel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - channels.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/channel/{id}\n  method: patch\n  operationId: updateChannel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - channels.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/channel/{id}/meta\n  method: get\n  operationId: getChannelMeta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - channels.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/channel/{id}/meta\n  method: patch\n  operationId: updateChannelMeta\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - channels.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/event/upcoming\n  method: get\n  operationId: listUpcomingEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - events.read\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /user/event/in-progress\n  method: get\n  operationId: listInProgressEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - events.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/event/history\n  method: get\n  operationId: listEventHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - events.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/event/{id}\n  method: get\n  operationId: getEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - events.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/event/{id}/streamKey\n  method: get\n  operationId: getEventStreamKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - events.read\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /oauth/token\n  method: post\n  operationId: refreshToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/restream/refs/heads/main/agentic-access/restream-agentic-access.yml
summary_line: 14 operations · 3 acting
tags:
- Broadcast
- Chat
- Content Delivery
- Live Streaming
- Multistreaming
- Video Streaming
---
