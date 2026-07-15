---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 5
api_specs:
- filename: akool-openapi.yml
  format: yaml
  label: Akool Talking Avatar API
  slug: akool-talking-avatar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akool/refs/heads/main/openapi/akool-openapi.yml
- filename: akool-openapi.yml
  format: yaml
  label: Akool Talking Photo API
  slug: akool-talking-photo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akool/refs/heads/main/openapi/akool-openapi.yml
- filename: akool-openapi.yml
  format: yaml
  label: Akool Face Swap API
  slug: akool-face-swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akool/refs/heads/main/openapi/akool-openapi.yml
- filename: akool-openapi.yml
  format: yaml
  label: Akool Video Translation API
  slug: akool-video-translation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akool/refs/heads/main/openapi/akool-openapi.yml
- filename: akool-openapi.yml
  format: yaml
  label: Akool Image Generation API
  slug: akool-image-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akool/refs/heads/main/openapi/akool-openapi.yml
- filename: akool-openapi.yml
  format: yaml
  label: Akool Live Avatar (Streaming) API
  slug: akool-live-avatar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akool/refs/heads/main/openapi/akool-openapi.yml
consequence_counts:
  read: 5
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Akool Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'Akool exposes 13 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Akool
provider_slug: akool
slug: akool-agentic-access
source_filename: akool-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/akool-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    acting: 8\n    connected: 5\n  by_consequence:\n    write: 8\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /api/open/v3/getToken\n  method: post\n  operationId: getToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/open/v3/talkingavatar/create\n  method: post\n  operationId: createTalkingAvatar\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/open/v3/content/video/createbytalkingphoto\n  method: post\n  operationId: createByTalkingPhoto\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/open/v3/content/video/infobymodelid\n  method: get\n  operationId: getVideoInfoByModelId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/open/v4/faceswap/faceswapPlusByImage\n  method: post\n  operationId: faceSwapPlusByImage\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/open/v3/faceswap/result/listbyids\n  method: get\n  operationId: listFaceSwapResultsByIds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/open/v3/language/list\n  method: get\n  operationId: listTranslationLanguages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/open/v3/content/video/createbytranslate\n  method: post\n  operationId: createByTranslate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/open/v4/content/image/createBySourcePrompt\n  method: post\n  operationId: createImageBySourcePrompt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/open/v3/content/image/infobymodelid\n  method: get\n  operationId: getImageInfoByModelId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/open/v4/liveAvatar/avatar/list\n  method: get\n  operationId: listLiveAvatars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/open/v4/liveAvatar/session/create\n  method: post\n  operationId: createLiveAvatarSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/open/v4/liveAvatar/session/close\n  method: post\n  operationId: closeLiveAvatarSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/akool/refs/heads/main/agentic-access/akool-agentic-access.yml
summary_line: 13 operations · 8 acting
tags:
- AI Avatars
- Video Generation
- AI Video
- Face Swap
- Generative AI
- Talking Avatar
- Video Translation
- Live Avatar
---
