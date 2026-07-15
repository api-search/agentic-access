---
acting_count: 0
action_class_counts:
  connected: 15
api_specs:
- filename: setlistfm-openapi.yml
  format: yaml
  label: setlist.fm Artists API
  slug: setlistfm-artists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/setlistfm/refs/heads/main/openapi/setlistfm-openapi.yml
- filename: setlistfm-openapi.yml
  format: yaml
  label: setlist.fm Setlists API
  slug: setlistfm-setlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/setlistfm/refs/heads/main/openapi/setlistfm-openapi.yml
- filename: setlistfm-openapi.yml
  format: yaml
  label: setlist.fm Venues API
  slug: setlistfm-venues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/setlistfm/refs/heads/main/openapi/setlistfm-openapi.yml
- filename: setlistfm-openapi.yml
  format: yaml
  label: setlist.fm Cities API
  slug: setlistfm-cities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/setlistfm/refs/heads/main/openapi/setlistfm-openapi.yml
- filename: setlistfm-openapi.yml
  format: yaml
  label: setlist.fm Countries API
  slug: setlistfm-countries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/setlistfm/refs/heads/main/openapi/setlistfm-openapi.yml
- filename: setlistfm-openapi.yml
  format: yaml
  label: setlist.fm Search API
  slug: setlistfm-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/setlistfm/refs/heads/main/openapi/setlistfm-openapi.yml
- filename: setlistfm-openapi.yml
  format: yaml
  label: setlist.fm User API
  slug: setlistfm-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/setlistfm/refs/heads/main/openapi/setlistfm-openapi.yml
consequence_counts:
  read: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Setlistfm Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'setlist.fm exposes 15 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: setlist.fm
provider_slug: setlistfm
slug: setlistfm-agentic-access
source_filename: setlistfm-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/setlistfm-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 15\n  by_consequence:\n    read: 15\n  human_in_the_loop_required: 0\noperations:\n- path: /artist/{mbid}\n  method: get\n  operationId: getArtist\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artist/{mbid}/setlists\n  method: get\n  operationId: getArtistSetlists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /setlist/{setlistId}\n  method: get\n  operationId:\
  \ getSetlist\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /setlist/version/{versionId}\n  method: get\n  operationId: getSetlistVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /venue/{venueId}\n  method: get\n  operationId: getVenue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /venue/{venueId}/setlists\n  method: get\n  operationId: getVenueSetlists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /city/{geoId}\n  method: get\n  operationId: getCity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /search/artists\n  method: get\n  operationId: searchArtists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/venues\n  method: get\n  operationId: searchVenues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/cities\n  method: get\n  operationId: searchCities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/countries\n  method: get\n  operationId: searchCountries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/setlists\n  method: get\n  operationId: searchSetlists\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/{userId}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/{userId}/attended\n  method: get\n  operationId: getUserAttended\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/{userId}/edited\n  method: get\n  operationId: getUserEdited\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/setlistfm/refs/heads/main/agentic-access/setlistfm-agentic-access.yml
summary_line: 15 operations
tags:
- Music
- Concerts
- Setlists
- Live Music
- Database
- Crowd-Sourced
- Entertainment
---
