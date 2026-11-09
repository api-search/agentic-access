---
acting_count: 0
action_class_counts:
  connected: 7
api_specs:
- filename: ignav-com-airports-api-openapi.yml
  format: yaml
  label: ignav-com Airports API
  slug: ignav-com-airports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ignav-com/openapi/ignav-com-airports-api-openapi.yml
- filename: ignav-com-fares-api-openapi.yml
  format: yaml
  label: ignav-com Fares API
  slug: ignav-com-fares-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ignav-com/openapi/ignav-com-fares-api-openapi.yml
- filename: ignav-com-health-api-openapi.yml
  format: yaml
  label: ignav-com Health API
  slug: ignav-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ignav-com/openapi/ignav-com-health-api-openapi.yml
consequence_counts:
  read: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ignav Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'ignav-com exposes 7 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ignav-com
provider_slug: ignav-com
slug: ignav-com-agentic-access
source_filename: ignav-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/ignav-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 7\n  by_consequence:\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /api/health\n  method: get\n  operationId: health_api_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/airports\n  method: get\n  operationId: search_airports_api_airports_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/fares/search\n  method: post\n  operationId:\
  \ search_fares_api_fares_search_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/fares/one-way\n  method: post\n  operationId: search_one_way_api_fares_one_way_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/fares/round-trip\n  method: post\n  operationId: search_round_trip_api_fares_round_trip_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/fares/booking-links\n  method: post\n  operationId: get_booking_links_api_fares_booking_links_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/fares/cheapest-dates\n  method: post\n  operationId:\
  \ search_cheapest_dates_api_fares_cheapest_dates_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/ignav-com/agentic-access/ignav-com-agentic-access.yml
summary_line: 7 operations
tags:
- Company
- Flights
- Travel
- Pricing
- Data
---
