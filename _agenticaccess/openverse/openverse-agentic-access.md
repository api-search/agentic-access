---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 13
api_specs:
- filename: openverse-audio-api-openapi.yml
  format: yaml
  label: Openverse audio API
  slug: openverse-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openverse/refs/heads/main/openapi/openverse-audio-api-openapi.yml
- filename: openverse-auth-api-openapi.yml
  format: yaml
  label: Openverse auth API
  slug: openverse-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openverse/refs/heads/main/openapi/openverse-auth-api-openapi.yml
- filename: openverse-images-api-openapi.yml
  format: yaml
  label: Openverse images API
  slug: openverse-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openverse/refs/heads/main/openapi/openverse-images-api-openapi.yml
consequence_counts:
  read: 13
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Openverse Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'Openverse exposes 17 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Openverse
provider_slug: openverse
slug: openverse-agentic-access
source_filename: openverse-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    connected: 13\n    acting: 4\n  by_consequence:\n    read: 13\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/audio/\n  method: get\n  operationId: audio_search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/audio/{identifier}/\n  method: get\n  operationId: audio_detail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/audio/{identifier}/related/\n  method:\
  \ get\n  operationId: audio_related\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/audio/{identifier}/report/\n  method: post\n  operationId: audio_report\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/audio/{identifier}/thumb/\n  method: get\n  operationId: audio_thumb\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/audio/{identifier}/waveform/\n  method: get\n  operationId: audio_waveform\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/audio/stats/\n  method: get\n  operationId: audio_stats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/auth_tokens/register/\n  method: post\n  operationId: register\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth_tokens/token/\n  method: post\n  operationId: token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/images/\n  method: get\n  operationId: images_search\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/images/{identifier}/\n  method: get\n  operationId: images_detail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/images/{identifier}/related/\n  method: get\n  operationId: images_related\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/images/{identifier}/report/\n  method: post\n  operationId: images_report\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/images/{identifier}/thumb/\n  method: get\n\
  \  operationId: images_thumb\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/images/oembed/\n  method: get\n  operationId: images_oembed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/images/stats/\n  method: get\n  operationId: images_stats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/rate_limit/\n  method: get\n  operationId: key_info\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openverse/refs/heads/main/agentic-access/openverse-agentic-access.yml
summary_line: 17 operations · 4 acting
tags:
- Image
- Audio
- Creative Commons
- Open Media
- Search
- Open Data
- Cultural Heritage
- Museums
---
