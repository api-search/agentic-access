---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 16
api_specs:
- filename: transcript-yt-com-languages-api-openapi.yml
  format: yaml
  label: transcript-yt-com Languages API
  slug: transcript-yt-com-languages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcript-yt-com/openapi/transcript-yt-com-languages-api-openapi.yml
- filename: transcript-yt-com-playlist-api-openapi.yml
  format: yaml
  label: transcript-yt-com Playlist API
  slug: transcript-yt-com-playlist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcript-yt-com/openapi/transcript-yt-com-playlist-api-openapi.yml
- filename: transcript-yt-com-search-api-openapi.yml
  format: yaml
  label: transcript-yt-com Search API
  slug: transcript-yt-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcript-yt-com/openapi/transcript-yt-com-search-api-openapi.yml
- filename: transcript-yt-com-summary-api-openapi.yml
  format: yaml
  label: transcript-yt-com Summary API
  slug: transcript-yt-com-summary-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcript-yt-com/openapi/transcript-yt-com-summary-api-openapi.yml
- filename: transcript-yt-com-transcript-api-openapi.yml
  format: yaml
  label: transcript-yt-com Transcript API
  slug: transcript-yt-com-transcript-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcript-yt-com/openapi/transcript-yt-com-transcript-api-openapi.yml
- filename: transcript-yt-com-transcripts-api-openapi.yml
  format: yaml
  label: transcript-yt-com Transcripts API
  slug: transcript-yt-com-transcripts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcript-yt-com/openapi/transcript-yt-com-transcripts-api-openapi.yml
- filename: transcript-yt-com-usage-api-openapi.yml
  format: yaml
  label: transcript-yt-com Usage API
  slug: transcript-yt-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcript-yt-com/openapi/transcript-yt-com-usage-api-openapi.yml
consequence_counts:
  read: 16
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Transcript Yt Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 18
overview: 'transcript-yt-com exposes 18 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: transcript-yt-com
provider_slug: transcript-yt-com
slug: transcript-yt-com-agentic-access
source_filename: transcript-yt-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/openapi.json, openapi/transcript-yt-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    connected: 16\n    acting: 2\n  by_consequence:\n    read: 16\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/transcript\n  method: get\n  operationId: getTranscript\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transcript\n  method: post\n  operationId: postTranscript\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/transcripts\n  method: post\n  operationId: postTranscripts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/search\n  method: get\n  operationId: searchYoutube\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/summary\n  method: get\n  operationId: getSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/summary\n  method: post\n  operationId: postSummary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/playlist\n  method:\
  \ get\n  operationId: getPlaylist\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/languages\n  method: get\n  operationId: listLanguages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/usage\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transcript\n  method: get\n  operationId: getTranscript\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transcript\n  method: post\n  operationId: postTranscript\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n- path: /v1/transcripts\n  method: post\n  operationId: postTranscripts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/search\n  method: get\n  operationId: searchYoutube\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/summary\n  method: get\n  operationId: getSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/summary\n  method: post\n  operationId: postSummary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v1/playlist\n  method: get\n  operationId: getPlaylist\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/languages\n  method: get\n  operationId: listLanguages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/usage\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/transcript-yt-com/agentic-access/transcript-yt-com-agentic-access.yml
summary_line: 18 operations · 2 acting
tags:
- Company
- YouTube
- Transcript
- MCP
---
