---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 11
api_specs:
- filename: reliance-jio-jioeventscpaasplatform-api-openapi.yml
  format: yaml
  label: Reliance Jio Events Cpaas Platform API
  slug: reliance-jio-jioeventscpaasplatform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reliance-jio/refs/heads/main/openapi/reliance-jio-jioeventscpaasplatform-api-openapi.yml
- filename: reliance-jio-jiomeetcpaasplatform-api-openapi.yml
  format: yaml
  label: Reliance Jio Meet Cpaas Platform API
  slug: reliance-jio-jiomeetcpaasplatform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reliance-jio/refs/heads/main/openapi/reliance-jio-jiomeetcpaasplatform-api-openapi.yml
consequence_counts:
  read: 11
  safety-critical: 1
  write: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Reliance Jio Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/platform/v1/recordings/stop
operation_count: 29
overview: 'Reliance Jio exposes 29 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 17 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Reliance Jio
provider_slug: reliance-jio
slug: reliance-jio-agentic-access
source_filename: reliance-jio-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/reliance-jio-jioeventscpaasplatform-api-openapi.yml, openapi/reliance-jio-jiomeetcpaasplatform-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 29\n  by_action_class:\n    acting: 18\n    connected: 11\n  by_consequence:\n    write: 17\n    read: 11\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /api/platform/v1/meetingInvite\n  method: post\n  operationId: postApiPlatformV1MeetingInvite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/platform/v1/sessions/{meetingId}/{sessionId}\n  method: delete\n  operationId: deleteApiPlatformV1SessionsByMeetingIdBySessionId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/platform/v1/sessions/{meetingId}\n  method: post\n  operationId: postApiPlatformV1SessionsByMeetingId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/platform/v1/sessions/{meetingId}\n  method: get\n  operationId: getApiPlatformV1SessionsByMeetingId\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/platform/v1/meetingInvite/{meetingId}\n  method: delete\n  operationId: deleteApiPlatformV1MeetingInviteByMeetingId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/platform/v1/meetingInvite/{meetingId}\n  method: get\n  operationId: getApiPlatformV1MeetingInviteByMeetingId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/platform/v1/schedule/webinar\n  method: delete\n  operationId: deleteApiPlatformV1ScheduleWebinar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/platform/v1/schedule/webinar\n  method: put\n  operationId: putApiPlatformV1ScheduleWebinar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/platform/v1/schedule/webinar\n  method: post\n  operationId: postApiPlatformV1ScheduleWebinar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/platform/v1/schedule/webinar\n  method: get\n  operationId:\
  \ getApiPlatformV1ScheduleWebinar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/platform/v1/webinar/{meetingId}/download\n  method: get\n  operationId: getApiPlatformV1WebinarByMeetingIdDownload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/meeting/meetingDetails/{meetingId}\n  method: get\n  operationId: getApiMeetingMeetingDetailsByMeetingId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/meeting/meetingDetails/{meetingId}\n  method: put\n  operationId: putApiMeetingMeetingDetailsByMeetingId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/meeting\n  method: post\n  operationId: postApiMeeting\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/oauth2/v2/token\n  method: post\n  operationId: postApiOauth2V2Token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/meeting/{userId}\n  method: get\n  operationId: getApiMeetingByUserId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/my_profile\n  method: get\n  operationId: getApiMyProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/meeting/cancel/{meetingId}\n  method: post\n  operationId: postApiMeetingCancelByMeetingId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/platform/v1/recordings/start\n  method: post\n  operationId: postApiPlatformV1RecordingsStart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    \
  \  - high-value\n    audit: required\n- path: /api/platform/v1/room\n  method: post\n  operationId: postApiPlatformV1Room\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/platform/v1/recordings/list\n  method: post\n  operationId: postApiPlatformV1RecordingsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/platform/v1/schedule/meeting\n  method: put\n  operationId: putApiPlatformV1ScheduleMeeting\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n     \
  \ - high-value\n    audit: required\n- path: /api/platform/v1/schedule/meeting\n  method: delete\n  operationId: deleteApiPlatformV1ScheduleMeeting\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/platform/v1/schedule/meeting\n  method: post\n  operationId: postApiPlatformV1ScheduleMeeting\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/platform/v1/schedule/meeting\n  method: get\n  operationId: getApiPlatformV1ScheduleMeeting\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/platform/v1/recordings/isrecording\n  method: post\n  operationId: postApiPlatformV1RecordingsIsrecording\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/platform/v1/recordings/stop\n  method: post\n  operationId: postApiPlatformV1RecordingsStop\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/platform/v1/analytics/report\n  method: get\n  operationId: getApiPlatformV1AnalyticsReport\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/platform/v1/chat/thread\n  method: get\n  operationId: getApiPlatformV1ChatThread\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reliance-jio/refs/heads/main/agentic-access/reliance-jio-agentic-access.yml
summary_line: 29 operations · 18 acting · 1 human-in-the-loop
tags:
- Telecommunications
- India
- Mobile Network Operator
- Network APIs
- CAMARA
- Open Gateway
- SIM Swap
- Identity Verification
- CPaaS
- Messaging
- Voice
- IoT
- Broadband
- 5G
- BSS
- OSS
- Standards
- Video Conferencing
---
