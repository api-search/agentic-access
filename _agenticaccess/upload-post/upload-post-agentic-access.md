---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 8
api_specs:
- filename: upload-post-openapi.yml
  format: yaml
  label: Upload-Post Upload Video API
  slug: upload-post-upload-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upload-post/refs/heads/main/openapi/upload-post-openapi.yml
- filename: upload-post-openapi.yml
  format: yaml
  label: Upload-Post Upload Photos API
  slug: upload-post-upload-photos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upload-post/refs/heads/main/openapi/upload-post-openapi.yml
- filename: upload-post-openapi.yml
  format: yaml
  label: Upload-Post Upload Text API
  slug: upload-post-upload-text-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upload-post/refs/heads/main/openapi/upload-post-openapi.yml
- filename: upload-post-openapi.yml
  format: yaml
  label: Upload-Post Profiles and Users API
  slug: upload-post-profiles-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upload-post/refs/heads/main/openapi/upload-post-openapi.yml
- filename: upload-post-openapi.yml
  format: yaml
  label: Upload-Post Analytics API
  slug: upload-post-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upload-post/refs/heads/main/openapi/upload-post-openapi.yml
consequence_counts:
  read: 8
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Upload Post Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'Upload-Post exposes 15 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Upload-Post
provider_slug: upload-post
slug: upload-post-agentic-access
source_filename: upload-post-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/upload-post-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    acting: 7\n    connected: 8\n  by_consequence:\n    write: 7\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /upload\n  method: post\n  operationId: uploadVideo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /upload_photos\n  method: post\n  operationId: uploadPhotos\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /upload_text\n  method: post\n  operationId: uploadText\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /uploadposts/status\n  method: get\n  operationId: getUploadStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /uploadposts/history\n  method: get\n  operationId: getUploadHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /uploadposts/users\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /uploadposts/users\n  method: post\n  operationId: createUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /uploadposts/users\n  method: delete\n  operationId: deleteUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /uploadposts/users/{username}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /uploadposts/users/generate-jwt\n  method: post\n  operationId: generateJwt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /uploadposts/users/validate-jwt\n  method: post\n  operationId: validateJwt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /uploadposts/me\n  method: get\n  operationId: getMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/{profile_username}\n  method: get\n  operationId: getAnalytics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /uploadposts/total-impressions/{profile_username}\n  method: get\n  operationId: getTotalImpressions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /uploadposts/post-analytics/{request_id}\n  method: get\n  operationId: getPostAnalytics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upload-post/refs/heads/main/agentic-access/upload-post-agentic-access.yml
summary_line: 15 operations · 7 acting
tags:
- Social Media
- Publishing
- Video
- Content
- Cross Posting
---
