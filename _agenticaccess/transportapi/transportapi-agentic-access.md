---
acting_count: 0
action_class_counts:
  connected: 7
api_specs:
- filename: transportapi-openapi.yml
  format: yaml
  label: TransportAPI
  slug: transportapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transportapi/refs/heads/main/openapi/transportapi-openapi.yml
consequence_counts:
  read: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Transportapi Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'TransportAPI exposes 7 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: TransportAPI
provider_slug: transportapi
slug: transportapi-agentic-access
source_filename: transportapi-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/transportapi-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 7\n  by_consequence:\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /bus/stop/{atcocode}/live.json\n  method: get\n  operationId: getBusStopLiveDepartures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bus/stop/{atcocode}/timetable.json\n  method: get\n  operationId: getBusStopTimetable\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bus/route/{operator}/{line}/{direction}/{atcocode}/{date}/timetable.json\n\
  \  method: get\n  operationId: getBusRouteTimetable\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /train/station/{station_code}/live.json\n  method: get\n  operationId: getTrainStationLiveDepartures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /train/station/{station_code}/{date}/{time}/timetable.json\n  method: get\n  operationId: getTrainStationTimetable\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /places.json\n  method: get\n  operationId: searchPlaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /journey/from/{from_coords}/to/{to_coords}.json\n  method:\
  \ get\n  operationId: planJourney\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transportapi/refs/heads/main/agentic-access/transportapi-agentic-access.yml
summary_line: 7 operations
tags:
- Public Transit
- Transport
- UK
- Real-Time
- Journey Planning
- Bus
- Rail
---
