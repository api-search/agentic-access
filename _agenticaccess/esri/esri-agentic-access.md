---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 13
api_specs:
- filename: esri-auth-api-openapi.yml
  format: yaml
  label: Esri Auth API
  slug: esri-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esri/refs/heads/main/openapi/esri-auth-api-openapi.yml
- filename: esri-geocoding-api-openapi.yml
  format: yaml
  label: Esri Geocoding API
  slug: esri-geocoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esri/refs/heads/main/openapi/esri-geocoding-api-openapi.yml
- filename: esri-routing-api-openapi.yml
  format: yaml
  label: Esri Routing API
  slug: esri-routing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esri/refs/heads/main/openapi/esri-routing-api-openapi.yml
- filename: esri-places-api-openapi.yml
  format: yaml
  label: Esri Places API
  slug: esri-places-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esri/refs/heads/main/openapi/esri-places-api-openapi.yml
- filename: esri-portal-api-openapi.yml
  format: yaml
  label: Esri Portal API
  slug: esri-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esri/refs/heads/main/openapi/esri-portal-api-openapi.yml
consequence_counts:
  read: 13
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Esri Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'Esri exposes 15 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Esri
provider_slug: esri
slug: esri-agentic-access
source_filename: esri-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-22'\nmethod: generated\nsource: openapi/esri-arcgis-geocoding-api-openapi.yml, openapi/esri-arcgis-places-api-openapi.yml,\n  openapi/esri-arcgis-portal-api-openapi.yml, openapi/esri-auth-api-openapi.yml, openapi/esri-geocoding-api-openapi.yml,\n  openapi/esri-routing-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 13\n    acting: 2\n  by_consequence:\n    read: 13\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /findAddressCandidates\n  method: get\n  operationId: findAddressCandidates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n   \
  \ - openid\n- path: /reverseGeocode\n  method: get\n  operationId: reverseGeocode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - openid\n- path: /places/near-point\n  method: get\n  operationId: findPlacesNearPoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - openid\n- path: /places/{placeId}\n  method: get\n  operationId: getPlaceDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - openid\n- path: /portals/self\n  method: get\n  operationId: getPortalSelf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - openid\n- path:\
  \ /community/users/{username}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - openid\n- path: /content/users/{username}/items\n  method: get\n  operationId: getUserItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - openid\n- path: /content/items/{itemId}\n  method: get\n  operationId: getItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - openid\n- path: /search\n  method: get\n  operationId: searchPortal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - openid\n- path: /sharing/rest/oauth2/token\n\
  \  method: post\n  operationId: getOAuthToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /World/GeocodeServer/findAddressCandidates\n  method: get\n  operationId: findAddressCandidates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /World/GeocodeServer/geocodeAddresses\n  method: post\n  operationId: geocodeAddresses\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /World/GeocodeServer/reverseGeocode\n  method:\
  \ get\n  operationId: reverseGeocode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /World/GeocodeServer/suggest\n  method: get\n  operationId: suggestAddresses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /World/Route/NAServer/Route_World/solve\n  method: get\n  operationId: solveRoute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/esri/refs/heads/main/agentic-access/esri-agentic-access.yml
summary_line: 15 operations · 2 acting
tags:
- Geographic
- Geospatial
- GIS
- Location
- Mapping
- Maps
- Spatial Analysis
- Geocoding
- Routing
---
