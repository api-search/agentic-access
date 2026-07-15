---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 6
api_specs:
- filename: vdocipher-openapi.yml
  format: yaml
  label: VdoCipher Videos API
  slug: vdocipher-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vdocipher/refs/heads/main/openapi/vdocipher-openapi.yml
- filename: vdocipher-openapi.yml
  format: yaml
  label: VdoCipher Upload API
  slug: vdocipher-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vdocipher/refs/heads/main/openapi/vdocipher-openapi.yml
- filename: vdocipher-openapi.yml
  format: yaml
  label: VdoCipher OTP & Playback Credentials API
  slug: vdocipher-playback-otp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vdocipher/refs/heads/main/openapi/vdocipher-openapi.yml
- filename: vdocipher-openapi.yml
  format: yaml
  label: VdoCipher Folders API
  slug: vdocipher-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vdocipher/refs/heads/main/openapi/vdocipher-openapi.yml
- filename: vdocipher-openapi.yml
  format: yaml
  label: VdoCipher Watermark API
  slug: vdocipher-watermark-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vdocipher/refs/heads/main/openapi/vdocipher-openapi.yml
- filename: vdocipher-openapi.yml
  format: yaml
  label: VdoCipher Meta & Files API
  slug: vdocipher-meta-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vdocipher/refs/heads/main/openapi/vdocipher-openapi.yml
consequence_counts:
  read: 6
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Vdocipher Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'VdoCipher exposes 12 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: VdoCipher
provider_slug: vdocipher
slug: vdocipher-agentic-access
source_filename: vdocipher-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/vdocipher-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 6\n    acting: 6\n  by_consequence:\n    read: 6\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /videos\n  method: get\n  operationId: listVideos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /videos\n  method: put\n  operationId: obtainUploadCredentials\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /videos/{videoId}\n  method: get\n  operationId: getVideoStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /videos/{videoId}\n  method: post\n  operationId: editVideoMeta\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /videos/{videoId}\n  method: delete\n  operationId: deleteVideos\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /videos/{videoId}/otp\n  method: post\n  operationId: generateOtp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /videos/{videoId}/files\n  method: get\n  operationId: listVideoFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /meta/{videoId}\n  method: get\n  operationId: getVideoMeta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /videos/tags\n  method: get\n  operationId: listTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /videos/folders\n  method: get\n  operationId: listFolders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /videos/folders\n  method: post\n  operationId: createFolder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /videos/folders/search\n  method: post\n  operationId: searchFolders\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vdocipher/refs/heads/main/agentic-access/vdocipher-agentic-access.yml
summary_line: 12 operations · 6 acting
tags:
- Video
- Secure Video Hosting
- DRM
- Streaming
- E-Learning
- OTT
- Watermarking
---
