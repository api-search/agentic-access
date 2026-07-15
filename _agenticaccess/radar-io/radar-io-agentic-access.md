---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 19
api_specs:
- filename: radar-io-openapi.yml
  format: yaml
  label: Radar Geocoding API
  slug: radar-geocoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar-io/refs/heads/main/openapi/radar-io-openapi.yml
- filename: radar-io-openapi.yml
  format: yaml
  label: Radar Search & Autocomplete API
  slug: radar-search-autocomplete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar-io/refs/heads/main/openapi/radar-io-openapi.yml
- filename: radar-io-openapi.yml
  format: yaml
  label: Radar Routing, Distance & Matrix API
  slug: radar-routing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar-io/refs/heads/main/openapi/radar-io-openapi.yml
- filename: radar-io-openapi.yml
  format: yaml
  label: Radar Geofences API
  slug: radar-geofences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar-io/refs/heads/main/openapi/radar-io-openapi.yml
- filename: radar-io-openapi.yml
  format: yaml
  label: Radar Track & Users API
  slug: radar-track-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar-io/refs/heads/main/openapi/radar-io-openapi.yml
- filename: radar-io-openapi.yml
  format: yaml
  label: Radar Events API
  slug: radar-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar-io/refs/heads/main/openapi/radar-io-openapi.yml
- filename: radar-io-openapi.yml
  format: yaml
  label: Radar Trips API
  slug: radar-trips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar-io/refs/heads/main/openapi/radar-io-openapi.yml
- filename: radar-io-openapi.yml
  format: yaml
  label: Radar Address Verification API
  slug: radar-address-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar-io/refs/heads/main/openapi/radar-io-openapi.yml
- filename: radar-io-openapi.yml
  format: yaml
  label: Radar Maps & Tiles API
  slug: radar-maps-tiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar-io/refs/heads/main/openapi/radar-io-openapi.yml
consequence_counts:
  read: 19
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Radar Io Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 26
overview: 'Radar exposes 26 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Radar
provider_slug: radar-io
slug: radar-io-agentic-access
source_filename: radar-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/radar-io-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 26\n  by_action_class:\n    connected: 19\n    acting: 7\n  by_consequence:\n    read: 19\n    write: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /geocode/forward\n  method: get\n  operationId: forwardGeocode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /geocode/reverse\n  method: get\n  operationId: reverseGeocode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /geocode/ip\n  method: get\n\
  \  operationId: ipGeocode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/autocomplete\n  method: get\n  operationId: autocomplete\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/places\n  method: get\n  operationId: searchPlaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/geofences\n  method: get\n  operationId: searchGeofences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /route/distance\n  method: get\n  operationId: routeDistance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /route/matrix\n  method: get\n  operationId: routeMatrix\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /route/directions\n  method: get\n  operationId: routeDirections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /route/match\n  method: post\n  operationId: routeMatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /geofences\n  method: get\n  operationId: listGeofences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /geofences/{tag}/{externalId}\n  method: put\n  operationId: upsertGeofence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /geofences/{tag}/{externalId}\n  method: get\n  operationId: getGeofence\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /geofences/{tag}/{externalId}\n  method: delete\n  operationId: deleteGeofence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /track\n  method:\
  \ post\n  operationId: track\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{userId}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{userId}\n  method: delete\n  operationId: deleteUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /events\n  method: get\n  operationId: listEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{eventId}\n  method: get\n  operationId: getEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trips\n  method: get\n  operationId: listTrips\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trips/{externalId}\n  method: post\n  operationId: upsertTrip\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /trips/{externalId}\n  method: get\n  operationId: getTrip\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trips/{externalId}\n  method: patch\n  operationId: updateTrip\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /addresses/validate\n  method: get\n  operationId: validateAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /maps/tiles/{z}/{x}/{y}.png\n  method: get\n  operationId: getRasterTile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/radar-io/refs/heads/main/agentic-access/radar-io-agentic-access.yml
summary_line: 26 operations · 7 acting
tags:
- Location
- Geocoding
- Geofencing
- Maps
- Routing
---
