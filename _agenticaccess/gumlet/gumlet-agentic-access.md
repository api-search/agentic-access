---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 9
api_specs:
- filename: gumlet-openapi.yml
  format: yaml
  label: Gumlet Video Assets API
  slug: gumlet-video-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumlet/refs/heads/main/openapi/gumlet-openapi.yml
- filename: gumlet-openapi.yml
  format: yaml
  label: Gumlet Video Collections API
  slug: gumlet-video-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumlet/refs/heads/main/openapi/gumlet-openapi.yml
- filename: gumlet-openapi.yml
  format: yaml
  label: Gumlet Live Streaming API
  slug: gumlet-live-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumlet/refs/heads/main/openapi/gumlet-openapi.yml
- filename: gumlet-openapi.yml
  format: yaml
  label: Gumlet Image Optimization API
  slug: gumlet-image-optimization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumlet/refs/heads/main/openapi/gumlet-openapi.yml
- filename: gumlet-openapi.yml
  format: yaml
  label: Gumlet Analytics API
  slug: gumlet-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumlet/refs/heads/main/openapi/gumlet-openapi.yml
- filename: gumlet-openapi.yml
  format: yaml
  label: Gumlet Uploads API
  slug: gumlet-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumlet/refs/heads/main/openapi/gumlet-openapi.yml
consequence_counts:
  read: 9
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Gumlet Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 18
overview: 'Gumlet exposes 18 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 9 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Gumlet
provider_slug: gumlet
slug: gumlet-agentic-access
source_filename: gumlet-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/gumlet-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    acting: 9\n    connected: 9\n  by_consequence:\n    write: 9\n    read: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /video/assets\n  method: post\n  operationId: createAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /video/assets/list/{collection_id}\n  method: get\n  operationId: listAssets\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /video/assets/{asset_id}\n  method: get\n  operationId: getAsset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /video/assets/{asset_id}\n  method: put\n  operationId: updateAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /video/assets/{asset_id}\n  method: delete\n  operationId: deleteAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /video/assets/upload\n  method: post\n  operationId: createAssetDirectUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /video/sources\n  method: get\n  operationId: listCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /video/sources\n  method: post\n  operationId: createCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /video/sources/{video_source_id}\n  method:\
  \ get\n  operationId: getCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /video/live/assets\n  method: post\n  operationId: createLiveAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /video/live/assets/{live_asset_id}\n  method: get\n  operationId: getLiveAsset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /video/live/assets/{live_asset_id}\n  method: delete\n  operationId: deleteLiveAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sources\n  method: get\n  operationId: listSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sources\n  method: post\n  operationId: createSource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sources/{source_id}\n  method: get\n  operationId: getSource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sources/{source_id}\n  method: delete\n  operationId: deleteSource\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analytics/videos\n  method: get\n  operationId: getVideoAnalytics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/images\n  method: get\n  operationId: getImageAnalytics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gumlet/refs/heads/main/agentic-access/gumlet-agentic-access.yml
summary_line: 18 operations · 9 acting
tags:
- Video
- Streaming
- Image Optimization
- CDN
- Encoding
- Analytics
---
