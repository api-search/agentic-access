---
acting_count: 21
action_class_counts:
  acting: 21
  connected: 21
api_specs:
- filename: fastpix-openapi.yml
  format: yaml
  label: FastPix On-Demand API
  slug: fastpix-on-demand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastpix/refs/heads/main/openapi/fastpix-openapi.yml
- filename: fastpix-openapi.yml
  format: yaml
  label: FastPix Live Streaming API
  slug: fastpix-live-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastpix/refs/heads/main/openapi/fastpix-openapi.yml
- filename: fastpix-openapi.yml
  format: yaml
  label: FastPix Simulcast API
  slug: fastpix-simulcast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastpix/refs/heads/main/openapi/fastpix-openapi.yml
- filename: fastpix-openapi.yml
  format: yaml
  label: FastPix Playback & Signing Keys API
  slug: fastpix-playback-signing-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastpix/refs/heads/main/openapi/fastpix-openapi.yml
- filename: fastpix-openapi.yml
  format: yaml
  label: FastPix In-Video AI API
  slug: fastpix-in-video-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastpix/refs/heads/main/openapi/fastpix-openapi.yml
- filename: fastpix-openapi.yml
  format: yaml
  label: FastPix Data & Views API
  slug: fastpix-data-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastpix/refs/heads/main/openapi/fastpix-openapi.yml
consequence_counts:
  read: 21
  safety-critical: 1
  write: 20
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Fastpix Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /live/streams/{streamId}/simulcast/{simulcastId}
operation_count: 42
overview: 'FastPix exposes 42 API operations that an AI agent could call, of which 21 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read, 20 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: FastPix
provider_slug: fastpix
slug: fastpix-agentic-access
source_filename: fastpix-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/fastpix-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 42\n  by_action_class:\n    acting: 21\n    connected: 21\n  by_consequence:\n    write: 20\n    read: 21\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /on-demand\n  method: post\n  operationId: createMedia\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /on-demand\n  method: get\n  operationId: listMedia\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /on-demand/upload\n  method: post\n  operationId: createUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /on-demand/uploads\n  method: get\n  operationId: listUploads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /on-demand/upload/{uploadId}\n  method: put\n  operationId: cancelUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /on-demand/{mediaId}\n  method: get\n  operationId: getMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /on-demand/{mediaId}\n  method: patch\n  operationId: updateMedia\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /on-demand/{mediaId}\n  method: delete\n  operationId: deleteMedia\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /on-demand/{mediaId}/media-clips\n  method: get\n\
  \  operationId: listMediaClips\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /on-demand/{mediaId}/source\n  method: patch\n  operationId: updateSourceAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /on-demand/{mediaId}/update-mp4Support\n  method: patch\n  operationId: updateMp4Support\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /on-demand/{mediaId}/tracks\n  method: post\n  operationId: addMediaTrack\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /on-demand/{mediaId}/tracks/{trackId}\n  method: patch\n  operationId: updateMediaTrack\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /on-demand/{mediaId}/tracks/{trackId}\n  method: delete\n  operationId: deleteMediaTrack\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /on-demand/{mediaId}/tracks/{trackId}/generate-subtitle\n  method: post\n  operationId: generateSubtitleTrack\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /live/streams\n  method: post\n  operationId: createStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /live/streams\n  method: get\n  operationId: listStreams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /live/streams/{streamId}\n\
  \  method: get\n  operationId: getStream\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /live/streams/{streamId}\n  method: patch\n  operationId: updateStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /live/streams/{streamId}\n  method: delete\n  operationId: deleteStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /live/streams/{streamId}/live-clips\n  method: get\n  operationId: listLiveClips\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /live/streams/{streamId}/playback-ids\n  method: post\n  operationId: createStreamPlaybackId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /live/streams/{streamId}/playback-ids/{playbackId}\n  method: get\n  operationId: getStreamPlaybackId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /live/streams/{streamId}/playback-ids/{playbackId}\n  method: delete\n  operationId: deleteStreamPlaybackId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /live/streams/{streamId}/simulcast\n  method: post\n  operationId: createSimulcast\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /live/streams/{streamId}/simulcast/{simulcastId}\n  method: get\n  operationId: getSimulcast\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /live/streams/{streamId}/simulcast/{simulcastId}\n  method: patch\n  operationId: updateSimulcast\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /live/streams/{streamId}/simulcast/{simulcastId}\n  method: delete\n  operationId: deleteSimulcast\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /security/signing-keys\n  method: post\n  operationId: createSigningKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /security/signing-keys\n  method: get\n  operationId: listSigningKeys\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /security/signing-keys/{signingKeyId}\n  method: get\n  operationId: getSigningKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /security/signing-keys/{signingKeyId}\n  method: delete\n  operationId: deleteSigningKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /on-demand/drm-configurations\n  method: get\n  operationId: listDrmConfigurations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /on-demand/drm-configurations/{drmConfigurationId}\n  method: get\n  operationId: getDrmConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/dimensions\n  method: get\n  operationId: listDimensions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/dimensions/{dimensionId}\n  method: get\n  operationId: listDimensionValues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/views\n  method: get\n  operationId: listVideoViews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/views/{viewId}\n  method: get\n  operationId: getVideoView\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/errors\n  method: get\n  operationId: listErrors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/metrics/timeseries/{metricId}\n  method: get\n  operationId: getTimeseriesData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/metrics/breakdown/{metricId}\n  method: get\n  operationId: getMetricBreakdown\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/metrics/overall/{metricId}\n  method: get\n  operationId: getOverallMetric\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fastpix/refs/heads/main/agentic-access/fastpix-agentic-access.yml
summary_line: 42 operations · 21 acting · 1 human-in-the-loop
tags:
- Video
- Streaming
- Live Streaming
- Video on Demand
- Encoding
- Playback
- Video Analytics
---
