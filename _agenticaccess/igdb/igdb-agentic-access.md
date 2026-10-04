---
acting_count: 0
action_class_counts:
  connected: 17
api_specs:
- filename: igdb-companies-api-openapi.yml
  format: yaml
  label: IGDB Companies API
  slug: igdb-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/igdb/refs/heads/main/openapi/igdb-companies-api-openapi.yml
- filename: igdb-games-api-openapi.yml
  format: yaml
  label: IGDB Games API
  slug: igdb-games-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/igdb/refs/heads/main/openapi/igdb-games-api-openapi.yml
- filename: igdb-genres-api-openapi.yml
  format: yaml
  label: IGDB Genres API
  slug: igdb-genres-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/igdb/refs/heads/main/openapi/igdb-genres-api-openapi.yml
- filename: igdb-media-api-openapi.yml
  format: yaml
  label: IGDB Media API
  slug: igdb-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/igdb/refs/heads/main/openapi/igdb-media-api-openapi.yml
- filename: igdb-platforms-api-openapi.yml
  format: yaml
  label: IGDB Platforms API
  slug: igdb-platforms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/igdb/refs/heads/main/openapi/igdb-platforms-api-openapi.yml
- filename: igdb-reference-api-openapi.yml
  format: yaml
  label: IGDB Reference API
  slug: igdb-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/igdb/refs/heads/main/openapi/igdb-reference-api-openapi.yml
- filename: igdb-releases-api-openapi.yml
  format: yaml
  label: IGDB Releases API
  slug: igdb-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/igdb/refs/heads/main/openapi/igdb-releases-api-openapi.yml
- filename: igdb-search-api-openapi.yml
  format: yaml
  label: IGDB Search API
  slug: igdb-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/igdb/refs/heads/main/openapi/igdb-search-api-openapi.yml
consequence_counts:
  read: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Igdb Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'IGDB exposes 17 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: IGDB
provider_slug: igdb
slug: igdb-agentic-access
source_filename: igdb-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/igdb-companies-api-openapi.yml, openapi/igdb-games-api-openapi.yml, openapi/igdb-genres-api-openapi.yml,\n  openapi/igdb-media-api-openapi.yml, openapi/igdb-platforms-api-openapi.yml, openapi/igdb-reference-api-openapi.yml,\n  openapi/igdb-releases-api-openapi.yml, openapi/igdb-search-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    connected: 17\n  by_consequence:\n    read: 17\n  human_in_the_loop_required: 0\noperations:\n- path: /companies\n  method: post\n  operationId: postCompanies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /involved_companies\n  method: post\n  operationId: postInvolvedCompanies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /games\n  method: post\n  operationId: postGames\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /genres\n  method: post\n  operationId: postGenres\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /themes\n  method: post\n  operationId: postThemes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /covers\n  method: post\n  operationId: postCovers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /screenshots\n  method: post\n  operationId: postScreenshots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artworks\n  method: post\n  operationId: postArtworks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platforms\n  method: post\n  operationId: postPlatforms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /game_modes\n  method: post\n  operationId: postGameModes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections\n  method: post\n  operationId: postCollections\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /franchises\n  method: post\n  operationId: postFranchises\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /keywords\n  method: post\n  operationId: postKeywords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /age_ratings\n  method: post\n  operationId: postAgeRatings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /websites\n  method: post\n  operationId: postWebsites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /release_dates\n  method: post\n  operationId:\
  \ postReleaseDates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search\n  method: post\n  operationId: postSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/igdb/refs/heads/main/agentic-access/igdb-agentic-access.yml
summary_line: 17 operations
tags:
- Entertainment
- Game Database
- Gaming
- Video Games
---
