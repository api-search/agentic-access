---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 6
api_specs:
- filename: transcriptapi-io-auth-api-openapi.yml
  format: yaml
  label: transcriptapi-io Auth API
  slug: transcriptapi-io-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcriptapi-io/openapi/transcriptapi-io-auth-api-openapi.yml
- filename: transcriptapi-io-channels-api-openapi.yml
  format: yaml
  label: transcriptapi-io Channels API
  slug: transcriptapi-io-channels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcriptapi-io/openapi/transcriptapi-io-channels-api-openapi.yml
- filename: transcriptapi-io-health-api-openapi.yml
  format: yaml
  label: transcriptapi-io Health API
  slug: transcriptapi-io-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcriptapi-io/openapi/transcriptapi-io-health-api-openapi.yml
- filename: transcriptapi-io-playlists-api-openapi.yml
  format: yaml
  label: transcriptapi-io Playlists API
  slug: transcriptapi-io-playlists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcriptapi-io/openapi/transcriptapi-io-playlists-api-openapi.yml
- filename: transcriptapi-io-public-tools-api-openapi.yml
  format: yaml
  label: transcriptapi-io Public tools API
  slug: transcriptapi-io-public-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcriptapi-io/openapi/transcriptapi-io-public-tools-api-openapi.yml
- filename: transcriptapi-io-search-api-openapi.yml
  format: yaml
  label: transcriptapi-io Search API
  slug: transcriptapi-io-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcriptapi-io/openapi/transcriptapi-io-search-api-openapi.yml
- filename: transcriptapi-io-transcripts-api-openapi.yml
  format: yaml
  label: transcriptapi-io Transcripts API
  slug: transcriptapi-io-transcripts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcriptapi-io/openapi/transcriptapi-io-transcripts-api-openapi.yml
- filename: transcriptapi-io-webhooks-api-openapi.yml
  format: yaml
  label: transcriptapi-io Webhooks API
  slug: transcriptapi-io-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcriptapi-io/openapi/transcriptapi-io-webhooks-api-openapi.yml
consequence_counts:
  read: 6
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Transcriptapi Io Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'transcriptapi-io exposes 14 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: transcriptapi-io
provider_slug: transcriptapi-io
slug: transcriptapi-io-agentic-access
source_filename: transcriptapi-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/transcriptapi-io-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    acting: 8\n    connected: 6\n  by_consequence:\n    write: 8\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /auth/login\n  method: post\n  operationId: login_auth_login_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transcript\n  method: get\n  operationId: get_transcript_transcript_get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search\n  method: get\n  operationId: search_search_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /channel/videos\n  method: get\n  operationId: channel_videos_channel_videos_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /channel/search\n  method: get\n  operationId: channel_search_channel_search_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /playlist\n  method: get\n  operationId: get_playlist_playlist_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n \
  \   audit: none\n- path: /channel/subscribe\n  method: post\n  operationId: subscribe_channel_subscribe_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /channel/subscribe\n  method: delete\n  operationId: unsubscribe_channel_subscribe_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tool/transcript\n  method: post\n  operationId: tool_transcript_tool_transcript_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tool/channel\n  method: post\n  operationId: tool_channel_tool_channel_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tool/playlist\n  method: post\n  operationId: tool_playlist_tool_playlist_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tool/translate\n  method: post\n  operationId: tool_translate_tool_translate_post\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tool/summarize\n  method: post\n  operationId: tool_summarize_tool_summarize_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /health\n  method: get\n  operationId: health_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/transcriptapi-io/agentic-access/transcriptapi-io-agentic-access.yml
summary_line: 14 operations · 8 acting
tags:
- Company
- YouTube
- Transcripts
- Data
---
