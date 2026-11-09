---
acting_count: 0
action_class_counts:
  connected: 14
api_specs:
- filename: adsbiq-com-aircraft-api-openapi.yml
  format: yaml
  label: adsbiq-com Aircraft API
  slug: adsbiq-com-aircraft-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adsbiq-com/openapi/adsbiq-com-aircraft-api-openapi.yml
- filename: adsbiq-com-airports-api-openapi.yml
  format: yaml
  label: adsbiq-com Airports API
  slug: adsbiq-com-airports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adsbiq-com/openapi/adsbiq-com-airports-api-openapi.yml
- filename: adsbiq-com-flights-api-openapi.yml
  format: yaml
  label: adsbiq-com Flights API
  slug: adsbiq-com-flights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adsbiq-com/openapi/adsbiq-com-flights-api-openapi.yml
- filename: adsbiq-com-geographic-api-openapi.yml
  format: yaml
  label: adsbiq-com Geographic API
  slug: adsbiq-com-geographic-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adsbiq-com/openapi/adsbiq-com-geographic-api-openapi.yml
- filename: adsbiq-com-network-api-openapi.yml
  format: yaml
  label: adsbiq-com Network API
  slug: adsbiq-com-network-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adsbiq-com/openapi/adsbiq-com-network-api-openapi.yml
consequence_counts:
  read: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Adsbiq Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'adsbiq-com exposes 14 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: adsbiq-com
provider_slug: adsbiq-com
slug: adsbiq-com-agentic-access
source_filename: adsbiq-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/adsbiq-com-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 14\n  by_consequence:\n    read: 14\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/all\n  method: get\n  operationId: getAllAircraft\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/hex/{hex}\n  method: get\n  operationId: getAircraftByHex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/reg/{registration}\n  method: get\n  operationId: getAircraftByRegistration\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/type/{type}\n  method: get\n  operationId: getAircraftByType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/callsign/{callsign}\n  method: get\n  operationId: getAircraftByCallsign\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/squawk/{code}\n  method: get\n  operationId: getAircraftBySquawk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/flight/{identifier}\n  method: get\n  operationId: getFlight\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v2/airport/{code}\n  method: get\n  operationId: getAirportActivity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/airport/{code}/arrivals\n  method: get\n  operationId: getAirportArrivals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/airport/{code}/departures\n  method: get\n  operationId: getAirportDepartures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/route/{origin}/{destination}\n  method: get\n  operationId: getRouteActivity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/airports/nearby\n \
  \ method: get\n  operationId: getNearbyAirports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/lat/{latitude}/lon/{longitude}/dist/{distance}\n  method: get\n  operationId: getAircraftNearby\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/stats\n  method: get\n  operationId: getNetworkStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/adsbiq-com/agentic-access/adsbiq-com-agentic-access.yml
summary_line: 14 operations
tags:
- Advertising
- Data Analytics
- Marketing Technology
- Company
---
