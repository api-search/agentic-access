---
acting_count: 0
action_class_counts:
  connected: 7
api_specs:
- filename: transit-alerts-api-openapi.yml
  format: yaml
  label: Transit Alerts API
  slug: transit-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transit/refs/heads/main/openapi/transit-alerts-api-openapi.yml
- filename: transit-departures-api-openapi.yml
  format: yaml
  label: Transit Departures API
  slug: transit-departures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transit/refs/heads/main/openapi/transit-departures-api-openapi.yml
- filename: transit-mobility-api-openapi.yml
  format: yaml
  label: Transit Mobility API
  slug: transit-mobility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transit/refs/heads/main/openapi/transit-mobility-api-openapi.yml
- filename: transit-networks-api-openapi.yml
  format: yaml
  label: Transit Networks API
  slug: transit-networks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transit/refs/heads/main/openapi/transit-networks-api-openapi.yml
- filename: transit-routes-api-openapi.yml
  format: yaml
  label: Transit Routes API
  slug: transit-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transit/refs/heads/main/openapi/transit-routes-api-openapi.yml
- filename: transit-stops-api-openapi.yml
  format: yaml
  label: Transit Stops API
  slug: transit-stops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transit/refs/heads/main/openapi/transit-stops-api-openapi.yml
- filename: transit-trips-api-openapi.yml
  format: yaml
  label: Transit Trips API
  slug: transit-trips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transit/refs/heads/main/openapi/transit-trips-api-openapi.yml
consequence_counts:
  read: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Transit Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Transit exposes 7 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Transit
provider_slug: transit
slug: transit-agentic-access
source_filename: transit-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/transit-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 7\n  by_consequence:\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /public/stop_departures\n  method: get\n  operationId: getStopDepartures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/networks\n  method: get\n  operationId: listNetworks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/routes\n  method: get\n  operationId: listRoutes\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/stops\n  method: get\n  operationId: listStops\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/trip\n  method: get\n  operationId: planTrip\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/alerts\n  method: get\n  operationId: getServiceAlerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/nearby_vehicles\n  method: get\n  operationId: getNearbyVehicles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transit/refs/heads/main/agentic-access/transit-agentic-access.yml
summary_line: 7 operations
tags:
- Public Transit
- Real-Time
- Trip Planning
- Multi-Modal
- GTFS
- GOFS
- Mobility
- Shared Mobility
---
