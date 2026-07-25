---
acting_count: 0
action_class_counts:
  connected: 8
api_specs:
- filename: foursquare-ask-api-openapi.yml
  format: yaml
  label: Foursquare Ask API
  slug: foursquare-ask-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/foursquare/refs/heads/main/openapi/foursquare-ask-api-openapi.yml
- filename: foursquare-autocomplete-api-openapi.yml
  format: yaml
  label: Foursquare Autocomplete API
  slug: foursquare-autocomplete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/foursquare/refs/heads/main/openapi/foursquare-autocomplete-api-openapi.yml
- filename: foursquare-details-api-openapi.yml
  format: yaml
  label: Foursquare Details API
  slug: foursquare-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/foursquare/refs/heads/main/openapi/foursquare-details-api-openapi.yml
- filename: foursquare-geotagging-api-openapi.yml
  format: yaml
  label: Foursquare Geotagging API
  slug: foursquare-geotagging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/foursquare/refs/heads/main/openapi/foursquare-geotagging-api-openapi.yml
- filename: foursquare-match-api-openapi.yml
  format: yaml
  label: Foursquare Match API
  slug: foursquare-match-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/foursquare/refs/heads/main/openapi/foursquare-match-api-openapi.yml
- filename: foursquare-photos-api-openapi.yml
  format: yaml
  label: Foursquare Photos API
  slug: foursquare-photos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/foursquare/refs/heads/main/openapi/foursquare-photos-api-openapi.yml
- filename: foursquare-search-api-openapi.yml
  format: yaml
  label: Foursquare Search API
  slug: foursquare-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/foursquare/refs/heads/main/openapi/foursquare-search-api-openapi.yml
- filename: foursquare-tips-api-openapi.yml
  format: yaml
  label: Foursquare Tips API
  slug: foursquare-tips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/foursquare/refs/heads/main/openapi/foursquare-tips-api-openapi.yml
consequence_counts:
  read: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Foursquare Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Foursquare exposes 8 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Foursquare
provider_slug: foursquare
slug: foursquare-agentic-access
source_filename: foursquare-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/foursquare-places-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 8\n  by_consequence:\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /places/search\n  method: get\n  operationId: searchPlaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autocomplete\n  method: get\n  operationId: autocomplete\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /places/match\n  method: get\n  operationId: matchPlace\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /places/ask\n  method: get\n  operationId: askPlaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /geotagging/candidates\n  method: get\n  operationId: geotaggingCandidates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /places/{fsq_place_id}\n  method: get\n  operationId: getPlace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /places/{fsq_place_id}/photos\n  method: get\n  operationId: getPlacePhotos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n    \
  \  max-ttl: 3600\n    audit: none\n- path: /places/{fsq_place_id}/tips\n  method: get\n  operationId: getPlaceTips\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/foursquare/refs/heads/main/agentic-access/foursquare-agentic-access.yml
summary_line: 8 operations
tags:
- Restaurant
- Locations
- Places
- Geocoding
- Recommendations
- Reviews
- Movement
---
