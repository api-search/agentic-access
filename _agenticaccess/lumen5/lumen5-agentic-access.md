---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 10
api_specs:
- filename: lumen5-video-creation-api-openapi.yml
  format: yaml
  label: Lumen5 Video Creation API
  slug: lumen5-video-creation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumen5/refs/heads/main/openapi/lumen5-video-creation-api-openapi.yml
consequence_counts:
  read: 10
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Lumen5 Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'Lumen5 exposes 15 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Lumen5
provider_slug: lumen5
slug: lumen5-agentic-access
source_filename: lumen5-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: generated\nsource: openapi/lumen5.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 10\n    acting: 5\n  by_consequence:\n    read: 10\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/video-creation/blueprints/\n  method: get\n  operationId: v1_video_creation_blueprints_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/video-creation/brand-kits/\n  method: get\n  operationId: v1_video_creation_brand_kits_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/v1/video-creation/projects/\n  method: get\n  operationId: v1_video_creation_projects_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/video-creation/recipes/\n  method: get\n  operationId: v1_video_creation_recipes_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/video-creation/requests/\n  method: get\n  operationId: v1_video_creation_requests_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/video-creation/requests/\n  method: post\n  operationId: v1_video_creation_requests_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/video-creation/requests/{request_id}/\n  method: get\n  operationId: v1_video_creation_requests_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/video-creation/resolve/\n  method: post\n  operationId: v1_video_creation_resolve_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/video-creation/templates/\n  method: get\n  operationId: v1_video_creation_templates_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/video-creation/voices/\n  method: get\n  operationId: v1_video_creation_voices_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/video-creation/webhook-endpoints/\n  method: get\n  operationId: v1_video_creation_webhook_endpoints_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/video-creation/webhook-endpoints/\n  method: post\n  operationId: v1_video_creation_webhook_endpoints_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/video-creation/webhook-endpoints/{endpoint_id}/\n\
  \  method: delete\n  operationId: v1_video_creation_webhook_endpoints_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/video-creation/webhook-endpoints/{endpoint_id}/rotate-secret/\n  method: post\n  operationId: v1_video_creation_webhook_endpoints_rotate_secret_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/video-creation/workspaces/\n  method: get\n  operationId: v1_video_creation_workspaces_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lumen5/refs/heads/main/agentic-access/lumen5-agentic-access.yml
summary_line: 15 operations · 5 acting
tags:
- Company
---
