---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 11
api_specs:
- filename: ready-player-me-avatars-api-openapi.yml
  format: yaml
  label: Ready Player Me Avatars API
  slug: ready-player-me-avatars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ready-player-me/refs/heads/main/openapi/ready-player-me-avatars-api-openapi.yml
- filename: ready-player-me-assets-api-openapi.yml
  format: yaml
  label: Ready Player Me Assets API
  slug: ready-player-me-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ready-player-me/refs/heads/main/openapi/ready-player-me-assets-api-openapi.yml
- filename: ready-player-me-auth-api-openapi.yml
  format: yaml
  label: Ready Player Me Auth API
  slug: ready-player-me-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ready-player-me/refs/heads/main/openapi/ready-player-me-auth-api-openapi.yml
consequence_counts:
  read: 11
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ready Player Me Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 23
overview: 'Ready Player Me exposes 23 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 12 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Ready Player Me
provider_slug: ready-player-me
slug: ready-player-me-agentic-access
source_filename: ready-player-me-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/ready-player-me-assets-api-openapi.yml, openapi/ready-player-me-auth-api-openapi.yml,\n  openapi/ready-player-me-avatars-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 11\n    acting: 12\n  by_consequence:\n    read: 11\n    write: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/assets\n  method: get\n  operationId: listAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/assets/{assetId}.glb\n  method: get\n  operationId: getAssetGlb\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/assets/{assetId}/thumbnail.png\n  method: get\n  operationId: getAssetThumbnail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/phoenix-assets\n  method: get\n  operationId: listPhoenixAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/users\n  method: post\n  operationId: createAnonymousUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/start\n  method: post\n  operationId: authStart\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/login\n  method: post\n  operationId: authLogin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/refresh\n  method: post\n  operationId: authRefresh\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/token\n  method: post\n  operationId: getAvatarToken\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/avatars\n  method: post\n  operationId: createAvatar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/avatars/templates\n  method: get\n  operationId: listAvatarTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/avatars/templates/{templateId}\n  method: post\n  operationId: createAvatarFromTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/avatars/{avatarId}\n  method: get\n  operationId: getAvatarMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/avatars/{avatarId}\n  method: patch\n  operationId: updateAvatar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/avatars/{avatarId}\n  method: put\n  operationId: saveAvatar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/avatars/{avatarId}\n  method: delete\n  operationId: deleteAvatar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/avatars/{avatarId}/draft\n  method: delete\n  operationId: deleteAvatarDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/avatars/{avatarId}/precompile\n  method: post\n  operationId: precompileAvatar\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/avatars/{avatarId}/colors\n  method: get\n  operationId: getAvatarColors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/avatars\n  method: get\n  operationId: listUserAvatars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/avatars/{avatarId}.glb\n  method: get\n  operationId: getAvatarGlb\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/avatars/{avatarId}.png\n  method: get\n  operationId: getAvatarPng\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/avatars/{avatarId}.glb\n  method: get\n  operationId: getAvatarGlbV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ready-player-me/refs/heads/main/agentic-access/ready-player-me-agentic-access.yml
summary_line: 23 operations · 12 acting
tags:
- Avatars
- 3D
- Gaming
- VR
- AR
- Metaverse
- glTF
- Cross-Platform
- Unity
- Unreal
- Web
- Mobile
---
