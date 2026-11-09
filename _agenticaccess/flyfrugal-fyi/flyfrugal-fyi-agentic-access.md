---
acting_count: 0
action_class_counts:
  connected: 14
api_specs:
- filename: flyfrugal-fyi-calendar-api-openapi.yml
  format: yaml
  label: Fly Frugal Calendar API
  slug: flyfrugal-fyi-calendar-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flyfrugal-fyi/openapi/flyfrugal-fyi-calendar-api-openapi.yml
- filename: flyfrugal-fyi-catalog-api-openapi.yml
  format: yaml
  label: Fly Frugal Catalog API
  slug: flyfrugal-fyi-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flyfrugal-fyi/openapi/flyfrugal-fyi-catalog-api-openapi.yml
- filename: flyfrugal-fyi-deals-api-openapi.yml
  format: yaml
  label: Fly Frugal Deals API
  slug: flyfrugal-fyi-deals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flyfrugal-fyi/openapi/flyfrugal-fyi-deals-api-openapi.yml
- filename: flyfrugal-fyi-history-api-openapi.yml
  format: yaml
  label: Fly Frugal History API
  slug: flyfrugal-fyi-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flyfrugal-fyi/openapi/flyfrugal-fyi-history-api-openapi.yml
- filename: flyfrugal-fyi-itineraries-api-openapi.yml
  format: yaml
  label: Fly Frugal Itineraries API
  slug: flyfrugal-fyi-itineraries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flyfrugal-fyi/openapi/flyfrugal-fyi-itineraries-api-openapi.yml
- filename: flyfrugal-fyi-weather-api-openapi.yml
  format: yaml
  label: Fly Frugal Weather API
  slug: flyfrugal-fyi-weather-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flyfrugal-fyi/openapi/flyfrugal-fyi-weather-api-openapi.yml
consequence_counts:
  read: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Flyfrugal Fyi Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'Fly Frugal exposes 14 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Fly Frugal
provider_slug: flyfrugal-fyi
slug: flyfrugal-fyi-agentic-access
source_filename: flyfrugal-fyi-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: generated\nsource: openapi/flyfrugal-fyi-openapi.yaml, openapi/openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 14\n  by_consequence:\n    read: 14\n  human_in_the_loop_required: 0\noperations:\n- path: /api/itineraries\n  method: get\n  operationId: listItineraries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/itineraries/{slug}\n  method: get\n  operationId: getItinerary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/deals\n  method:\
  \ get\n  operationId: listFlightDeals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/calendar\n  method: get\n  operationId: getRouteCalendar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/history\n  method: get\n  operationId: getFareHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/catalog\n  method: get\n  operationId: getAirportCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/weather\n  method: get\n  operationId: getTypicalWeather\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/itineraries\n  method: get\n  operationId: listItineraries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/itineraries/{slug}\n  method: get\n  operationId: getItinerary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/deals\n  method: get\n  operationId: listFlightDeals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/calendar\n  method: get\n  operationId: getRouteCalendar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/history\n  method: get\n  operationId: getFareHistory\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/catalog\n  method: get\n  operationId: getAirportCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/weather\n  method: get\n  operationId: getTypicalWeather\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/flyfrugal-fyi/agentic-access/flyfrugal-fyi-agentic-access.yml
summary_line: 14 operations
tags:
- Travel
- Data
- API
- MCP
- Flight Deals
- Company
---
