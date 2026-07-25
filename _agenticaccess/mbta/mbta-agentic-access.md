---
acting_count: 0
action_class_counts:
  connected: 22
api_specs:
- filename: mbta-alerts-api-openapi.yml
  format: yaml
  label: MBTA Alerts API
  slug: mbta-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mbta/refs/heads/main/openapi/mbta-alerts-api-openapi.yml
- filename: mbta-facilities-api-openapi.yml
  format: yaml
  label: MBTA Facilities API
  slug: mbta-facilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mbta/refs/heads/main/openapi/mbta-facilities-api-openapi.yml
- filename: mbta-lines-api-openapi.yml
  format: yaml
  label: MBTA Lines API
  slug: mbta-lines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mbta/refs/heads/main/openapi/mbta-lines-api-openapi.yml
- filename: mbta-predictions-api-openapi.yml
  format: yaml
  label: MBTA Predictions API
  slug: mbta-predictions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mbta/refs/heads/main/openapi/mbta-predictions-api-openapi.yml
- filename: mbta-routepatterns-api-openapi.yml
  format: yaml
  label: MBTA RoutePatterns API
  slug: mbta-routepatterns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mbta/refs/heads/main/openapi/mbta-routepatterns-api-openapi.yml
- filename: mbta-routes-api-openapi.yml
  format: yaml
  label: MBTA Routes API
  slug: mbta-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mbta/refs/heads/main/openapi/mbta-routes-api-openapi.yml
- filename: mbta-schedules-api-openapi.yml
  format: yaml
  label: MBTA Schedules API
  slug: mbta-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mbta/refs/heads/main/openapi/mbta-schedules-api-openapi.yml
- filename: mbta-services-api-openapi.yml
  format: yaml
  label: MBTA Services API
  slug: mbta-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mbta/refs/heads/main/openapi/mbta-services-api-openapi.yml
- filename: mbta-shapes-api-openapi.yml
  format: yaml
  label: MBTA Shapes API
  slug: mbta-shapes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mbta/refs/heads/main/openapi/mbta-shapes-api-openapi.yml
- filename: mbta-stops-api-openapi.yml
  format: yaml
  label: MBTA Stops API
  slug: mbta-stops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mbta/refs/heads/main/openapi/mbta-stops-api-openapi.yml
- filename: mbta-trips-api-openapi.yml
  format: yaml
  label: MBTA Trips API
  slug: mbta-trips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mbta/refs/heads/main/openapi/mbta-trips-api-openapi.yml
- filename: mbta-vehicles-api-openapi.yml
  format: yaml
  label: MBTA Vehicles API
  slug: mbta-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mbta/refs/heads/main/openapi/mbta-vehicles-api-openapi.yml
consequence_counts:
  read: 22
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Mbta Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 22
overview: 'MBTA exposes 22 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: MBTA
provider_slug: mbta
slug: mbta-agentic-access
source_filename: mbta-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/mbta-mbta-v3-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 22\n  by_consequence:\n    read: 22\n  human_in_the_loop_required: 0\noperations:\n- path: /alerts\n  method: get\n  operationId: listAlerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /alerts/{id}\n  method: get\n  operationId: getAlert\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /facilities\n  method: get\n  operationId: listFacilities\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /facilities/{id}\n  method: get\n  operationId: getFacility\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lines\n  method: get\n  operationId: listLines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lines/{id}\n  method: get\n  operationId: getLine\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /predictions\n  method: get\n  operationId: listPredictions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /routes\n  method: get\n  operationId:\
  \ listRoutes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /routes/{id}\n  method: get\n  operationId: getRoute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /route_patterns\n  method: get\n  operationId: listRoutePatterns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /route_patterns/{id}\n  method: get\n  operationId: getRoutePattern\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schedules\n  method: get\n  operationId: listSchedules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /services\n  method: get\n  operationId: listServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/{id}\n  method: get\n  operationId: getService\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shapes\n  method: get\n  operationId: listShapes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shapes/{id}\n  method: get\n  operationId: getShape\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stops\n  method: get\n  operationId: listStops\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /stops/{id}\n  method: get\n  operationId: getStop\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trips\n  method: get\n  operationId: listTrips\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trips/{id}\n  method: get\n  operationId: getTrip\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vehicles\n  method: get\n  operationId: listVehicles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vehicles/{id}\n  method: get\n  operationId: getVehicle\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mbta/refs/heads/main/agentic-access/mbta-agentic-access.yml
summary_line: 22 operations
tags:
- Boston
- Massachusetts
- Public Transportation
- Real-Time
- Transit
---
