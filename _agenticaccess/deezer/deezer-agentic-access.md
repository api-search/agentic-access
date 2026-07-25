---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 38
api_specs:
- filename: deezer-album-api-openapi.yml
  format: yaml
  label: Deezer Album API
  slug: deezer-album-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deezer/refs/heads/main/openapi/deezer-album-api-openapi.yml
- filename: deezer-artist-api-openapi.yml
  format: yaml
  label: Deezer Artist API
  slug: deezer-artist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deezer/refs/heads/main/openapi/deezer-artist-api-openapi.yml
- filename: deezer-chart-api-openapi.yml
  format: yaml
  label: Deezer Chart API
  slug: deezer-chart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deezer/refs/heads/main/openapi/deezer-chart-api-openapi.yml
- filename: deezer-editorial-api-openapi.yml
  format: yaml
  label: Deezer Editorial API
  slug: deezer-editorial-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deezer/refs/heads/main/openapi/deezer-editorial-api-openapi.yml
- filename: deezer-genre-api-openapi.yml
  format: yaml
  label: Deezer Genre API
  slug: deezer-genre-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deezer/refs/heads/main/openapi/deezer-genre-api-openapi.yml
- filename: deezer-infos-api-openapi.yml
  format: yaml
  label: Deezer Infos API
  slug: deezer-infos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deezer/refs/heads/main/openapi/deezer-infos-api-openapi.yml
- filename: deezer-playlist-api-openapi.yml
  format: yaml
  label: Deezer Playlist API
  slug: deezer-playlist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deezer/refs/heads/main/openapi/deezer-playlist-api-openapi.yml
- filename: deezer-radio-api-openapi.yml
  format: yaml
  label: Deezer Radio API
  slug: deezer-radio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deezer/refs/heads/main/openapi/deezer-radio-api-openapi.yml
- filename: deezer-search-api-openapi.yml
  format: yaml
  label: Deezer Search API
  slug: deezer-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deezer/refs/heads/main/openapi/deezer-search-api-openapi.yml
- filename: deezer-track-api-openapi.yml
  format: yaml
  label: Deezer Track API
  slug: deezer-track-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deezer/refs/heads/main/openapi/deezer-track-api-openapi.yml
- filename: deezer-user-api-openapi.yml
  format: yaml
  label: Deezer User API
  slug: deezer-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deezer/refs/heads/main/openapi/deezer-user-api-openapi.yml
consequence_counts:
  read: 38
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Deezer Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 41
overview: 'Deezer exposes 41 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 38 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Deezer
provider_slug: deezer
slug: deezer-agentic-access
source_filename: deezer-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/deezer-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 41\n  by_action_class:\n    connected: 38\n    acting: 3\n  by_consequence:\n    read: 38\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /infos\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /track/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /album/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /album/{id}/tracks\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artist/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artist/{id}/top\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artist/{id}/albums\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artist/{id}/related\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /artist/{id}/radio\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artist/{id}/playlists\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /playlist/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /playlist/{id}/tracks\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /playlist/{id}/tracks\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - manage_library\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /playlist/{id}/tracks\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - manage_library\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chart\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chart/{genre_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chart/{genre_id}/tracks\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n  \
  \    max-ttl: 3600\n    audit: none\n- path: /chart/{genre_id}/albums\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chart/{genre_id}/artists\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/album\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/artist\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/playlist\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/track\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /genre\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /genre/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /genre/{id}/artists\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /radio\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /radio/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /radio/{id}/tracks\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /editorial\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /editorial/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /editorial/{id}/releases\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /user/me\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - basic_access\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/{id}/playlists\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/{id}/playlists\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - manage_library\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/{id}/tracks\n  method: get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/{id}/albums\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/{id}/artists\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/{id}/history\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - listening_history\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deezer/refs/heads/main/agentic-access/deezer-agentic-access.yml
summary_line: 41 operations · 3 acting
tags:
- Music
- Streaming
- Audio
- OAuth
- Catalog
- Playlists
---
