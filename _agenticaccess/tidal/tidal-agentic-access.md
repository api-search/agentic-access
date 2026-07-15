---
acting_count: 93
action_class_counts:
  acting: 93
  connected: 232
api_specs:
- filename: tidal-catalog-api-openapi.yml
  format: yaml
  label: TIDAL Catalog API
  slug: tidal-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidal/refs/heads/main/openapi/tidal-catalog-api-openapi.yml
- filename: tidal-search-api-openapi.yml
  format: yaml
  label: TIDAL Search API
  slug: tidal-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidal/refs/heads/main/openapi/tidal-search-api-openapi.yml
- filename: tidal-playlists-api-openapi.yml
  format: yaml
  label: TIDAL Playlists API
  slug: tidal-playlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidal/refs/heads/main/openapi/tidal-playlists-api-openapi.yml
- filename: tidal-users-api-openapi.yml
  format: yaml
  label: TIDAL Users API
  slug: tidal-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidal/refs/heads/main/openapi/tidal-users-api-openapi.yml
- filename: tidal-user-collections-api-openapi.yml
  format: yaml
  label: TIDAL User Collections API
  slug: tidal-user-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidal/refs/heads/main/openapi/tidal-user-collections-api-openapi.yml
- filename: tidal-recommendations-api-openapi.yml
  format: yaml
  label: TIDAL Recommendations API
  slug: tidal-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidal/refs/heads/main/openapi/tidal-recommendations-api-openapi.yml
- filename: tidal-playback-api-openapi.yml
  format: yaml
  label: TIDAL Playback API
  slug: tidal-playback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidal/refs/heads/main/openapi/tidal-playback-api-openapi.yml
- filename: tidal-social-api-openapi.yml
  format: yaml
  label: TIDAL Social API
  slug: tidal-social-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidal/refs/heads/main/openapi/tidal-social-api-openapi.yml
- filename: tidal-commerce-api-openapi.yml
  format: yaml
  label: TIDAL Commerce API
  slug: tidal-commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidal/refs/heads/main/openapi/tidal-commerce-api-openapi.yml
- filename: tidal-claims-api-openapi.yml
  format: yaml
  label: TIDAL Claims API
  slug: tidal-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidal/refs/heads/main/openapi/tidal-claims-api-openapi.yml
consequence_counts:
  physical: 43
  read: 232
  write: 50
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tidal Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /albums/{id}/relationships/coverArt
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /albums/{id}/relationships/items
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /artistClaims/{id}/relationships/acceptedArtists
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /artists/{id}/relationships/following
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /artists/{id}/relationships/following
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /artists/{id}/relationships/profileArt
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /installations/{id}/relationships/offlineInventory
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /installations/{id}/relationships/offlineInventory
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /playQueues/{id}/relationships/current
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /playQueues/{id}/relationships/future
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /playQueues/{id}/relationships/future
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /playQueues/{id}/relationships/future
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /playlists/{id}/relationships/collaboratorProfiles
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /playlists/{id}/relationships/collaboratorProfiles
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /playlists/{id}/relationships/coverArt
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /playlists/{id}/relationships/items
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /playlists/{id}/relationships/items
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /playlists/{id}/relationships/items
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /tracks/{id}/relationships/albums
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /userCollectionAlbums/{id}/relationships/items
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /userCollectionAlbums/{id}/relationships/items
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /userCollectionArtists/{id}/relationships/items
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /userCollectionArtists/{id}/relationships/items
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /userCollectionFolders/{id}/relationships/items
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /userCollectionFolders/{id}/relationships/items
operation_count: 325
overview: 'TIDAL exposes 325 API operations that an AI agent could call, of which 93 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 232 read, 50 write, and 43 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: TIDAL
provider_slug: tidal
slug: tidal-agentic-access
source_filename: tidal-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/tidal-catalog-api-openapi.yml, openapi/tidal-claims-api-openapi.yml, openapi/tidal-commerce-api-openapi.yml,\n  openapi/tidal-playback-api-openapi.yml, openapi/tidal-playlists-api-openapi.yml, openapi/tidal-recommendations-api-openapi.yml,\n  openapi/tidal-search-api-openapi.yml, openapi/tidal-social-api-openapi.yml, openapi/tidal-user-collections-api-openapi.yml,\n  openapi/tidal-users-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 325\n  by_action_class:\n    connected: 232\n    acting: 93\n  by_consequence:\n    read: 232\n    write: 50\n    physical: 43\n  human_in_the_loop_required: 0\noperations:\n- path: /albumStatistics\n  method: get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - r_usr\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /albumStatistics/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - r_usr\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /albumStatistics/{id}/relationships/owners\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - r_usr\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /albums\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - r_usr\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /albums\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - w_usr\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /albums/{id}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - w_usr\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /albums/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /albums/{id}\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - w_usr\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /albums/{id}/relationships/albumStatistics\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - r_usr\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /albums/{id}/relationships/artists\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /albums/{id}/relationships/coverArt\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /albums/{id}/relationships/coverArt\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - w_usr\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /albums/{id}/relationships/genres\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /albums/{id}/relationships/items\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /albums/{id}/relationships/items\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - w_usr\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /albums/{id}/relationships/owners\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /albums/{id}/relationships/priceConfig\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /albums/{id}/relationships/providers\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /albums/{id}/relationships/replacement\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /albums/{id}/relationships/shares\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - r_usr\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /albums/{id}/relationships/similarAlbums\n  method: get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /albums/{id}/relationships/suggestedCoverArts\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - r_usr\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /albums/{id}/relationships/usageRules\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artistBiographies\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artistBiographies/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artistBiographies/{id}\n\
  \  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - w_usr\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /artistBiographies/{id}/relationships/owners\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artistRoles\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artistRoles/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artists\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    scope:\n    - r_usr\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artists\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - w_usr\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /artists/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artists/{id}\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - w_usr\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /artists/{id}/relationships/albums\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artists/{id}/relationships/biography\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artists/{id}/relationships/followers\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artists/{id}/relationships/following\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - w_usr\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /artists/{id}/relationships/following\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artists/{id}/relationships/following\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - w_usr\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /artists/{id}/relationships/owners\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artists/{id}/relationships/profileArt\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /artists/{id}/relationships/profileArt\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - w_usr\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /artists/{id}/relationships/radio\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artists/{id}/relationships/roles\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artists/{id}/relationships/similarArtists\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artists/{id}/relationships/trackProviders\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artists/{id}/relationships/tracks\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artists/{id}/relationships/videos\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artworks\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artworks\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    scope:\n    - w_usr\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /artworks/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artworks/{id}/relationships/owners\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /credits\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /credits/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /credits/{id}/relationships/artist\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /credits/{id}/relationships/category\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /genres\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /genres/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lyrics\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lyrics\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    scope:\n    - w_usr\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lyrics/{id}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lyrics/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lyrics/{id}\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - w_usr\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lyrics/{id}/relationships/owners\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lyrics/{id}/relationships/track\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /providerOwners\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - r_usr\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /providerOwners/{id}/relationships/owners\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - r_usr\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /providerOwners/{id}/relationships/provider\n  method: get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - r_usr\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /providerProductInfos\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - r_usr\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /providerProductInfos/{id}/relationships/provider\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - r_usr\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /providerProductInfos/{id}/relationships/subject\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - r_usr\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /providers\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /providers/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trackStatistics\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - r_usr\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trackStatistics/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - r_usr\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trackStatistics/{id}/relationships/owners\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - r_usr\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tracks\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    scope:\n    - r_usr\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tracks\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - w_usr\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tracks/{id}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - w_usr\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tracks/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tracks/{id}\n  method: patch\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - w_usr\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tracks/{id}/relationships/albums\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tracks/{id}/relationships/albums\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - w_usr\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tracks/{id}/relationships/artists\n  method: get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tracks/{id}/relationships/credits\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tracks/{id}/relationships/download\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tracks/{id}/relationships/genres\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tracks/{id}/relationships/lyrics\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tracks/{id}/relationships/metadataStatus\n  method:\
  \ get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tracks/{id}/relationships/owners\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tracks/{id}/relationships/priceConfig\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tracks/{id}/relationships/providers\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tracks/{id}/relationships/radio\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tracks/{id}/relationships/replacement\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tracks/{id}/relationships/shares\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - r_usr\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tracks/{id}/relationships/similarTracks\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tracks/{id}/relationships/sourceFile\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tracks/{id}/relationships/suggestedTracks\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /tracks/{id}/relationships/trackStatistics\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tracks/{id}/relationships/usageRules\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tracksMetadataStatus\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tracksMetadataStatus/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /videos\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n- path: /videos/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /videos/{id}/relationships/albums\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /videos/{id}/relationships/artists\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /videos/{id}/relationships/credits\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /videos/{id}/relationships/providers\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /videos/{id}/relationships/replacement\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /videos/{id}/relationships/similarVideos\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /videos/{id}/relationships/suggestedVideos\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /videos/{id}/relationships/thumbnailArt\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /videos/{id}/relationships/usageRules\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n   \
  \ subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artistClaims\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - r_usr\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artistClaims\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - w_usr\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /artistClaims/{id}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - w_usr\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /artistClaims/{id}\n  method:\
  \ get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - r_usr\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artistClaims/{id}\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - w_usr\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /artistClaims/{id}/relationships/acceptedArtists\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - r_usr\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artistClaims/{id}/relationships/acceptedArtists\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - w_usr\n    audience: null\n    token:\n \
  \     max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /artistClaims/{id}/relationships/owners\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - r_usr\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artistClaims/{id}/relationships/recommendedArtists\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - r_usr\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contentClaims\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - r_usr\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contentClaims\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    scope:\n    - w_usr\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contentClaims/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - r_usr\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contentClaims/{id}/relationships/claimedResource\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - r_usr\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contentClaims/{id}/relationships/claimingArtist\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - r_usr\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contentClaims/{id}/relationships/owners\n  method: get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - r_usr\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /manualArtistClaims\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - w_usr\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /priceConfigurations\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /priceConfigurations\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - w_usr\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /priceConfigurations/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /purchases\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - r_usr\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /purchases/{id}/relationships/owners\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - r_usr\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /purchases/{id}/relationships/subject\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - r_usr\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /squareConnections\n  method: post\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    scope:\n    - w_usr\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /squareConnections/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - r_usr\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stripeConnections\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - r_usr\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stripeConnections\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - w_usr\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /stripeConnections/{id}/relationships/owners\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - r_usr\n\n\n# --- truncated at 32 KB (82 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/tidal/refs/heads/main/agentic-access/tidal-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tidal/refs/heads/main/agentic-access/tidal-agentic-access.yml
summary_line: 325 operations · 93 acting
tags:
- Music
- Streaming
- Hi-Fi
- HiRes Lossless
- Audio
- Block
- Square
---
