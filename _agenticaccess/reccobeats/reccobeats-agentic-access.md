---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 13
api_specs:
- filename: reccobeats-openapi.yml
  format: yaml
  label: ReccoBeats Track API
  slug: reccobeats-track-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reccobeats/refs/heads/main/openapi/reccobeats-openapi.yml
- filename: reccobeats-openapi.yml
  format: yaml
  label: ReccoBeats Audio Features API
  slug: reccobeats-audio-features-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reccobeats/refs/heads/main/openapi/reccobeats-openapi.yml
- filename: reccobeats-openapi.yml
  format: yaml
  label: ReccoBeats Audio Analysis API
  slug: reccobeats-audio-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reccobeats/refs/heads/main/openapi/reccobeats-openapi.yml
- filename: reccobeats-openapi.yml
  format: yaml
  label: ReccoBeats Recommendation API
  slug: reccobeats-recommendation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reccobeats/refs/heads/main/openapi/reccobeats-openapi.yml
- filename: reccobeats-openapi.yml
  format: yaml
  label: ReccoBeats Artist API
  slug: reccobeats-artist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reccobeats/refs/heads/main/openapi/reccobeats-openapi.yml
- filename: reccobeats-openapi.yml
  format: yaml
  label: ReccoBeats Album API
  slug: reccobeats-album-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reccobeats/refs/heads/main/openapi/reccobeats-openapi.yml
consequence_counts:
  read: 13
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Reccobeats Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'ReccoBeats exposes 14 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ReccoBeats
provider_slug: reccobeats
slug: reccobeats-agentic-access
source_filename: reccobeats-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/reccobeats-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 13\n    acting: 1\n  by_consequence:\n    read: 13\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /track\n  method: get\n  operationId: getTracks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /track/{id}\n  method: get\n  operationId: getTrackById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /track/{id}/audio-features\n  method: get\n  operationId:\
  \ getTrackAudioFeatures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /track/recommendation\n  method: get\n  operationId: getRecommendation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analysis/audio-features\n  method: post\n  operationId: extractAudioFeatures\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /artist\n  method: get\n  operationId: getArtists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artist/search\n  method:\
  \ get\n  operationId: searchArtists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artist/{id}\n  method: get\n  operationId: getArtistById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artist/{id}/album\n  method: get\n  operationId: getArtistAlbums\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artist/{id}/track\n  method: get\n  operationId: getArtistTracks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /album\n  method: get\n  operationId: getAlbums\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /album/search\n  method: get\n  operationId: searchAlbums\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /album/{id}\n  method: get\n  operationId: getAlbumById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /album/{id}/track\n  method: get\n  operationId: getAlbumTracks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reccobeats/refs/heads/main/agentic-access/reccobeats-agentic-access.yml
summary_line: 14 operations · 1 acting
tags:
- Music
- Recommendations
- Audio Features
- Audio Analysis
- Music Database
- Spotify Alternative
---
