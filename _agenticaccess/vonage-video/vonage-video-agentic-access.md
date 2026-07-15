---
acting_count: 24
action_class_counts:
  acting: 24
  connected: 9
api_specs:
- filename: vonage-video-openapi.yml
  format: yaml
  label: Vonage Video Sessions API
  slug: vonage-video-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vonage-video/refs/heads/main/openapi/vonage-video-openapi.yml
- filename: vonage-video-openapi.yml
  format: yaml
  label: Vonage Video Streams & Signaling API
  slug: vonage-video-streams-signaling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vonage-video/refs/heads/main/openapi/vonage-video-openapi.yml
- filename: vonage-video-openapi.yml
  format: yaml
  label: Vonage Video Archives API
  slug: vonage-video-archives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vonage-video/refs/heads/main/openapi/vonage-video-openapi.yml
- filename: vonage-video-openapi.yml
  format: yaml
  label: Vonage Video Broadcasts API
  slug: vonage-video-broadcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vonage-video/refs/heads/main/openapi/vonage-video-openapi.yml
- filename: vonage-video-openapi.yml
  format: yaml
  label: Vonage Video SIP & Render API
  slug: vonage-video-sip-render-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vonage-video/refs/heads/main/openapi/vonage-video-openapi.yml
- filename: vonage-video-openapi.yml
  format: yaml
  label: Vonage Video Webhooks API
  slug: vonage-video-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vonage-video/refs/heads/main/openapi/vonage-video-openapi.yml
consequence_counts:
  physical: 2
  read: 9
  safety-critical: 4
  write: 18
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 4
kind: agentic-access
layout: agentic-access
method: generated
name: Vonage Video Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /project/{applicationId}/archive/{archiveId}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /project/{applicationId}/broadcast/{broadcastId}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /project/{applicationId}/captions/{captionsId}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /project/{applicationId}/render/{renderId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /project/{applicationId}/session/{sessionId}/connection/{connectionId}/signal
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /project/{applicationId}/session/{sessionId}/signal
operation_count: 33
overview: 'Vonage Video API exposes 33 API operations that an AI agent could call, of which 24 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 18 write, 2 physical, and 4 safety-critical.


  4 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Vonage Video API
provider_slug: vonage-video
slug: vonage-video-agentic-access
source_filename: vonage-video-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/vonage-video-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 33\n  by_action_class:\n    acting: 24\n    connected: 9\n  by_consequence:\n    write: 18\n    read: 9\n    physical: 2\n    safety-critical: 4\n  human_in_the_loop_required: 4\noperations:\n- path: /session/create\n  method: post\n  operationId: createSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /project/{applicationId}/session/{sessionId}/connection\n  method: get\n\
  \  operationId: listConnections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /project/{applicationId}/session/{sessionId}/connection/{connectionId}\n  method: delete\n  operationId: forceDisconnect\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /project/{applicationId}/session/{sessionId}/migrate\n  method: post\n  operationId: migrateSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /project/{applicationId}/session/{sessionId}/stream\n\
  \  method: get\n  operationId: listStreams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /project/{applicationId}/session/{sessionId}/stream\n  method: put\n  operationId: setStreamClassLists\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /project/{applicationId}/session/{sessionId}/stream/{streamId}\n  method: get\n  operationId: getStream\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /project/{applicationId}/session/{sessionId}/mute\n  method: post\n  operationId: muteSession\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /project/{applicationId}/session/{sessionId}/stream/{streamId}/mute\n  method: post\n  operationId: muteStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /project/{applicationId}/session/{sessionId}/signal\n  method: post\n  operationId: signalSession\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /project/{applicationId}/session/{sessionId}/connection/{connectionId}/signal\n  method: post\n  operationId: signalConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /project/{applicationId}/archive\n  method: get\n  operationId: listArchives\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /project/{applicationId}/archive\n  method: post\n  operationId: startArchive\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /project/{applicationId}/archive/{archiveId}\n  method: get\n  operationId: getArchive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /project/{applicationId}/archive/{archiveId}\n  method: delete\n  operationId: deleteArchive\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /project/{applicationId}/archive/{archiveId}/stop\n  method: post\n  operationId: stopArchive\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n    \
  \  exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /project/{applicationId}/archive/{archiveId}/layout\n  method: put\n  operationId: setArchiveLayout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /project/{applicationId}/archive/{archiveId}/streams\n  method: patch\n  operationId: selectArchiveStreams\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /project/{applicationId}/broadcast\n  method: get\n  operationId:\
  \ listBroadcasts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /project/{applicationId}/broadcast\n  method: post\n  operationId: startBroadcast\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /project/{applicationId}/broadcast/{broadcastId}\n  method: get\n  operationId: getBroadcast\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /project/{applicationId}/broadcast/{broadcastId}/stop\n  method: post\n  operationId: stopBroadcast\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /project/{applicationId}/broadcast/{broadcastId}/layout\n  method: put\n  operationId: setBroadcastLayout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /project/{applicationId}/broadcast/{broadcastId}/streams\n  method: patch\n  operationId: selectBroadcastStreams\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /project/{applicationId}/dial\n\
  \  method: post\n  operationId: dial\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /project/{applicationId}/session/{sessionId}/play-dtmf\n  method: post\n  operationId: playDtmfAll\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /project/{applicationId}/session/{sessionId}/connection/{connectionId}/play-dtmf\n  method: post\n  operationId: playDtmfConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /project/{applicationId}/captions/{captionsId}/start\n  method: post\n  operationId: startCaptions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /project/{applicationId}/captions/{captionsId}/stop\n  method: post\n  operationId: stopCaptions\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /project/{applicationId}/render\n  method: get\n  operationId: listRenders\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /project/{applicationId}/render\n  method: post\n  operationId: startRender\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /project/{applicationId}/render/{renderId}\n  method: get\n  operationId: getRender\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /project/{applicationId}/render/{renderId}\n  method: delete\n  operationId: stopRender\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n\
  \      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vonage-video/refs/heads/main/agentic-access/vonage-video-agentic-access.yml
summary_line: 33 operations · 24 acting · 4 human-in-the-loop
tags:
- Video
- WebRTC
- Live Streaming
- Real-Time Communications
- CPaaS
---
