---
acting_count: 0
action_class_counts:
  connected: 16
api_specs:
- filename: transit-openapi.yml
  format: yaml
  label: Transit API
  slug: transit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transit-app/refs/heads/main/openapi/transit-openapi.yml
consequence_counts:
  read: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Transit App Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'Transit exposes 16 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Transit
provider_slug: transit-app
slug: transit-app-agentic-access
source_filename: transit-app-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/transit-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 16\n  by_consequence:\n    read: 16\n  human_in_the_loop_required: 0\noperations:\n- path: /v4/public/nearby_routes\n  method: get\n  operationId: /v4/public/nearby_routes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/public/nearby_stops\n  method: get\n  operationId: /v4/public/nearby_stops\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/public/stop_departures\n\
  \  method: get\n  operationId: /v4/public/stop_departures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/public/estimate_plan_duration\n  method: get\n  operationId: /v4/public/estimate_plan_duration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/public/plan\n  method: get\n  operationId: /v4/public/plan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /map_layers/placemarks\n  method: get\n  operationId: /map_layers/placemarks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/public/available_networks\n  method: get\n  operationId: /v4/public/available_networks\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /map_layers/available_networks\n  method: get\n  operationId: /map_layers/available_networks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/public/route_details\n  method: get\n  operationId: /v4/public/route_details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/public/routes_for_networks\n  method: get\n  operationId: /v4/public/routes_for_networks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/public/stops_for_network\n  method: get\n  operationId: /v4/public/stops_for_network\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/public/alerts_for_networks\n  method: get\n  operationId: /v4/public/alerts_for_networks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/public/latest_update_for_network\n  method: get\n  operationId: /v4/public/latest_update_for_network\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/public/search_stops\n  method: get\n  operationId: /v4/public/search_stops\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/public/trip_details\n  method: get\n  operationId: /v4/public/trip_details\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/vehicles\n  method: get\n  operationId: /v4/vehicles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transit-app/refs/heads/main/agentic-access/transit-app-agentic-access.yml
summary_line: 16 operations
tags:
- Transit
- Public Transit
- Multimodal
- Mobility
- Trip Planning
- Routing
- Real-Time
- GTFS
- GOFS
- Bikeshare
- Scooters
- Carshare
- On-Demand Transit
- Service Alerts
- Shared Mobility
- Crowdsourced Data
---
