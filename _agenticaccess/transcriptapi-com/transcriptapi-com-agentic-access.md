---
acting_count: 0
action_class_counts:
  connected: 13
api_specs:
- filename: transcriptapi-com-youtube-channel-api-openapi.yml
  format: yaml
  label: transcriptapi-com YouTube channel API
  slug: transcriptapi-com-youtube-channel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcriptapi-com/openapi/transcriptapi-com-youtube-channel-api-openapi.yml
- filename: transcriptapi-com-youtube-playlist-api-openapi.yml
  format: yaml
  label: transcriptapi-com YouTube playlist API
  slug: transcriptapi-com-youtube-playlist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcriptapi-com/openapi/transcriptapi-com-youtube-playlist-api-openapi.yml
- filename: transcriptapi-com-youtube-search-api-openapi.yml
  format: yaml
  label: transcriptapi-com YouTube search API
  slug: transcriptapi-com-youtube-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcriptapi-com/openapi/transcriptapi-com-youtube-search-api-openapi.yml
- filename: transcriptapi-com-youtube-transcript-api-openapi.yml
  format: yaml
  label: transcriptapi-com YouTube transcript API
  slug: transcriptapi-com-youtube-transcript-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcriptapi-com/openapi/transcriptapi-com-youtube-transcript-api-openapi.yml
- filename: transcriptapi-com-youtube-video-api-openapi.yml
  format: yaml
  label: transcriptapi-com YouTube video API
  slug: transcriptapi-com-youtube-video-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcriptapi-com/openapi/transcriptapi-com-youtube-video-api-openapi.yml
consequence_counts:
  read: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Transcriptapi Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'transcriptapi-com exposes 13 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: transcriptapi-com
provider_slug: transcriptapi-com
slug: transcriptapi-com-agentic-access
source_filename: transcriptapi-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/transcriptapi-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 13\n  by_consequence:\n    read: 13\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v2/youtube/transcript\n  method: get\n  operationId: get_transcript_v2_api_v2_youtube_transcript_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/youtube/info\n  method: get\n  operationId: get_video_info_v2_api_v2_youtube_info_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /api/v2/youtube/search\n  method: get\n  operationId: search_api_v2_youtube_search_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/youtube/channel/resolve\n  method: get\n  operationId: resolve_channel_api_v2_youtube_channel_resolve_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/youtube/channel/info\n  method: get\n  operationId: channel_info_api_v2_youtube_channel_info_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/youtube/channel/playlists\n  method: get\n  operationId: channel_playlists_api_v2_youtube_channel_playlists_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/youtube/channel/posts\n  method: get\n  operationId: channel_posts_api_v2_youtube_channel_posts_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/youtube/channel/sections\n  method: get\n  operationId: channel_sections_api_v2_youtube_channel_sections_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/youtube/channel/search\n  method: get\n  operationId: channel_search_api_v2_youtube_channel_search_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/youtube/channel/videos\n  method: get\n  operationId: channel_videos_api_v2_youtube_channel_videos_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/youtube/channel/latest\n  method: get\n  operationId: channel_latest_api_v2_youtube_channel_latest_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/youtube/playlist/videos\n  method: get\n  operationId: playlist_videos_api_v2_youtube_playlist_videos_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/youtube/video/metadata\n  method: get\n  operationId: get_video_metadata_api_v2_youtube_video_metadata_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/transcriptapi-com/agentic-access/transcriptapi-com-agentic-access.yml
summary_line: 13 operations
tags:
- Transcripts
- YouTube API
- Search
- Content Extraction
---
