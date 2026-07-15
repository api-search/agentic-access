---
acting_count: 0
action_class_counts:
  connected: 15
api_specs:
- filename: swagger.json
  format: json
  label: setlist.fm API
  slug: setlist-fm-api
  spec_type: OpenAPI
  url: https://api.setlist.fm/docs/1.0/ui/swagger.json
consequence_counts:
  read: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Setlist Fm Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'setlist.fm exposes 15 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: setlist.fm
provider_slug: setlist-fm
slug: setlist-fm-agentic-access
source_filename: setlist-fm-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/setlist-fm-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 15\n  by_consequence:\n    read: 15\n  human_in_the_loop_required: 0\noperations:\n- path: /1.0/artist/{mbid}\n  method: get\n  operationId: resource__1.0_artist__mbid__getArtist_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1.0/artist/{mbid}/setlists\n  method: get\n  operationId: resource__1.0_artist__mbid__setlists_getArtistSetlists_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /1.0/city/{geoId}\n  method: get\n  operationId: resource__1.0_city__geoId__getCity_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1.0/search/artists\n  method: get\n  operationId: resource__1.0_search_artists_getArtists_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1.0/search/cities\n  method: get\n  operationId: resource__1.0_search_cities_getCities_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1.0/search/countries\n  method: get\n  operationId: resource__1.0_search_countries_getCountries_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /1.0/search/setlists\n  method: get\n  operationId: resource__1.0_search_setlists_getSetlists_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1.0/search/venues\n  method: get\n  operationId: resource__1.0_search_venues_getVenues_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1.0/setlist/version/{versionId}\n  method: get\n  operationId: resource__1.0_setlist_version__versionId__getSetlistVersion_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1.0/setlist/{setlistId}\n  method: get\n  operationId: resource__1.0_setlist__setlistId__getSetlist_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1.0/user/{userId}\n  method: get\n  operationId: resource__1.0_user__userId__getUser_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1.0/user/{userId}/attended\n  method: get\n  operationId: resource__1.0_user__userId__attended_getUserAttendedSetlists_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1.0/user/{userId}/edited\n  method: get\n  operationId: resource__1.0_user__userId__edited_getUserEditedSetlists_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1.0/venue/{venueId}\n  method: get\n  operationId: resource__1.0_venue__venueId__getVenue_GET\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1.0/venue/{venueId}/setlists\n  method: get\n  operationId: resource__1.0_venue__venueId__setlists_getVenueSetlists_GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/setlist-fm/refs/heads/main/agentic-access/setlist-fm-agentic-access.yml
summary_line: 15 operations
tags:
- Music
- Concerts
- Setlists
- Live Music
- Venues
- Artists
- Tour Dates
- Events
---
