---
acting_count: 0
action_class_counts:
  connected: 32
api_specs:
- filename: soundcharts-album-api-openapi.yml
  format: yaml
  label: Soundcharts Album API
  slug: soundcharts-album-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundcharts/refs/heads/main/openapi/soundcharts-album-api-openapi.yml
- filename: soundcharts-artist-api-openapi.yml
  format: yaml
  label: Soundcharts Artist API
  slug: soundcharts-artist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundcharts/refs/heads/main/openapi/soundcharts-artist-api-openapi.yml
- filename: soundcharts-chart-api-openapi.yml
  format: yaml
  label: Soundcharts Chart API
  slug: soundcharts-chart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundcharts/refs/heads/main/openapi/soundcharts-chart-api-openapi.yml
- filename: soundcharts-metrics-api-openapi.yml
  format: yaml
  label: Soundcharts Metrics API
  slug: soundcharts-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundcharts/refs/heads/main/openapi/soundcharts-metrics-api-openapi.yml
- filename: soundcharts-playlist-api-openapi.yml
  format: yaml
  label: Soundcharts Playlist API
  slug: soundcharts-playlist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundcharts/refs/heads/main/openapi/soundcharts-playlist-api-openapi.yml
- filename: soundcharts-radio-api-openapi.yml
  format: yaml
  label: Soundcharts Radio API
  slug: soundcharts-radio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundcharts/refs/heads/main/openapi/soundcharts-radio-api-openapi.yml
- filename: soundcharts-referential-api-openapi.yml
  format: yaml
  label: Soundcharts Referential API
  slug: soundcharts-referential-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundcharts/refs/heads/main/openapi/soundcharts-referential-api-openapi.yml
- filename: soundcharts-search-api-openapi.yml
  format: yaml
  label: Soundcharts Search API
  slug: soundcharts-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundcharts/refs/heads/main/openapi/soundcharts-search-api-openapi.yml
- filename: soundcharts-song-api-openapi.yml
  format: yaml
  label: Soundcharts Song API
  slug: soundcharts-song-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundcharts/refs/heads/main/openapi/soundcharts-song-api-openapi.yml
consequence_counts:
  read: 32
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Soundcharts Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 32
overview: 'Soundcharts exposes 32 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 32 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Soundcharts
provider_slug: soundcharts
slug: soundcharts-agentic-access
source_filename: soundcharts-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/soundcharts-album-api-openapi.yml, openapi/soundcharts-artist-api-openapi.yml,\n  openapi/soundcharts-chart-api-openapi.yml, openapi/soundcharts-metrics-api-openapi.yml, openapi/soundcharts-playlist-api-openapi.yml,\n  openapi/soundcharts-radio-api-openapi.yml, openapi/soundcharts-referential-api-openapi.yml,\n  openapi/soundcharts-search-api-openapi.yml, openapi/soundcharts-song-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 32\n  by_action_class:\n    connected: 32\n  by_consequence:\n    read: 32\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v2/album/by-uuid/{uuid}\n  method: get\n  operationId: getAlbumMetadata\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/album/by-upc/{upc}\n  method: get\n  operationId: getAlbumByUpc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/album/by-platform/{platform}/{identifier}\n  method: get\n  operationId: getAlbumByPlatformId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2.26/album/{uuid}/tracks\n  method: get\n  operationId: getAlbumTracks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/artist/{uuid}\n  method: get\n  operationId: getArtistMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/artist/by-platform/{platform}/{identifier}\n  method: get\n  operationId: getArtistByPlatformId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/artist/{uuid}/songs\n  method: get\n  operationId: getArtistSongs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/artist/{uuid}/albums\n  method: get\n  operationId: getArtistAlbums\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/artist/{uuid}/related\n  method: get\n  operationId: getSimilarArtists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/v2/artist/{uuid}/current/stats\n  method: get\n  operationId: getArtistCurrentStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/artist/{uuid}/soundcharts/score\n  method: get\n  operationId: getArtistSoundchartsScore\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/chart/song/by-platform/{platform}\n  method: get\n  operationId: getSongChartsByPlatform\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/chart/song/{slug}/ranking/latest\n  method: get\n  operationId: getSongRankingLatest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/v2/chart/song/{slug}/ranking/{datetime}\n  method: get\n  operationId: getSongRankingForDate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/chart/album/{slug}/ranking/latest\n  method: get\n  operationId: getAlbumRankingLatest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/chart/tiktok/music/weekly/ranking/latest\n  method: get\n  operationId: getTiktokMusicRankingLatest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/song/{uuid}/audience/{platform}\n  method: get\n  operationId: getSongAudience\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/v2/artist/{uuid}/audience/{platform}\n  method: get\n  operationId: getArtistAudience\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/artist/{uuid}/streaming/{platform}/listening\n  method: get\n  operationId: getArtistStreamingAudience\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/artist/{uuid}/popularity/{platform}\n  method: get\n  operationId: getArtistPopularity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/playlist/{uuid}\n  method: get\n  operationId: getPlaylistMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/v2/playlist/by-platform/{platform}/{identifier}\n  method: get\n  operationId: getPlaylistByPlatformId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/playlist/{uuid}/tracks\n  method: get\n  operationId: getPlaylistTracks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/radio/{uuid}\n  method: get\n  operationId: getRadio\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/radio/by-slug/{slug}\n  method: get\n  operationId: getRadioBySlug\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/artist/{uuid}/broadcasts\n  method: get\n  operationId:\
  \ getArtistRadioSpins\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/referential/platforms\n  method: get\n  operationId: getPlatforms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/search\n  method: post\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/song/{uuid}\n  method: get\n  operationId: getSongMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/song/by-isrc/{isrc}\n  method: get\n  operationId: getSongByIsrc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/song/by-platform/{platform}/{identifier}\n  method: get\n  operationId: getSongByPlatformId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/song/{uuid}/audio-features\n  method: get\n  operationId: getSongAudioFeatures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soundcharts/refs/heads/main/agentic-access/soundcharts-agentic-access.yml
summary_line: 32 operations
tags:
- Music
- Analytics
- Market Intelligence
- Metadata
- Streaming
- Charts
---
