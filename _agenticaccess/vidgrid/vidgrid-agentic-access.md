---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 5
api_specs:
- filename: vidgrid-caption-api-openapi.yml
  format: yaml
  label: VidGrid Caption API
  slug: vidgrid-caption-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vidgrid/refs/heads/main/openapi/vidgrid-caption-api-openapi.yml
- filename: vidgrid-folder-api-openapi.yml
  format: yaml
  label: VidGrid Folder API
  slug: vidgrid-folder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vidgrid/refs/heads/main/openapi/vidgrid-folder-api-openapi.yml
- filename: vidgrid-search-api-openapi.yml
  format: yaml
  label: VidGrid Search API
  slug: vidgrid-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vidgrid/refs/heads/main/openapi/vidgrid-search-api-openapi.yml
- filename: vidgrid-token-api-openapi.yml
  format: yaml
  label: VidGrid Token API
  slug: vidgrid-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vidgrid/refs/heads/main/openapi/vidgrid-token-api-openapi.yml
- filename: vidgrid-user-api-openapi.yml
  format: yaml
  label: VidGrid User API
  slug: vidgrid-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vidgrid/refs/heads/main/openapi/vidgrid-user-api-openapi.yml
- filename: vidgrid-video-api-openapi.yml
  format: yaml
  label: VidGrid Video API
  slug: vidgrid-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vidgrid/refs/heads/main/openapi/vidgrid-video-api-openapi.yml
- filename: vidgrid-webhooks-api-openapi.yml
  format: yaml
  label: VidGrid Webhooks API
  slug: vidgrid-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vidgrid/refs/heads/main/openapi/vidgrid-webhooks-api-openapi.yml
consequence_counts:
  read: 5
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Vidgrid Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'VidGrid exposes 15 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 10 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: VidGrid
provider_slug: vidgrid
slug: vidgrid-agentic-access
source_filename: vidgrid-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/vidgrid-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 5\n    acting: 10\n  by_consequence:\n    read: 5\n    write: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /vidgrid/v2/videos/{identifier}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vidgrid/v2/videos/{identifier}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vidgrid/v2/videos/{identifier}\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vidgrid/v2/captions/{identifier}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vidgrid/v2/captions/{identifier}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vidgrid/v2/folders/{identifier}\n  method:\
  \ get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vidgrid/v2/folders/{identifier}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vidgrid/v2/folders/{identifier}\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vidgrid/v2/users/{identifier}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /vidgrid/v2/users/{identifier}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vidgrid/v2/search/{resource}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vidgrid/v2/captions\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vidgrid/v2/folders\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vidgrid/v2/tokens\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vidgrid/v2/webhooks\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vidgrid/refs/heads/main/agentic-access/vidgrid-agentic-access.yml
summary_line: 15 operations · 10 acting
tags:
- Video
- Screen Recording
- Captions
- Video Hosting
- Webhook
- Training
- HR
---
