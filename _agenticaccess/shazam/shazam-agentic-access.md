---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 11
api_specs:
- filename: shazam-rest-api-openapi.yml
  format: yaml
  label: Shazam REST API (RapidAPI)
  slug: shazam-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shazam/refs/heads/main/openapi/shazam-rest-api-openapi.yml
consequence_counts:
  read: 11
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Shazam Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Shazam exposes 12 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Shazam
provider_slug: shazam
slug: shazam-agentic-access
source_filename: shazam-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/shazam-rest-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    acting: 1\n    connected: 11\n  by_consequence:\n    write: 1\n    read: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /discovery/v5/{language}/{endpoint_country}/{device}/-/tag/{uuid_1}/{uuid_2}\n  method: post\n  operationId: recognizeTrack\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /discovery/v5/{language}/{endpoint_country}/web/-/track/{track_id}\n\
  \  method: get\n  operationId: getTrack\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/amapi/v1/catalog/{endpoint_country}/playlists/{playlist_id}/tracks\n  method: get\n  operationId: getPlaylistTracks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/charts/locations\n  method: get\n  operationId: getChartLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/search/v4/{language}/{endpoint_country}/web/search\n  method: get\n  operationId: searchArtists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/search/v3/{language}/{endpoint_country}/web/search\n\
  \  method: get\n  operationId: searchTracks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/amapi/v1/catalog/{endpoint_country}/artists/{artist_id}\n  method: get\n  operationId: getArtist\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/amapi/v1/catalog/{endpoint_country}/artists/{artist_id}/albums\n  method: get\n  operationId: getArtistAlbums\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/amapi/v1/catalog/{endpoint_country}/albums/{album_id}\n  method: get\n  operationId: getAlbum\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shazam/v3/{language}/{endpoint_country}/web/-/tracks/track-similarities-id-{track_id}\n\
  \  method: get\n  operationId: getRelatedTracks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/count/v2/web/track/{track_id}\n  method: get\n  operationId: getListeningCounter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/count/v2/web/track\n  method: get\n  operationId: getListeningCounterMany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shazam/refs/heads/main/agentic-access/shazam-agentic-access.yml
summary_line: 12 operations · 1 acting
tags:
- Music
- Audio Recognition
- Song Identification
- Charts
- Artists
- Tracks
- Fingerprinting
---
