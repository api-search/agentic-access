---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 3
api_specs:
- filename: anisongs-jp-check-purity-api-openapi.yml
  format: yaml
  label: Anisongs Check Purity API
  slug: anisongs-jp-check-purity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anisongs-jp/openapi/anisongs-jp-check-purity-api-openapi.yml
- filename: anisongs-jp-create-playlist-api-openapi.yml
  format: yaml
  label: Anisongs Create Playlist API
  slug: anisongs-jp-create-playlist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anisongs-jp/openapi/anisongs-jp-create-playlist-api-openapi.yml
- filename: anisongs-jp-get-artist-api-openapi.yml
  format: yaml
  label: Anisongs Get Artist API
  slug: anisongs-jp-get-artist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anisongs-jp/openapi/anisongs-jp-get-artist-api-openapi.yml
- filename: anisongs-jp-get-program-api-openapi.yml
  format: yaml
  label: Anisongs Get Program API
  slug: anisongs-jp-get-program-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anisongs-jp/openapi/anisongs-jp-get-program-api-openapi.yml
- filename: anisongs-jp-search-tracks-api-openapi.yml
  format: yaml
  label: Anisongs Search Tracks API
  slug: anisongs-jp-search-tracks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anisongs-jp/openapi/anisongs-jp-search-tracks-api-openapi.yml
consequence_counts:
  read: 3
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Anisongs Jp Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Anisongs exposes 5 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Anisongs
provider_slug: anisongs-jp
slug: anisongs-jp-agentic-access
source_filename: anisongs-jp-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/anisongs-jp-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 3\n    acting: 2\n  by_consequence:\n    read: 3\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /search_tracks\n  method: post\n  operationId: searchTracks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get_program\n  method: post\n  operationId: getProgram\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get_artist\n  method: post\n  operationId:\
  \ getArtist\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /check_purity\n  method: post\n  operationId: checkPurity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /create_playlist\n  method: post\n  operationId: createPlaylist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/anisongs-jp/agentic-access/anisongs-jp-agentic-access.yml
summary_line: 5 operations · 2 acting
tags:
- Anime
- Music
- Database
- Japanese
- Entertainment
---
