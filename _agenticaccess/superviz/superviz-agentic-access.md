---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 5
api_specs:
- filename: superviz-openapi.yml
  format: yaml
  label: SuperViz Participants API
  slug: superviz-participants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superviz/refs/heads/main/openapi/superviz-openapi.yml
- filename: superviz-openapi.yml
  format: yaml
  label: SuperViz Channels API
  slug: superviz-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superviz/refs/heads/main/openapi/superviz-openapi.yml
- filename: superviz-openapi.yml
  format: yaml
  label: SuperViz Realtime Data API
  slug: superviz-realtime-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superviz/refs/heads/main/openapi/superviz-openapi.yml
- filename: superviz-openapi.yml
  format: yaml
  label: SuperViz Rooms API
  slug: superviz-rooms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superviz/refs/heads/main/openapi/superviz-openapi.yml
- filename: superviz-openapi.yml
  format: yaml
  label: SuperViz Contextual Comments API
  slug: superviz-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superviz/refs/heads/main/openapi/superviz-openapi.yml
- filename: superviz-openapi.yml
  format: yaml
  label: SuperViz Meetings API
  slug: superviz-meetings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superviz/refs/heads/main/openapi/superviz-openapi.yml
- filename: superviz-openapi.yml
  format: yaml
  label: SuperViz Webhooks API
  slug: superviz-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superviz/refs/heads/main/openapi/superviz-openapi.yml
- filename: superviz-openapi.yml
  format: yaml
  label: SuperViz Authentication API
  slug: superviz-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superviz/refs/heads/main/openapi/superviz-openapi.yml
consequence_counts:
  read: 5
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Superviz Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'SuperViz exposes 6 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SuperViz
provider_slug: superviz
slug: superviz-agentic-access
source_filename: superviz-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/superviz-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 5\n    acting: 1\n  by_consequence:\n    read: 5\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /realtime/1.0/participants/{channel}\n  method: get\n  operationId: getChannelParticipants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /realtime/1.0/channels\n  method: get\n  operationId: listChannels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /realtime/1.0/channels/{channel}/events\n  method: post\n  operationId: publishEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rooms/{roomId}/participants\n  method: get\n  operationId: getRoomParticipants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rooms/{roomId}/comments\n  method: get\n  operationId: listRoomComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /meetings/{meetingId}\n  method: get\n  operationId: getMeetingStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/superviz/refs/heads/main/agentic-access/superviz-agentic-access.yml
summary_line: 6 operations · 1 acting
tags:
- Real Time
- Collaboration
- Presence
- Synchronization
- Video
- WebRTC
- SDK
---
