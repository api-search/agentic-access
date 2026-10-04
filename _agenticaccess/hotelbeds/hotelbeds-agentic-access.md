---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 10
api_specs:
- filename: hotelbeds-activities-api-openapi.yml
  format: yaml
  label: Hotelbeds Activities API
  slug: hotelbeds-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotelbeds/refs/heads/main/openapi/hotelbeds-activities-api-openapi.yml
- filename: hotelbeds-booking-api-openapi.yml
  format: yaml
  label: Hotelbeds Booking API
  slug: hotelbeds-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotelbeds/refs/heads/main/openapi/hotelbeds-booking-api-openapi.yml
- filename: hotelbeds-cache-api-openapi.yml
  format: yaml
  label: Hotelbeds Cache API
  slug: hotelbeds-cache-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotelbeds/refs/heads/main/openapi/hotelbeds-cache-api-openapi.yml
- filename: hotelbeds-content-api-openapi.yml
  format: yaml
  label: Hotelbeds Content API
  slug: hotelbeds-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotelbeds/refs/heads/main/openapi/hotelbeds-content-api-openapi.yml
- filename: hotelbeds-transfers-api-openapi.yml
  format: yaml
  label: Hotelbeds Transfers API
  slug: hotelbeds-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotelbeds/refs/heads/main/openapi/hotelbeds-transfers-api-openapi.yml
consequence_counts:
  read: 10
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Hotelbeds Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'Hotelbeds exposes 13 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Hotelbeds
provider_slug: hotelbeds
slug: hotelbeds-agentic-access
source_filename: hotelbeds-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/hotelbeds-activities-api-openapi.yml, openapi/hotelbeds-booking-api-openapi.yml,\n  openapi/hotelbeds-cache-api-openapi.yml, openapi/hotelbeds-content-api-openapi.yml, openapi/hotelbeds-transfers-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 10\n    acting: 3\n  by_consequence:\n    read: 10\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /activity-api/3.0/activities/availability\n  method: post\n  operationId: getActivityAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hotel-api/1.0/status\n\
  \  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hotel-api/1.0/hotels\n  method: post\n  operationId: getAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hotel-api/1.0/checkrates\n  method: post\n  operationId: checkRates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hotel-api/1.0/bookings\n  method: get\n  operationId: listBookings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hotel-api/1.0/bookings\n\
  \  method: post\n  operationId: confirmBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hotel-api/1.0/bookings/{bookingId}\n  method: get\n  operationId: getBookingDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hotel-api/1.0/bookings/{bookingId}\n  method: delete\n  operationId: cancelBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hotel-cache-api/1.0/availabilities\n  method: get\n  operationId:\
  \ getCacheFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hotel-content-api/1.0/hotels\n  method: get\n  operationId: getHotelContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hotel-content-api/1.0/locations/countries\n  method: get\n  operationId: getCountries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hotel-content-api/1.0/locations/destinations\n  method: get\n  operationId: getDestinations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transfer-api/1.0/availability/{language}/from/{fromType}/{fromCode}/to/{toType}/{toCode}\n  method: get\n\
  \  operationId: getTransferAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hotelbeds/refs/heads/main/agentic-access/hotelbeds-agentic-access.yml
summary_line: 13 operations · 3 acting
tags:
- Travel
- Hotels
- Bedbank
- Accommodation
- Booking
---
