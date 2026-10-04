---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 2
api_specs:
- filename: nexar-citystream-live-feed-api-v4-api-openapi.yml
  format: yaml
  label: Nexar CityStream™ Live Feed API V4 API
  slug: nexar-citystream-live-feed-api-v4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexar/refs/heads/main/openapi/nexar-citystream-live-feed-api-v4-api-openapi.yml
- filename: nexar-get-a-collection-of-road-signs-api-openapi.yml
  format: yaml
  label: Nexar Get a collection of road signs API
  slug: nexar-get-a-collection-of-road-signs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexar/refs/heads/main/openapi/nexar-get-a-collection-of-road-signs-api-openapi.yml
- filename: nexar-get-a-collection-of-work-zones-api-openapi.yml
  format: yaml
  label: Nexar Get a collection of work zones API
  slug: nexar-get-a-collection-of-work-zones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexar/refs/heads/main/openapi/nexar-get-a-collection-of-work-zones-api-openapi.yml
- filename: nexar-get-a-specific-work-zone-api-openapi.yml
  format: yaml
  label: Nexar Get a specific work zone API
  slug: nexar-get-a-specific-work-zone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexar/refs/heads/main/openapi/nexar-get-a-specific-work-zone-api-openapi.yml
- filename: nexar-get-the-details-of-a-specific-road-sign-api-openapi.yml
  format: yaml
  label: Nexar Get the details of a specific road sign API
  slug: nexar-get-the-details-of-a-specific-road-sign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexar/refs/heads/main/openapi/nexar-get-the-details-of-a-specific-road-sign-api-openapi.yml
- filename: nexar-virtualcam-api-api-openapi.yml
  format: yaml
  label: Nexar VirtualCam API
  slug: nexar-virtualcam-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexar/refs/heads/main/openapi/nexar-virtualcam-api-api-openapi.yml
consequence_counts:
  read: 2
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Nexar Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Nexar exposes 8 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Nexar
provider_slug: nexar
slug: nexar-agentic-access
source_filename: nexar-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/nexar-citystream-live-feed-api-v4-api-openapi.yml, openapi/nexar-get-a-collection-of-road-signs-api-openapi.yml,\n  openapi/nexar-get-a-collection-of-work-zones-api-openapi.yml, openapi/nexar-get-a-specific-work-zone-api-openapi.yml,\n  openapi/nexar-get-the-details-of-a-specific-road-sign-api-openapi.yml, openapi/nexar-virtualcam-api-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 6\n    connected: 2\n  by_consequence:\n    write: 6\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/livefeed/v4/detections\n  method: post\n  operationId: CityStreamAPI_FindRealtimeDetections\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/roadinventory/v3/detections\n  method: post\n  operationId: NexarPlatformAPI_FindDetections\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/workzones/v3/detections\n  method: post\n  operationId: NexarPlatformAPI_FindDetections\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/workzones/v3/detections/single\n  method: post\n  operationId: NexarPlatformAPI_GetDetection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/roadinventory/v3/detections/single\n  method: post\n  operationId: NexarPlatformAPI_GetDetection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/virtualcam/v5/frames\n  method: post\n  operationId: VcamService_FindRawFrames\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/virtualcam/v4/coverage\n  method: post\n  operationId: VcamService_GetH3Coverage\n  x-agentic-access:\n   \
  \ action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/virtualcam/v4/frames\n  method: post\n  operationId: RoadItemService_FindRawFrames\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nexar/refs/heads/main/agentic-access/nexar-agentic-access.yml
summary_line: 8 operations · 6 acting
tags:
- Company
- Mapping
- Geospatial
- Transportation
- Computer Vision
- Autonomous Vehicles
- Smart Cities
- Imagery
- Road Data
- Machine Learning
---
