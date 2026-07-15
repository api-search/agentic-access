---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 38
api_specs:
- filename: aerodatabox-openapi.yml
  format: yaml
  label: AeroDataBox Flight API
  slug: aerodatabox-flight-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/openapi/aerodatabox-openapi.yml
- filename: aerodatabox-openapi.yml
  format: yaml
  label: AeroDataBox Aircraft API
  slug: aerodatabox-aircraft-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/openapi/aerodatabox-openapi.yml
- filename: aerodatabox-openapi.yml
  format: yaml
  label: AeroDataBox Airport API
  slug: aerodatabox-airport-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/openapi/aerodatabox-openapi.yml
- filename: aerodatabox-openapi.yml
  format: yaml
  label: AeroDataBox Statistical API
  slug: aerodatabox-statistical-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/openapi/aerodatabox-openapi.yml
- filename: aerodatabox-openapi.yml
  format: yaml
  label: AeroDataBox Flight Alert API
  slug: aerodatabox-flight-alert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/openapi/aerodatabox-openapi.yml
consequence_counts:
  read: 38
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Aerodatabox Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 42
overview: 'AeroDataBox exposes 42 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 38 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AeroDataBox
provider_slug: aerodatabox
slug: aerodatabox-agentic-access
source_filename: aerodatabox-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/aerodatabox-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 42\n  by_action_class:\n    connected: 38\n    acting: 4\n  by_consequence:\n    read: 38\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /aircrafts/{searchBy}/{searchParam}\n  method: get\n  operationId: GetAircraft\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /aircrafts/{searchBy}/{searchParam}/registrations\n  method: get\n  operationId: GetAircraftRegistrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /aircrafts/{searchBy}/{searchParam}/all\n  method: get\n  operationId: GetAllAircraft\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /airlines/{airlineCode}/aircrafts\n  method: get\n  operationId: GetAirlineFleet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /aircrafts/reg/{reg}/image/beta\n  method: get\n  operationId: GetAircraftImageByRegistration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /aircrafts/search/term\n  method: get\n  operationId: SearchAircraftByTerm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /airports/{codeType}/{code}\n\
  \  method: get\n  operationId: GetAirport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /airports/{codeType}/{code}/runways\n  method: get\n  operationId: GetAirportRunways\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /airports/search/location\n  method: get\n  operationId: SearchAirportsByLocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /airports/search/ip\n  method: get\n  operationId: SearchAirportsByIpGeoLocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /airports/search/term\n  method: get\n  operationId: SearchAirportByTerm\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions/webhook/{subjectType}/{subjectId}\n  method: post\n  operationId: SubscribeWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/webhook/{subscriptionId}\n  method: get\n  operationId: GetWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions/webhook/{subscriptionId}\n  method: delete\n  operationId: UnsubscribeWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/webhook\n  method: get\n  operationId: GetWebhookList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions/webhook/{subscriptionId}/refresh\n  method: patch\n  operationId: RefreshWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/balance\n  method: get\n  operationId: GetBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions/balance/refill\n  method: post\n  operationId:\
  \ RefillBalance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /flights/{searchBy}/{searchParam}\n  method: get\n  operationId: GetFlight_FlightNearest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /flights/{searchBy}/{searchParam}/{dateLocal}\n  method: get\n  operationId: GetFlight_FlightOnSpecificDate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /flights/{searchBy}/{searchParam}/{dateFromLocal}/{dateToLocal}\n  method: get\n  operationId: GetFlightHistory_FlightHistory\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /flights/{searchBy}/{searchParam}/dates\n  method: get\n  operationId: GetFlightDates_FlightDatesAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /flights/{searchBy}/{searchParam}/dates/{fromLocal}/{toLocal}\n  method: get\n  operationId: GetFlightDates_FlightDatesInRange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /flights/airports/{codeType}/{code}/{fromLocal}/{toLocal}\n  method: get\n  operationId: GetAirportFlights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /flights/airports/{codeType}/{code}\n  method: get\n  operationId: GetAirportFlightsRelative\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /flights/search/term\n  method: get\n  operationId: SearchFlightsByTerm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health/services/feeds/{service}\n  method: get\n  operationId: GetFeedServiceStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health/services/airports/{icao}/feeds\n  method: get\n  operationId: GetAirportFeedStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health/services/feeds/{service}/airports\n  method: get\n  operationId: GetFeedAirports\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /industry/faa-ladd/{id}/status\n  method: get\n  operationId: GetFaaLaddAircraftStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /airports/{codeType}/{code}/time/local\n  method: get\n  operationId: GetAirportLocalTime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /airports/{codeType}/{code}/time/solar\n  method: get\n  operationId: GetAirportSolarTime_SolarTimeCurrent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /airports/{codeType}/{code}/time/solar/{dateLocal}\n  method: get\n  operationId: GetAirportSolarTime_SolarTimeSpecificDate\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /airports/{codeType}/{codeFrom}/distance-time/{codeTo}\n  method: get\n  operationId: GetAirportDistanceTime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /airports/{codeType}/{code}/delays\n  method: get\n  operationId: GetAirportDelay_DelaysCurrent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /airports/{codeType}/{code}/delays/{dateLocal}\n  method: get\n  operationId: GetAirportDelay_DelaysHistorical\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /airports/{codeType}/{code}/delays/{dateFromLocal}/{dateToLocal}\n  method: get\n  operationId: GetAirportDelays\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /airports/{codeType}/{code}/stats/routes/daily\n  method: get\n  operationId: GetRouteDailyStatistics_RoutesDailyCurrent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /airports/{codeType}/{code}/stats/routes/daily/{dateLocal}\n  method: get\n  operationId: GetRouteDailyStatistics_RoutesDailAtSpecificDate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /airports/delays\n  method: get\n  operationId: GetGlobalDelays_GlobalDelaysCurent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /airports/delays/{dateUtc}\n  method:\
  \ get\n  operationId: GetGlobalDelays_GlobalDelaysAtSpecificDate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /flights/{number}/delays\n  method: get\n  operationId: GetFlightDelays\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/agentic-access/aerodatabox-agentic-access.yml
summary_line: 42 operations · 4 acting
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
---
