---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 8
api_specs:
- filename: dacast-openapi.yml
  format: yaml
  label: Dacast VOD API
  slug: dacast-vod-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dacast/refs/heads/main/openapi/dacast-openapi.yml
- filename: dacast-openapi.yml
  format: yaml
  label: Dacast Live Channels API
  slug: dacast-live-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dacast/refs/heads/main/openapi/dacast-openapi.yml
- filename: dacast-openapi.yml
  format: yaml
  label: Dacast Playlists API
  slug: dacast-playlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dacast/refs/heads/main/openapi/dacast-openapi.yml
- filename: dacast-openapi.yml
  format: yaml
  label: Dacast Analytics API
  slug: dacast-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dacast/refs/heads/main/openapi/dacast-openapi.yml
consequence_counts:
  read: 8
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Dacast Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 19
overview: 'Dacast exposes 19 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 11 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Dacast
provider_slug: dacast
slug: dacast-agentic-access
source_filename: dacast-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/dacast-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    acting: 11\n    connected: 8\n  by_consequence:\n    write: 11\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/vod\n  method: post\n  operationId: createVodUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/vod\n  method: get\n  operationId: listVideos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/vod/{videoId}\n  method: get\n  operationId: lookupVideo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/vod/{videoId}\n  method: delete\n  operationId: deleteVideoSource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/vod/{videoId}/rendition/{renditionId}\n  method: delete\n  operationId: deleteRendition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v2/vod/upload/multipart\n  method: post\n  operationId: initiateMultipartUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/channel\n  method: post\n  operationId: createChannel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/channel\n  method: get\n  operationId: listChannels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/channel/{channelId}\n  method: get\n  operationId:\
  \ lookupStream\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/channel/{channelId}/ingest\n  method: put\n  operationId: switchStreamIngest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/channel/{channelId}/type\n  method: put\n  operationId: changeChannelType\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/channel/online\n  method: get\n  operationId: listOnlineStreams\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/channel/{channelId}/simulcast\n  method: get\n  operationId: listSimulcastDestinations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/channel/{channelId}/simulcast\n  method: post\n  operationId: addSimulcastDestination\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/channel/{channelId}/simulcast/{destinationId}\n  method: delete\n  operationId: deleteSimulcastDestination\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n  \
  \  escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/playlist\n  method: post\n  operationId: createPlaylist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/playlist/{playlistId}\n  method: get\n  operationId: getPlaylist\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/playlist/{playlistId}\n  method: put\n  operationId: setPlaylistContent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v2/analytics\n  method: get\n  operationId: getAnalytics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dacast/refs/heads/main/agentic-access/dacast-agentic-access.yml
summary_line: 19 operations · 11 acting
tags:
- Live Streaming
- Video
- VOD
- OTT
- Video Hosting
- Media
- Analytics
---
