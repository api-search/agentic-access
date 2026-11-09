---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 25
api_specs:
- filename: chartmetric-charts-api-openapi.yml
  format: yaml
  label: Chartmetric Charts API
  slug: chartmetric-charts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-charts-api-openapi.yml
- filename: chartmetric-search-api-openapi.yml
  format: yaml
  label: Chartmetric Search API
  slug: chartmetric-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-search-api-openapi.yml
- filename: chartmetric-album-api-openapi.yml
  format: yaml
  label: Chartmetric Album API
  slug: chartmetric-album-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-album-api-openapi.yml
- filename: chartmetric-artist-api-openapi.yml
  format: yaml
  label: Chartmetric Artist API
  slug: chartmetric-artist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-artist-api-openapi.yml
- filename: chartmetric-brand-api-openapi.yml
  format: yaml
  label: Chartmetric Brand API
  slug: chartmetric-brand-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-brand-api-openapi.yml
- filename: chartmetric-city-api-openapi.yml
  format: yaml
  label: Chartmetric City API
  slug: chartmetric-city-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-city-api-openapi.yml
- filename: chartmetric-country-api-openapi.yml
  format: yaml
  label: Chartmetric Country API
  slug: chartmetric-country-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-country-api-openapi.yml
- filename: chartmetric-curator-api-openapi.yml
  format: yaml
  label: Chartmetric Curator API
  slug: chartmetric-curator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-curator-api-openapi.yml
- filename: chartmetric-event-api-openapi.yml
  format: yaml
  label: Chartmetric Event API
  slug: chartmetric-event-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-event-api-openapi.yml
- filename: chartmetric-festival-api-openapi.yml
  format: yaml
  label: Chartmetric Festival API
  slug: chartmetric-festival-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-festival-api-openapi.yml
- filename: chartmetric-genre-api-openapi.yml
  format: yaml
  label: Chartmetric Genre API
  slug: chartmetric-genre-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-genre-api-openapi.yml
- filename: chartmetric-playlist-api-openapi.yml
  format: yaml
  label: Chartmetric Playlist API
  slug: chartmetric-playlist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-playlist-api-openapi.yml
- filename: chartmetric-radio-api-openapi.yml
  format: yaml
  label: Chartmetric Radio API
  slug: chartmetric-radio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-radio-api-openapi.yml
- filename: chartmetric-sns-api-openapi.yml
  format: yaml
  label: Chartmetric SNS API
  slug: chartmetric-sns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-sns-api-openapi.yml
- filename: chartmetric-token-api-openapi.yml
  format: yaml
  label: Chartmetric Token API
  slug: chartmetric-token-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-token-api-openapi.yml
- filename: chartmetric-track-api-openapi.yml
  format: yaml
  label: Chartmetric Track API
  slug: chartmetric-track-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-track-api-openapi.yml
- filename: chartmetric-venue-api-openapi.yml
  format: yaml
  label: Chartmetric Venue API
  slug: chartmetric-venue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-venue-api-openapi.yml
consequence_counts:
  read: 25
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Chartmetric Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 26
overview: 'Chartmetric exposes 26 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 25 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Chartmetric
provider_slug: chartmetric
slug: chartmetric-agentic-access
source_filename: chartmetric-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/chartmetric-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 26\n  by_action_class:\n    acting: 1\n    connected: 25\n  by_consequence:\n    write: 1\n    read: 25\n  human_in_the_loop_required: 0\noperations:\n- path: /token\n  method: post\n  operationId: createToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /search\n  method: get\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artist/{id}\n  method: get\n  operationId: getArtist\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artist/{id}/stat/{source}\n  method: get\n  operationId: getArtistStat\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artist/{id}/urls\n  method: get\n  operationId: getArtistUrls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artist/{id}/relatedartists\n  method: get\n  operationId: getRelatedArtists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artist/{id}/where-people-listen\n\
  \  method: get\n  operationId: getArtistWherePeopleListen\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artist/{id}/tracks\n  method: get\n  operationId: getArtistTracks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artist/{id}/albums\n  method: get\n  operationId: getArtistAlbums\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artist/{id}/{source}/{status}/playlists\n  method: get\n  operationId: getArtistPlaylists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /track/{id}\n  method: get\n  operationId: getTrack\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /track/{id}/{platform}/stats\n  method: get\n  operationId: getTrackStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /track/{id}/{chartType}/charts\n  method: get\n  operationId: getTrackCharts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /track/{id}/{platform}/{status}/playlists\n  method: get\n  operationId: getTrackPlaylists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /album/{id}\n  method: get\n  operationId: getAlbum\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /album/{id}/tracks\n  method: get\n  operationId: getAlbumTracks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /album/{id}/{source}/followers\n  method: get\n  operationId: getAlbumFollowers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /album/{id}/{source}/{status}/playlists\n  method: get\n  operationId: getAlbumPlaylists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /playlist/{platform}/{id}\n  method: get\n  operationId: getPlaylist\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /playlist/{platform}/{id}/{span}/tracks\n  method: get\n  operationId:\
  \ getPlaylistTracks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /playlist/{platform}/{id}/snapshot\n  method: get\n  operationId: getPlaylistSnapshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /playlist/{platform}/lists\n  method: get\n  operationId: getPlaylistLists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /charts/{platform}\n  method: get\n  operationId: getCharts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /charts/artist/{id}/{chartType}/cm-score\n  method: get\n  operationId: getArtistCmScore\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /charts/track/{id}/{chartType}/cm-score\n  method: get\n  operationId: getTrackCmScore\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /charts/album/{id}/{chartType}/cm-score\n  method: get\n  operationId: getAlbumCmScore\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/chartmetric/agentic-access/chartmetric-agentic-access.yml
summary_line: 26 operations · 1 acting
tags:
- Music
- Analytics
- Artist Intelligence
- Streaming
- Charts
---
