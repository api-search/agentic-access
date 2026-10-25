---
acting_count: 0
action_class_counts:
  connected: 26
api_specs:
- filename: public-transport-victoria-departures-api-openapi.yml
  format: yaml
  label: Public Transport Victoria Departures API
  slug: public-transport-victoria-departures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/public-transport-victoria/refs/heads/main/openapi/public-transport-victoria-departures-api-openapi.yml
- filename: public-transport-victoria-directions-api-openapi.yml
  format: yaml
  label: Public Transport Victoria Directions API
  slug: public-transport-victoria-directions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/public-transport-victoria/refs/heads/main/openapi/public-transport-victoria-directions-api-openapi.yml
- filename: public-transport-victoria-disruptions-api-openapi.yml
  format: yaml
  label: Public Transport Victoria Disruptions API
  slug: public-transport-victoria-disruptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/public-transport-victoria/refs/heads/main/openapi/public-transport-victoria-disruptions-api-openapi.yml
- filename: public-transport-victoria-fareestimate-api-openapi.yml
  format: yaml
  label: Public Transport Victoria Fare Estimate API
  slug: public-transport-victoria-fareestimate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/public-transport-victoria/refs/heads/main/openapi/public-transport-victoria-fareestimate-api-openapi.yml
- filename: public-transport-victoria-outlets-api-openapi.yml
  format: yaml
  label: Public Transport Victoria Outlets API
  slug: public-transport-victoria-outlets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/public-transport-victoria/refs/heads/main/openapi/public-transport-victoria-outlets-api-openapi.yml
- filename: public-transport-victoria-patterns-api-openapi.yml
  format: yaml
  label: Public Transport Victoria Patterns API
  slug: public-transport-victoria-patterns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/public-transport-victoria/refs/heads/main/openapi/public-transport-victoria-patterns-api-openapi.yml
- filename: public-transport-victoria-routes-api-openapi.yml
  format: yaml
  label: Public Transport Victoria Routes API
  slug: public-transport-victoria-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/public-transport-victoria/refs/heads/main/openapi/public-transport-victoria-routes-api-openapi.yml
- filename: public-transport-victoria-routetypes-api-openapi.yml
  format: yaml
  label: Public Transport Victoria Route Types API
  slug: public-transport-victoria-routetypes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/public-transport-victoria/refs/heads/main/openapi/public-transport-victoria-routetypes-api-openapi.yml
- filename: public-transport-victoria-runs-api-openapi.yml
  format: yaml
  label: Public Transport Victoria Runs API
  slug: public-transport-victoria-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/public-transport-victoria/refs/heads/main/openapi/public-transport-victoria-runs-api-openapi.yml
- filename: public-transport-victoria-search-api-openapi.yml
  format: yaml
  label: Public Transport Victoria Search API
  slug: public-transport-victoria-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/public-transport-victoria/refs/heads/main/openapi/public-transport-victoria-search-api-openapi.yml
- filename: public-transport-victoria-stops-api-openapi.yml
  format: yaml
  label: Public Transport Victoria Stops API
  slug: public-transport-victoria-stops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/public-transport-victoria/refs/heads/main/openapi/public-transport-victoria-stops-api-openapi.yml
consequence_counts:
  read: 26
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Public Transport Victoria Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 26
overview: 'Public Transport Victoria exposes 26 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 26 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Public Transport Victoria
provider_slug: public-transport-victoria
slug: public-transport-victoria-agentic-access
source_filename: public-transport-victoria-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: generated\nsource: openapi/public-transport-victoria-timetable-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 26\n  by_action_class:\n    connected: 26\n  by_consequence:\n    read: 26\n  human_in_the_loop_required: 0\noperations:\n- path: /v3/departures/route_type/{route_type}/stop/{stop_id}\n  method: get\n  operationId: Departures_GetForStop\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/departures/route_type/{route_type}/stop/{stop_id}/route/{route_id}\n  method: get\n  operationId: Departures_GetForStopAndRoute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/directions/route/{route_id}\n  method: get\n  operationId: Directions_ForRoute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/directions/{direction_id}\n  method: get\n  operationId: Directions_ForDirection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/directions/{direction_id}/route_type/{route_type}\n  method: get\n  operationId: Directions_ForDirectionAndType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/disruptions\n  method: get\n  operationId: Disruptions_GetAllDisruptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/disruptions/route/{route_id}\n  method: get\n  operationId: Disruptions_GetDisruptionsByRoute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/disruptions/route/{route_id}/stop/{stop_id}\n  method: get\n  operationId: Disruptions_GetDisruptionsByRouteAndStop\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/disruptions/stop/{stop_id}\n  method: get\n  operationId: Disruptions_GetDisruptionsByStop\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/disruptions/{disruption_id}\n  method: get\n  operationId: Disruptions_GetDisruptionById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/disruptions/modes\n  method: get\n  operationId: Disruptions_GetDisruptionModes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/fare_estimate/min_zone/{minZone}/max_zone/{maxZone}\n  method: get\n  operationId: FareEstimate_GetFareEstimateByZone\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/outlets\n  method: get\n  operationId: Outlets_GetAllOutlets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/outlets/location/{latitude},{longitude}\n  method: get\n  operationId: Outlets_GetOutletsByGeolocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/pattern/run/{run_ref}/route_type/{route_type}\n  method: get\n  operationId: Patterns_GetPatternByRun\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/routes\n  method: get\n  operationId: Routes_OneOrMoreRoutes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/routes/{route_id}\n  method: get\n  operationId: Routes_RouteFromId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/route_types\n  method: get\n  operationId: RouteTypes_GetRouteTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v3/runs/route/{route_id}\n  method: get\n  operationId: Runs_ForRoute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/runs/route/{route_id}/route_type/{route_type}\n  method: get\n  operationId: Runs_ForRouteAndRouteType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/runs/{run_ref}\n  method: get\n  operationId: Runs_ForRun\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/runs/{run_ref}/route_type/{route_type}\n  method: get\n  operationId: Runs_ForRunAndRouteType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/search/{search_term}\n\
  \  method: get\n  operationId: Search_Search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/stops/{stop_id}/route_type/{route_type}\n  method: get\n  operationId: Stops_StopDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/stops/route/{route_id}/route_type/{route_type}\n  method: get\n  operationId: Stops_StopsForRoute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/stops/location/{latitude},{longitude}\n  method: get\n  operationId: Stops_StopsByGeolocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/public-transport-victoria/refs/heads/main/agentic-access/public-transport-victoria-agentic-access.yml
summary_line: 26 operations
tags:
- Company
- Public Transport
- Government
- Transit
- Timetables
- Australia
- Open Data
---
