---
acting_count: 0
action_class_counts:
  connected: 7
api_specs:
- filename: opensky-rest-api.json
  format: json
  label: OpenSky Network REST API
  slug: opensky-network-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensky/refs/heads/main/openapi/opensky-rest-api.json
consequence_counts:
  read: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Opensky Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'OpenSky Network exposes 7 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: OpenSky Network
provider_slug: opensky
slug: opensky-agentic-access
source_filename: opensky-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/opensky-rest-api.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 7\n  by_consequence:\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /states/all\n  method: get\n  operationId: getStateVectorsAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /states/own\n  method: get\n  operationId: getOwnStateVectors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /flights/all\n  method: get\n  operationId: getFlightsAll\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /flights/aircraft\n  method: get\n  operationId: getFlightsByAircraft\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /flights/arrival\n  method: get\n  operationId: getFlightsByArrivalAirport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /flights/departure\n  method: get\n  operationId: getFlightsByDepartureAirport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tracks\n  method: get\n  operationId: getTrackByAircraft\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opensky/refs/heads/main/agentic-access/opensky-agentic-access.yml
summary_line: 7 operations
tags:
- Aviation
- Flight Tracking
- ADS-B
- Aircraft
- Airport
- Real-Time
- Historical Data
---
