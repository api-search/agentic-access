---
acting_count: 0
action_class_counts:
  connected: 20
api_specs:
- filename: sound-transit-onebusaway-openapi.yml
  format: yaml
  label: Sound Transit OneBusAway API
  slug: sound-transit-onebusaway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sound-transit/refs/heads/main/openapi/sound-transit-onebusaway-openapi.yml
consequence_counts:
  read: 20
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sound Transit Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 20
overview: 'Sound Transit exposes 20 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Sound Transit
provider_slug: sound-transit
slug: sound-transit-agentic-access
source_filename: sound-transit-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/sound-transit-onebusaway-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    connected: 20\n  by_consequence:\n    read: 20\n  human_in_the_loop_required: 0\noperations:\n- path: /agencies-with-coverage.json\n  method: get\n  operationId: listAgenciesWithCoverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agency/{id}.json\n  method: get\n  operationId: getAgency\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /route/{id}.json\n  method:\
  \ get\n  operationId: getRoute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /routes-for-agency/{id}.json\n  method: get\n  operationId: listRoutesForAgency\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /routes-for-location.json\n  method: get\n  operationId: listRoutesForLocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stop/{id}.json\n  method: get\n  operationId: getStop\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stops-for-location.json\n  method: get\n  operationId: listStopsForLocation\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stops-for-route/{id}.json\n  method: get\n  operationId: listStopsForRoute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schedule-for-stop/{id}.json\n  method: get\n  operationId: getScheduleForStop\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /arrivals-and-departures-for-stop/{id}.json\n  method: get\n  operationId: getArrivalsAndDeparturesForStop\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /arrival-and-departure-for-stop/{id}.json\n  method: get\n  operationId: getArrivalAndDepartureForStop\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trip/{id}.json\n  method: get\n  operationId: getTrip\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trip-details/{id}.json\n  method: get\n  operationId: getTripDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trips-for-route/{id}.json\n  method: get\n  operationId: listTripsForRoute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trips-for-location.json\n  method: get\n  operationId: listTripsForLocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trip-for-vehicle/{id}.json\n  method:\
  \ get\n  operationId: getTripForVehicle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vehicles-for-agency/{id}.json\n  method: get\n  operationId: listVehiclesForAgency\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /current-time.json\n  method: get\n  operationId: getCurrentTime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /config.json\n  method: get\n  operationId: getConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shape/{id}.json\n  method: get\n  operationId: getShape\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sound-transit/refs/heads/main/agentic-access/sound-transit-agentic-access.yml
summary_line: 20 operations
tags:
- Transit
- Transportation
- GTFS
- Real-Time
- Public Transit
- Government
- Seattle
---
