---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 7
api_specs:
- filename: openrouteservice-directions-api-openapi.yml
  format: yaml
  label: OpenRouteService Directions API
  slug: openrouteservice-directions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrouteservice/refs/heads/main/openapi/openrouteservice-directions-api-openapi.yml
- filename: openrouteservice-elevation-api-openapi.yml
  format: yaml
  label: OpenRouteService Elevation API
  slug: openrouteservice-elevation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrouteservice/refs/heads/main/openapi/openrouteservice-elevation-api-openapi.yml
- filename: openrouteservice-geocoding-api-openapi.yml
  format: yaml
  label: OpenRouteService Geocoding API
  slug: openrouteservice-geocoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrouteservice/refs/heads/main/openapi/openrouteservice-geocoding-api-openapi.yml
- filename: openrouteservice-health-api-openapi.yml
  format: yaml
  label: OpenRouteService Health API
  slug: openrouteservice-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrouteservice/refs/heads/main/openapi/openrouteservice-health-api-openapi.yml
- filename: openrouteservice-isochrones-api-openapi.yml
  format: yaml
  label: OpenRouteService Isochrones API
  slug: openrouteservice-isochrones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrouteservice/refs/heads/main/openapi/openrouteservice-isochrones-api-openapi.yml
- filename: openrouteservice-matrix-api-openapi.yml
  format: yaml
  label: OpenRouteService Matrix API
  slug: openrouteservice-matrix-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrouteservice/refs/heads/main/openapi/openrouteservice-matrix-api-openapi.yml
- filename: openrouteservice-optimization-api-openapi.yml
  format: yaml
  label: OpenRouteService Optimization API
  slug: openrouteservice-optimization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrouteservice/refs/heads/main/openapi/openrouteservice-optimization-api-openapi.yml
- filename: openrouteservice-poi-api-openapi.yml
  format: yaml
  label: OpenRouteService POI API
  slug: openrouteservice-poi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrouteservice/refs/heads/main/openapi/openrouteservice-poi-api-openapi.yml
- filename: openrouteservice-snapping-api-openapi.yml
  format: yaml
  label: OpenRouteService Snapping API
  slug: openrouteservice-snapping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrouteservice/refs/heads/main/openapi/openrouteservice-snapping-api-openapi.yml
consequence_counts:
  read: 7
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Openrouteservice Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'OpenRouteService exposes 17 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 10 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: OpenRouteService
provider_slug: openrouteservice
slug: openrouteservice-agentic-access
source_filename: openrouteservice-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openrouteservice-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    connected: 7\n    acting: 10\n  by_consequence:\n    read: 7\n    write: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/directions/{profile}\n  method: get\n  operationId: getDirectionsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/directions/{profile}\n  method: post\n  operationId: getDirectionsPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/directions/{profile}/geojson\n  method: post\n  operationId: getDirectionsGeoJson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/directions/{profile}/gpx\n  method: post\n  operationId: getDirectionsGpx\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/isochrones/{profile}\n  method: post\n  operationId: getIsochrones\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/matrix/{profile}\n  method: post\n  operationId: getMatrix\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /geocode/search\n  method: get\n  operationId: geocodeSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /geocode/reverse\n  method: get\n  operationId: geocodeReverse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /geocode/autocomplete\n\
  \  method: get\n  operationId: geocodeAutocomplete\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /elevation/point\n  method: get\n  operationId: getElevationPoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /elevation/point\n  method: post\n  operationId: postElevationPoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /elevation/line\n  method: post\n  operationId: getElevationLine\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /optimization\n  method: post\n  operationId: getOptimization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pois\n  method: post\n  operationId: getPOIs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/snap/{profile}\n  method: post\n  operationId: snapCoordinates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n  \
  \    max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/status\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openrouteservice/refs/heads/main/agentic-access/openrouteservice-agentic-access.yml
summary_line: 17 operations · 10 acting
tags:
- Routing
- Geospatial
- Directions
- Isochrones
- Matrix
- Geocoding
- Elevation
- Optimization
- OpenStreetMap
- Navigation
- Logistics
- Humanitarian
---
