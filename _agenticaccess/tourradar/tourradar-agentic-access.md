---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 19
api_specs:
- filename: tourradar-bookings-api-openapi.yml
  format: yaml
  label: TourRadar Bookings API
  slug: tourradar-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tourradar/refs/heads/main/openapi/tourradar-bookings-api-openapi.yml
- filename: tourradar-bulk-api-openapi.yml
  format: yaml
  label: TourRadar Bulk API
  slug: tourradar-bulk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tourradar/refs/heads/main/openapi/tourradar-bulk-api-openapi.yml
- filename: tourradar-operators-api-openapi.yml
  format: yaml
  label: TourRadar Operators API
  slug: tourradar-operators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tourradar/refs/heads/main/openapi/tourradar-operators-api-openapi.yml
- filename: tourradar-pricing-availability-api-openapi.yml
  format: yaml
  label: TourRadar Pricing & Availability API
  slug: tourradar-pricing-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tourradar/refs/heads/main/openapi/tourradar-pricing-availability-api-openapi.yml
- filename: tourradar-taxonomy-api-openapi.yml
  format: yaml
  label: TourRadar Taxonomy API
  slug: tourradar-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tourradar/refs/heads/main/openapi/tourradar-taxonomy-api-openapi.yml
- filename: tourradar-tours-api-openapi.yml
  format: yaml
  label: TourRadar Tours API
  slug: tourradar-tours-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tourradar/refs/heads/main/openapi/tourradar-tours-api-openapi.yml
consequence_counts:
  read: 19
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tourradar Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 21
overview: 'TourRadar exposes 21 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: TourRadar
provider_slug: tourradar
slug: tourradar-agentic-access
source_filename: tourradar-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: generated\nsource: openapi/tourradar-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    connected: 19\n    acting: 2\n  by_consequence:\n    read: 19\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/bookings\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - com.tourradar.bookings/read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/bookings\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - com.tourradar.bookings/write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/bookings/affiliate\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - com.tourradar.bookings.affiliate/read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/bookings/operator/{operator}/{bookingCode}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - com.tourradar.bookings/read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/bookings/{bookingId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - com.tourradar.bookings/read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/bookings/{bookingId}/status\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    scope:\n    - com.tourradar.bookings/read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/operators\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - com.tourradar.operators/read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/operators/{operator}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - com.tourradar.operators/read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/operators/{operator}/booking-fields\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - com.tourradar.operators/read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/operators/{operator}/bulk/departures\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    scope:\n    - com.tourradar.operators/read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/operators/{operator}/bulk/tours\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - com.tourradar.operators/read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/taxonomy/currencies\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/taxonomy/destinations/{type}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/taxonomy/languages\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/taxonomy/tours/types\n  method: get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tours/search\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - com.tourradar.tours/read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tours/{tourId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - com.tourradar.tours/read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tours/{tourId}/departures\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - com.tourradar.tours/read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tours/{tourId}/departures/{departureId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n   \
  \ subject: optional\n    scope:\n    - com.tourradar.tours/read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tours/{tourId}/departures/{departureId}/price\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - com.tourradar.tours/read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tours/{tourId}/prices\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - com.tourradar.tours/read\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tourradar/refs/heads/main/agentic-access/tourradar-agentic-access.yml
summary_line: 21 operations · 2 acting
tags:
- Travel
- Tours
- Booking
- Marketplace
- Adventure Travel
- Distribution
- Affiliates
---
