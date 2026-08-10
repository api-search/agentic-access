---
acting_count: 0
action_class_counts:
  connected: 5
api_specs:
- filename: artlist-album-api-openapi.yml
  format: yaml
  label: Artlist Album API
  slug: artlist-album-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artlist/refs/heads/main/openapi/artlist-album-api-openapi.yml
- filename: artlist-artist-api-openapi.yml
  format: yaml
  label: Artlist Artist API
  slug: artlist-artist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artlist/refs/heads/main/openapi/artlist-artist-api-openapi.yml
- filename: artlist-downloadable-api-openapi.yml
  format: yaml
  label: Artlist Downloadable API
  slug: artlist-downloadable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artlist/refs/heads/main/openapi/artlist-downloadable-api-openapi.yml
- filename: artlist-song-api-openapi.yml
  format: yaml
  label: Artlist Song API
  slug: artlist-song-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artlist/refs/heads/main/openapi/artlist-song-api-openapi.yml
consequence_counts:
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Artlist Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Artlist exposes 5 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Artlist
provider_slug: artlist
slug: artlist-agentic-access
source_filename: artlist-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: generated\nsource: openapi/artlist-download-openapi-original.yml, openapi/artlist-search-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 5\n  by_consequence:\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /https://business.artlist.io/download/v1/downloadable/{assetType}/{id}/{format}\n  method: get\n  operationId: downloadable-controller-get-downloadable-url\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /https://business.artlist.io/search/v1/song/{id}\n  method: get\n  operationId: song-controller-get-song\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /https://business.artlist.io/search/v1/song\n  method: get\n  operationId: song-controller-get-songs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /https://business.artlist.io/search/v1/artist/{id}\n  method: get\n  operationId: artist-controller-get-artist\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /https://business.artlist.io/search/v1/album/{id}\n  method: get\n  operationId: album-controller-get-album\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/artlist/refs/heads/main/agentic-access/artlist-agentic-access.yml
summary_line: 5 operations
tags:
- Company
- Music
- Audio
- Media
- Stock Media
- Content Licensing
- Creative Tools
- Search
- Generative AI
- Video
---
