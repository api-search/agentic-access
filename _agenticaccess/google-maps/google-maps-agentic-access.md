---
acting_count: 0
action_class_counts:
  connected: 7
api_specs:
- filename: google-maps-autocomplete-api-openapi.yml
  format: yaml
  label: Google Maps Platform Autocomplete API
  slug: google-maps-autocomplete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-maps/refs/heads/main/openapi/google-maps-autocomplete-api-openapi.yml
- filename: google-maps-directions-api-openapi.yml
  format: yaml
  label: Google Maps Platform Directions API
  slug: google-maps-directions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-maps/refs/heads/main/openapi/google-maps-directions-api-openapi.yml
- filename: google-maps-geocoding-api-openapi.yml
  format: yaml
  label: Google Maps Platform Geocoding API
  slug: google-maps-geocoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-maps/refs/heads/main/openapi/google-maps-geocoding-api-openapi.yml
- filename: google-maps-nearby-search-api-openapi.yml
  format: yaml
  label: Google Maps Platform Nearby Search API
  slug: google-maps-nearby-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-maps/refs/heads/main/openapi/google-maps-nearby-search-api-openapi.yml
- filename: google-maps-photos-api-openapi.yml
  format: yaml
  label: Google Maps Platform Photos API
  slug: google-maps-photos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-maps/refs/heads/main/openapi/google-maps-photos-api-openapi.yml
- filename: google-maps-place-details-api-openapi.yml
  format: yaml
  label: Google Maps Platform Place Details API
  slug: google-maps-place-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-maps/refs/heads/main/openapi/google-maps-place-details-api-openapi.yml
- filename: google-maps-text-search-api-openapi.yml
  format: yaml
  label: Google Maps Platform Text Search API
  slug: google-maps-text-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-maps/refs/heads/main/openapi/google-maps-text-search-api-openapi.yml
consequence_counts:
  read: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Google Maps Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Google Maps Platform exposes 7 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Google Maps Platform
provider_slug: google-maps
slug: google-maps-agentic-access
source_filename: google-maps-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/google-maps-autocomplete-api-openapi.yml, openapi/google-maps-directions-api-openapi.yml,\n  openapi/google-maps-geocoding-api-openapi.yml, openapi/google-maps-nearby-search-api-openapi.yml,\n  openapi/google-maps-photos-api-openapi.yml, openapi/google-maps-place-details-api-openapi.yml,\n  openapi/google-maps-text-search-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 7\n  by_consequence:\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /places:autocomplete\n  method: post\n  operationId: autocompletePlaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /directions/json\n  method: get\n  operationId: getDirections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /geocode/json\n  method: get\n  operationId: geocode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /places:searchNearby\n  method: post\n  operationId: searchPlacesNearby\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /places/{placeId}/photos/{photoReference}/media\n  method: get\n  operationId: getPlacePhoto\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /places/{placeId}\n  method: get\n  operationId: getPlaceDetails\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /places:searchText\n  method: post\n  operationId: searchPlacesText\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-maps/refs/heads/main/agentic-access/google-maps-agentic-access.yml
summary_line: 7 operations
tags:
- Environment
- Geocoding
- Geolocation
- Maps
- Navigation
- Places
- Routing
- Solar
- Geospatial
---
