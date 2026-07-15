---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 12
api_specs:
- filename: launch27-openapi.yml
  format: yaml
  label: Launch27 Authentication API
  slug: launch27-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/launch27/refs/heads/main/openapi/launch27-openapi.yml
- filename: launch27-openapi.yml
  format: yaml
  label: Launch27 Account Settings API
  slug: launch27-account-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/launch27/refs/heads/main/openapi/launch27-openapi.yml
- filename: launch27-openapi.yml
  format: yaml
  label: Launch27 Booking Helpers API
  slug: launch27-booking-helpers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/launch27/refs/heads/main/openapi/launch27-openapi.yml
- filename: launch27-openapi.yml
  format: yaml
  label: Launch27 Booking Policies API
  slug: launch27-booking-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/launch27/refs/heads/main/openapi/launch27-openapi.yml
- filename: launch27-openapi.yml
  format: yaml
  label: Launch27 Guest Booking API
  slug: launch27-guest-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/launch27/refs/heads/main/openapi/launch27-openapi.yml
- filename: launch27-openapi.yml
  format: yaml
  label: Launch27 Customer Bookings API
  slug: launch27-customer-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/launch27/refs/heads/main/openapi/launch27-openapi.yml
consequence_counts:
  read: 12
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Launch27 Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 21
overview: 'Launch27 exposes 21 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read and 9 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Launch27
provider_slug: launch27
slug: launch27-agentic-access
source_filename: launch27-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/launch27-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    acting: 9\n    connected: 12\n  by_consequence:\n    write: 9\n    read: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /login\n  method: post\n  operationId: login\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings\n  method: get\n  operationId: getSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /booking/form\n  method: get\n  operationId: getBookingForm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /booking/services\n  method: get\n  operationId: getBookingServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /booking/spots\n  method: post\n  operationId: getBookingSpots\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /booking/location\n  method: post\n  operationId: getBookingLocation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n \
  \   subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /booking/frequencies\n  method: get\n  operationId: getBookingFrequencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /booking/frequencies/{id}/next\n  method: post\n  operationId: getNextBookingDateForFrequency\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /booking/custom_fields\n  method: get\n  operationId: getBookingCustomFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /booking/estimate_price\n  method: post\n  operationId: estimateBookingPrice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /policy/booking\n  method: get\n  operationId: getNewBookingPolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /policy/reschedule\n  method: get\n  operationId: getRescheduleBookingPolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /policy/cancellation\n  method: get\n  operationId: getCancellationPolicy\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /policy/location\n  method: get\n  operationId: getLocationPolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /booking\n  method: post\n  operationId: createGuestBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer/bookings\n  method: get\n  operationId: listCustomerBookings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer/bookings\n  method: post\n  operationId: createCustomerBooking\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer/bookings/count\n  method: get\n  operationId: countCustomerBookings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer/bookings/{id}\n  method: get\n  operationId: getCustomerBooking\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer/bookings/{id}\n  method: put\n  operationId: updateCustomerBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /customer/bookings/{id}/cancel\n  method: post\n  operationId: cancelCustomerBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/launch27/refs/heads/main/agentic-access/launch27-agentic-access.yml
summary_line: 21 operations · 9 acting
tags:
- Field Service Management
- Home Services
- Cleaning Services
- Booking
- Scheduling
- Fullsteam
- Vonigo
---
