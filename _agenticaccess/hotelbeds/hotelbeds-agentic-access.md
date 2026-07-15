---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 8
api_specs:
- filename: hotelbeds-openapi.yml
  format: yaml
  label: Hotel Booking API
  slug: hotel-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotelbeds/refs/heads/main/openapi/hotelbeds-openapi.yml
- filename: hotelbeds-openapi.yml
  format: yaml
  label: Hotel Content API
  slug: hotel-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotelbeds/refs/heads/main/openapi/hotelbeds-openapi.yml
- filename: hotelbeds-openapi.yml
  format: yaml
  label: Cache Rates API
  slug: cache-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotelbeds/refs/heads/main/openapi/hotelbeds-openapi.yml
- filename: hotelbeds-openapi.yml
  format: yaml
  label: Activities API
  slug: activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotelbeds/refs/heads/main/openapi/hotelbeds-openapi.yml
- filename: hotelbeds-openapi.yml
  format: yaml
  label: Transfers API
  slug: transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotelbeds/refs/heads/main/openapi/hotelbeds-openapi.yml
- filename: hotelbeds-openapi.yml
  format: yaml
  label: Webhooks
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotelbeds/refs/heads/main/openapi/hotelbeds-openapi.yml
consequence_counts:
  read: 8
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Hotelbeds Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'Hotelbeds exposes 13 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Hotelbeds
provider_slug: hotelbeds
slug: hotelbeds-agentic-access
source_filename: hotelbeds-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/hotelbeds-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 8\n    acting: 5\n  by_consequence:\n    read: 8\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /hotel-api/1.0/status\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hotel-api/1.0/hotels\n  method: post\n  operationId: getAvailability\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hotel-api/1.0/checkrates\n  method: post\n  operationId: checkRates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hotel-api/1.0/bookings\n  method: get\n  operationId: listBookings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hotel-api/1.0/bookings\n  method: post\n  operationId: confirmBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /hotel-api/1.0/bookings/{bookingId}\n  method: get\n  operationId: getBookingDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hotel-api/1.0/bookings/{bookingId}\n  method: delete\n  operationId: cancelBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hotel-content-api/1.0/hotels\n  method: get\n  operationId: getHotelContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hotel-content-api/1.0/locations/countries\n  method: get\n  operationId: getCountries\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hotel-content-api/1.0/locations/destinations\n  method: get\n  operationId: getDestinations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /activity-api/3.0/activities/availability\n  method: post\n  operationId: getActivityAvailability\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transfer-api/1.0/availability/{language}/from/{fromType}/{fromCode}/to/{toType}/{toCode}\n  method: get\n  operationId: getTransferAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /hotel-cache-api/1.0/availabilities\n  method: get\n  operationId: getCacheFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hotelbeds/refs/heads/main/agentic-access/hotelbeds-agentic-access.yml
summary_line: 13 operations · 5 acting
tags:
- Travel
- Hotels
- Bedbank
- Accommodation
- Booking
---
