---
acting_count: 28
action_class_counts:
  acting: 28
  connected: 16
api_specs:
- filename: kreatorflow-ai-audio-api-openapi.yml
  format: yaml
  label: kreatorflow-ai Audio API
  slug: kreatorflow-ai-audio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kreatorflow-ai/openapi/kreatorflow-ai-audio-api-openapi.yml
- filename: kreatorflow-ai-images-api-openapi.yml
  format: yaml
  label: kreatorflow-ai Images API
  slug: kreatorflow-ai-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kreatorflow-ai/openapi/kreatorflow-ai-images-api-openapi.yml
- filename: kreatorflow-ai-jobs-api-openapi.yml
  format: yaml
  label: kreatorflow-ai Jobs API
  slug: kreatorflow-ai-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kreatorflow-ai/openapi/kreatorflow-ai-jobs-api-openapi.yml
- filename: kreatorflow-ai-lip-sync-api-openapi.yml
  format: yaml
  label: kreatorflow-ai Lip Sync API
  slug: kreatorflow-ai-lip-sync-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kreatorflow-ai/openapi/kreatorflow-ai-lip-sync-api-openapi.yml
- filename: kreatorflow-ai-mcp-api-openapi.yml
  format: yaml
  label: kreatorflow-ai MCP API
  slug: kreatorflow-ai-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kreatorflow-ai/openapi/kreatorflow-ai-mcp-api-openapi.yml
- filename: kreatorflow-ai-models-api-openapi.yml
  format: yaml
  label: kreatorflow-ai Models API
  slug: kreatorflow-ai-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kreatorflow-ai/openapi/kreatorflow-ai-models-api-openapi.yml
- filename: kreatorflow-ai-uploads-api-openapi.yml
  format: yaml
  label: kreatorflow-ai Uploads API
  slug: kreatorflow-ai-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kreatorflow-ai/openapi/kreatorflow-ai-uploads-api-openapi.yml
- filename: kreatorflow-ai-video-api-openapi.yml
  format: yaml
  label: kreatorflow-ai Video API
  slug: kreatorflow-ai-video-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kreatorflow-ai/openapi/kreatorflow-ai-video-api-openapi.yml
consequence_counts:
  read: 16
  write: 28
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Kreatorflow Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 44
overview: 'kreatorflow-ai exposes 44 API operations that an AI agent could call, of which 28 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read and 28 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: kreatorflow-ai
provider_slug: kreatorflow-ai
slug: kreatorflow-ai-agentic-access
source_filename: kreatorflow-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/developers.kreatorflow.ai-openapi.json, openapi/kreatorflow-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 44\n  by_action_class:\n    connected: 16\n    acting: 28\n  by_consequence:\n    read: 16\n    write: 28\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/models\n  method: get\n  operationId: getModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/uploads\n  method: post\n  operationId: postUploads\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/uploads\n  method: put\n  operationId: putUploads\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/uploads/complete\n  method: post\n  operationId: postUploadsComplete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/uploads/{upload_id}\n  method: delete\n  operationId: deleteUploadsByUploadId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/storage\n  method: get\n  operationId: getStorage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/images\n  method: post\n  operationId: postImages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/characters\n  method: post\n  operationId: postCharacters\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/characters\n  method: get\n  operationId: getCharacters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/characters/{character_id}\n  method: get\n  operationId: getCharactersByCharacterId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/characters/{character_id}\n  method: delete\n  operationId: deleteCharactersByCharacterId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos\n  method: post\n  operationId: postVideos\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/video-edits\n  method: post\n  operationId: postVideoEdits\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos/edit\n  method: post\n  operationId: postVideosEdit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos/extend\n  method: post\n \
  \ operationId: postVideosExtend\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/audio\n  method: post\n  operationId: postAudio\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/lip-sync\n  method: post\n  operationId: postLipSync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/voices\n\
  \  method: get\n  operationId: getVoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/{job_id}\n  method: get\n  operationId: getJobsByJobId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/{job_id}/output\n  method: get\n  operationId: getJobsByJobIdOutput\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/{job_id}/output\n  method: head\n  operationId: headJobsByJobIdOutputHead\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/mcp\n  method: post\n  operationId: postMcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/models\n  method: get\n  operationId: getModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/uploads\n  method: post\n  operationId: postUploads\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/uploads\n  method: put\n  operationId: putUploads\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/uploads/complete\n  method: post\n  operationId: postUploadsComplete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/uploads/{upload_id}\n  method: delete\n  operationId: deleteUploadsByUploadId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/storage\n  method: get\n  operationId: getStorage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/images\n  method: post\n  operationId: postImages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/characters\n  method: post\n  operationId: postCharacters\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/characters\n  method: get\n  operationId: getCharacters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/characters/{character_id}\n  method: get\n  operationId: getCharactersByCharacterId\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/characters/{character_id}\n  method: delete\n  operationId: deleteCharactersByCharacterId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos\n  method: post\n  operationId: postVideos\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/video-edits\n  method: post\n  operationId: postVideoEdits\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos/edit\n  method: post\n  operationId: postVideosEdit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos/extend\n  method: post\n  operationId: postVideosExtend\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/audio\n  method: post\n  operationId: postAudio\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/lip-sync\n  method: post\n  operationId: postLipSync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/voices\n  method: get\n  operationId: getVoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/{job_id}\n  method: get\n  operationId: getJobsByJobId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/jobs/{job_id}/output\n  method: get\n  operationId: getJobsByJobIdOutput\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/{job_id}/output\n  method: head\n  operationId: headJobsByJobIdOutputHead\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/mcp\n  method: post\n  operationId: postMcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/kreatorflow-ai/agentic-access/kreatorflow-ai-agentic-access.yml
summary_line: 44 operations · 28 acting
tags:
- Artificial Intelligence
- Video
- Image
- Voice
- Platform
---
