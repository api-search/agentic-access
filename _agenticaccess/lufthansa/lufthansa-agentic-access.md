---
acting_count: 0
action_class_counts:
  connected: 15
api_specs:
- filename: lufthansa-openapi.yml
  format: yaml
  label: Lufthansa Public API
  slug: public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lufthansa/refs/heads/main/openapi/lufthansa-openapi.yml
consequence_counts:
  read: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Lufthansa Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'Lufthansa exposes 15 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Lufthansa
provider_slug: lufthansa
slug: lufthansa-agentic-access
source_filename: lufthansa-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/lufthansa-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 15\n  by_consequence:\n    read: 15\n  human_in_the_loop_required: 0\noperations:\n- path: /references/countries/{countryCode}\n  method: get\n  operationId: ReferencesCountriesByCountryCodeGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /references/cities/{cityCode}\n  method: get\n  operationId: ReferencesCitiesByCityCodeGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /references/airports/{airportCode}\n  method: get\n  operationId: ReferencesAirportsByAirportCodeGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /references/airports/nearest/{latitude},{longitude}\n  method: get\n  operationId: ReferencesAirportsNearestByLatitudeAndLongitudeGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /references/airlines/{airlineCode}\n  method: get\n  operationId: ReferencesAirlinesByAirlineCodeGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /references/aircraft/{aircraftCode}\n  method: get\n  operationId: ReferencesAircraftByAircraftCodeGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /offers/seatmaps/{flightNumber}/{origin}/{destination}/{date}/{cabinClass}\n  method: get\n  operationId: OffersSeatmapsDestinationDateCabinClassByFlightNumberAndOriginGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /offers/lounges/{location}\n  method: get\n  operationId: OffersLoungesByLocationGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operations/flightstatus/{flightNumber}/{date}\n  method: get\n  operationId: OperationsFlightstatusByFlightNumberAndDateGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operations/flightstatus/route/{origin}/{destination}/{date}\n  method: get\n  operationId: OperationsFlightstatusRouteDateByOriginAndDestinationGet\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operations/flightstatus/arrivals/{airportCode}/{fromDateTime}\n  method: get\n  operationId: OperationsFlightstatusArrivalsByAirportCodeAndFromDateTimeGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operations/flightstatus/departures/{airportCode}/{fromDateTime}\n  method: get\n  operationId: OperationsFlightstatusDeparturesByAirportCodeAndFromDateTimeGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operations/schedules/{origin}/{destination}/{fromDateTime}\n  method: get\n  operationId: OperationsSchedulesFromDateTimeByOriginAndDestinationGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cargo/shipmentTracking/{aWBPrefix}-{aWBNumber}\n  method: get\n  operationId: CargoShipmentTrackingByAWBPrefixAndAWBNumberGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cargo/getRoute/{origin}-{destination}/{fromDate}/{productCode}\n  method: get\n  operationId: CargoGetRouteFromDateProductCodeByOriginAndDestinationGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lufthansa/refs/heads/main/agentic-access/lufthansa-agentic-access.yml
summary_line: 15 operations
tags:
- Airlines
- Travel
- Aviation
- Flights
---
