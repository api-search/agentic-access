---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 7
api_specs:
- filename: flightpowers-com-account-api-openapi.yml
  format: yaml
  label: flightpowers-com Account API
  slug: flightpowers-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flightpowers-com/openapi/flightpowers-com-account-api-openapi.yml
- filename: flightpowers-com-flights-api-openapi.yml
  format: yaml
  label: flightpowers-com Flights API
  slug: flightpowers-com-flights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flightpowers-com/openapi/flightpowers-com-flights-api-openapi.yml
- filename: flightpowers-com-hotels-api-openapi.yml
  format: yaml
  label: flightpowers-com Hotels API
  slug: flightpowers-com-hotels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flightpowers-com/openapi/flightpowers-com-hotels-api-openapi.yml
- filename: flightpowers-com-verify-api-openapi.yml
  format: yaml
  label: flightpowers-com Verify API
  slug: flightpowers-com-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flightpowers-com/openapi/flightpowers-com-verify-api-openapi.yml
consequence_counts:
  read: 7
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Flightpowers Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'flightpowers-com exposes 14 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: flightpowers-com
provider_slug: flightpowers-com
slug: flightpowers-com-agentic-access
source_filename: flightpowers-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/flightpowers-com-api-openapi.json, openapi/flightpowers-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 7\n    acting: 7\n  by_consequence:\n    read: 7\n    write: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/verify\n  method: get\n  operationId: verify_v1_verify_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/flights/oneway\n  method: post\n  operationId: v1_flights_oneway_v1_flights_oneway_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/flights/roundtrip\n  method: post\n  operationId: v1_flights_roundtrip_v1_flights_roundtrip_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/hotels/search\n  method: post\n  operationId: v1_hotels_search_v1_hotels_search_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/hotels/by-name\n  method: post\n  operationId: v1_hotels_by_name_v1_hotels_by_name_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/hotels/rooms\n  method: post\n  operationId: v1_hotels_rooms_v1_hotels_rooms_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/hotels/resolve\n  method: post\n  operationId: v1_hotels_resolve_v1_hotels_resolve_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/verify\n  method: get\n  operationId: verifyKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/flights/oneway\n  method: post\n  operationId: searchOnewayFlights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/flights/roundtrip\n  method: post\n  operationId: searchRoundtripFlights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/hotels/search\n  method: post\n  operationId: searchHotels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/hotels/by-name\n  method: post\n  operationId: findHotelByName\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/hotels/rooms\n  method: post\n  operationId: getHotelRooms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/hotels/resolve\n  method: post\n  operationId: resolveHotelId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/flightpowers-com/agentic-access/flightpowers-com-agentic-access.yml
summary_line: 14 operations · 7 acting
tags:
- Company
- Travel
- Data
- Flights
- Hotels
---
