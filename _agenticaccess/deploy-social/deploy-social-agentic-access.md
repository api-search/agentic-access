---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 9
api_specs:
- filename: deploy-social-account-api-openapi.yml
  format: yaml
  label: deploy.social Account API
  slug: deploy-social-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deploy-social/openapi/deploy-social-account-api-openapi.yml
- filename: deploy-social-destinations-api-openapi.yml
  format: yaml
  label: deploy.social Destinations API
  slug: deploy-social-destinations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deploy-social/openapi/deploy-social-destinations-api-openapi.yml
- filename: deploy-social-media-api-openapi.yml
  format: yaml
  label: deploy.social Media API
  slug: deploy-social-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deploy-social/openapi/deploy-social-media-api-openapi.yml
- filename: deploy-social-posts-api-openapi.yml
  format: yaml
  label: deploy.social Posts API
  slug: deploy-social-posts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deploy-social/openapi/deploy-social-posts-api-openapi.yml
consequence_counts:
  read: 9
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Deploy Social Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 18
overview: 'deploy.social exposes 18 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 9 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: deploy.social
provider_slug: deploy-social
slug: deploy-social-agentic-access
source_filename: deploy-social-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/deploy-social-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    connected: 9\n    acting: 9\n  by_consequence:\n    read: 9\n    write: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /me\n  method: get\n  operationId: getMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platforms\n  method: get\n  operationId: listPlatforms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /destinations\n  method: get\n  operationId: listDestinations\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /destinations/{id}\n  method: get\n  operationId: getDestination\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /destinations/{id}/options\n  method: get\n  operationId: getDestinationOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /media/uploads\n  method: post\n  operationId: createUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /media/imports\n  method: post\n  operationId:\
  \ createImport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /media/{id}/complete\n  method: post\n  operationId: completeUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /media\n  method: get\n  operationId: listMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /media/{id}\n  method: get\n  operationId: getMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /posts\n  method: post\n  operationId: createPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /posts\n  method: get\n  operationId: listPosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /posts/{id}\n  method: get\n  operationId: getPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /posts/{id}\n  method: patch\n  operationId: updatePost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /posts/{id}\n  method: delete\n  operationId: deletePost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /posts/{id}/publish\n  method: post\n  operationId: publishPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /posts/{id}/cancel\n  method: post\n  operationId: cancelPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n   \
  \ audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /posts/{id}/retry\n  method: post\n  operationId: retryPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/deploy-social/agentic-access/deploy-social-agentic-access.yml
summary_line: 18 operations · 9 acting
tags:
- Company
- Social Media
- Video
- Short-Form Video
- Cross-Posting
- Scheduling
- Content Publishing
- MCP
---
