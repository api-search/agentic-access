---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 2
api_specs:
- filename: bytark-openapi.yml
  format: yaml
  label: ByteArk Stream Video API
  slug: bytark-stream-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytark/refs/heads/main/openapi/bytark-openapi.yml
- filename: bytark-openapi.yml
  format: yaml
  label: ByteArk Live Streaming API
  slug: bytark-live-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytark/refs/heads/main/openapi/bytark-openapi.yml
- filename: bytark-openapi.yml
  format: yaml
  label: ByteArk Storage API
  slug: bytark-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytark/refs/heads/main/openapi/bytark-openapi.yml
- filename: bytark-openapi.yml
  format: yaml
  label: ByteArk CDN API
  slug: bytark-cdn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytark/refs/heads/main/openapi/bytark-openapi.yml
- filename: bytark-openapi.yml
  format: yaml
  label: ByteArk Player API
  slug: bytark-player-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytark/refs/heads/main/openapi/bytark-openapi.yml
consequence_counts:
  read: 2
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bytark Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'ByteArk exposes 7 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ByteArk
provider_slug: bytark
slug: bytark-agentic-access
source_filename: bytark-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/bytark-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 2\n    acting: 5\n  by_consequence:\n    read: 2\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /videos\n  method: get\n  operationId: listVideos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /videos\n  method: post\n  operationId: createVideos\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /videos/{videoKey}\n  method: get\n  operationId: getVideo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /upload/v1/form-data/videos/{videoKey}\n  method: post\n  operationId: uploadVideoFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{serviceId}/{apiKey}/createchannel\n  method: post\n  operationId: createLiveChannel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n \
  \   audit: required\n- path: /{serviceId}/{apiKey}/listchannels\n  method: post\n  operationId: listLiveChannels\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{serviceId}/{apiKey}/deletechannel\n  method: post\n  operationId: deleteLiveChannel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bytark/refs/heads/main/agentic-access/bytark-agentic-access.yml
summary_line: 7 operations · 5 acting
tags:
- Video
- Streaming
- Video on Demand
- Live Streaming
- CDN
- Object Storage
- Transcoding
- DRM
- Media
---
