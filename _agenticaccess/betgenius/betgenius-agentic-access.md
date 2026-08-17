---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 5
api_specs:
- filename: betgenius-booking-v2-openapi.yml
  format: yaml
  label: BetGenius Booking API V2
  slug: betgenius-booking-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/betgenius/refs/heads/main/openapi/betgenius-booking-v2-openapi.yml
- filename: betgenius-booking-v1-openapi.yml
  format: yaml
  label: BetGenius Booking API V1
  slug: betgenius-booking-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/betgenius/refs/heads/main/openapi/betgenius-booking-v1-openapi.yml
- filename: betgenius-video-v3-openapi.yml
  format: yaml
  label: BetGenius Video Streaming API v3
  slug: betgenius-video-streaming-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/betgenius/refs/heads/main/openapi/betgenius-video-v3-openapi.yml
consequence_counts:
  read: 5
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Betgenius Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'BetGenius exposes 13 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BetGenius
provider_slug: betgenius
slug: betgenius-agentic-access
source_filename: betgenius-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: generated\nsource: openapi/betgenius-booking-v1-openapi.yml, openapi/betgenius-booking-v2-openapi.yml,\n  openapi/betgenius-video-v3-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    acting: 8\n    connected: 5\n  by_consequence:\n    write: 8\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /api/booking/Book\n  method: post\n  operationId: BookingV1_Book\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/booking/UnBook\n\
  \  method: post\n  operationId: BookingV1_UnBook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/booking/Fixtures\n  method: get\n  operationId: BookingV1_Fixtures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/booking/Book\n  method: post\n  operationId: BookingV2_Book\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/booking/UnBook\n  method: post\n  operationId: BookingV2_UnBook\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/booking/Fixtures\n  method: get\n  operationId: BookingV2_Fixtures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fixtures\n  method: get\n  operationId: getFixtures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fixtures/{id}\n  method: get\n  operationId: getFixture\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fixtures/{id}/live-streams/{streamId}/deliveries/dash/{deliveryId}\n  method: post\n\
  \  operationId: createDASHStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fixtures/{id}/live-streams/{streamId}/deliveries/hls/{deliveryId}\n  method: post\n  operationId: createHLSStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fixtures/{id}/live-streams/{streamId}/deliveries/srt/{deliveryId}\n  method: post\n  operationId: createSRTStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fixtures/{id}/vod-streams/{streamId}/deliveries/hls/{deliveryId}\n  method: post\n  operationId: createHlsVod\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /regions\n  method: get\n  operationId: getRegions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/betgenius/refs/heads/main/agentic-access/betgenius-agentic-access.yml
summary_line: 13 operations · 8 acting
tags:
- Sportsbook
- Sports Betting
- Sports Data
- Odds Feeds
- Trading Services
- Risk Management
- Live Streaming
- In-Play Betting
- BetBuilder
- Player Engagement
- Marketing Technology
- Gambling
---
