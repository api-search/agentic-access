---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 5
api_specs:
- filename: bergsonne-allgaeu-de-availability-api-openapi.yml
  format: yaml
  label: Hotel Bergsonne Allgäu Availability API
  slug: bergsonne-allgaeu-de-availability-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bergsonne-allgaeu-de/openapi/bergsonne-allgaeu-de-availability-api-openapi.yml
- filename: bergsonne-allgaeu-de-bookings-api-openapi.yml
  format: yaml
  label: Hotel Bergsonne Allgäu Bookings API
  slug: bergsonne-allgaeu-de-bookings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bergsonne-allgaeu-de/openapi/bergsonne-allgaeu-de-bookings-api-openapi.yml
- filename: bergsonne-allgaeu-de-fact-sheet-api-openapi.yml
  format: yaml
  label: Hotel Bergsonne Allgäu Fact Sheet API
  slug: bergsonne-allgaeu-de-fact-sheet-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bergsonne-allgaeu-de/openapi/bergsonne-allgaeu-de-fact-sheet-api-openapi.yml
- filename: bergsonne-allgaeu-de-hotel-api-openapi.yml
  format: yaml
  label: Hotel Bergsonne Allgäu Hotel API
  slug: bergsonne-allgaeu-de-hotel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bergsonne-allgaeu-de/openapi/bergsonne-allgaeu-de-hotel-api-openapi.yml
- filename: bergsonne-allgaeu-de-hotel-bergsonne-allg-u-booking-api-api-openapi.yml
  format: yaml
  label: Hotel Bergsonne Allgäu Hotel Bergsonne Allgäu Booking API
  slug: bergsonne-allgaeu-de-hotel-bergsonne-allg-u-booking-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bergsonne-allgaeu-de/openapi/bergsonne-allgaeu-de-hotel-bergsonne-allg-u-booking-api-api-openapi.yml
- filename: bergsonne-allgaeu-de-price-quote-api-openapi.yml
  format: yaml
  label: Hotel Bergsonne Allgäu Price Quote API
  slug: bergsonne-allgaeu-de-price-quote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bergsonne-allgaeu-de/openapi/bergsonne-allgaeu-de-price-quote-api-openapi.yml
consequence_counts:
  read: 5
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bergsonne Allgaeu De Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Hotel Bergsonne Allgäu exposes 6 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Hotel Bergsonne Allgäu
provider_slug: bergsonne-allgaeu-de
slug: bergsonne-allgaeu-de-agentic-access
source_filename: bergsonne-allgaeu-de-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/bergsonne-allgaeu-de-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 5\n    acting: 1\n  by_consequence:\n    read: 5\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: routeByAction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - booking:read\n    - hotel:read\n- path: /hotel\n  method: get\n  operationId: getHotelDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  \    scope:\n    - booking:read\n    - hotel:read\n- path: /availability\n  method: get\n  operationId: searchAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - booking:read\n    - hotel:read\n- path: /price-quote\n  method: get\n  operationId: getPriceQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - booking:read\n    - hotel:read\n- path: /fact-sheet\n  method: get\n  operationId: getFactSheet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - booking:read\n    - hotel:read\n- path: /bookings\n  method: post\n  operationId: createBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    scope:\n    - booking:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/bergsonne-allgaeu-de/agentic-access/bergsonne-allgaeu-de-agentic-access.yml
summary_line: 6 operations · 1 acting
tags:
- Hotels
- Hospitality
- Travel
- Germany
- Allgäu
- Retreat
---
