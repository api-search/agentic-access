---
acting_count: 0
action_class_counts:
  connected: 9
api_specs:
- filename: esri-arcgis-platform-openapi.yml
  format: yaml
  label: ESRI ArcGIS Platform API
  slug: esri-arcgis-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esri-arcgis/refs/heads/main/openapi/esri-arcgis-platform-openapi.yml
consequence_counts:
  read: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Esri Arcgis Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'ESRI ArcGIS exposes 9 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ESRI ArcGIS
provider_slug: esri-arcgis
slug: esri-arcgis-agentic-access
source_filename: esri-arcgis-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/esri-arcgis-platform-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 9\n  by_consequence:\n    read: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /portals/self\n  method: get\n  operationId: getPortalSelf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - openid\n- path: /community/users/{username}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - openid\n- path:\
  \ /content/users/{username}/items\n  method: get\n  operationId: getUserItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - openid\n- path: /content/items/{itemId}\n  method: get\n  operationId: getItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - openid\n- path: /search\n  method: get\n  operationId: searchPortal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - openid\n- path: /findAddressCandidates\n  method: get\n  operationId: findAddressCandidates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - openid\n- path: /reverseGeocode\n\
  \  method: get\n  operationId: reverseGeocode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - openid\n- path: /places/near-point\n  method: get\n  operationId: findPlacesNearPoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - openid\n- path: /places/{placeId}\n  method: get\n  operationId: getPlaceDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - openid\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/esri-arcgis/refs/heads/main/agentic-access/esri-arcgis-agentic-access.yml
summary_line: 9 operations
tags:
- GIS
- Geospatial
- Mapping
- Location
- Spatial Analysis
---
