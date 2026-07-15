---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 13
api_specs:
- filename: beds24-openapi.yml
  format: yaml
  label: Beds24 Authentication API
  slug: beds24-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beds24/refs/heads/main/openapi/beds24-openapi.yml
- filename: beds24-openapi.yml
  format: yaml
  label: Beds24 Bookings API
  slug: beds24-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beds24/refs/heads/main/openapi/beds24-openapi.yml
- filename: beds24-openapi.yml
  format: yaml
  label: Beds24 Invoices & Charges API
  slug: beds24-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beds24/refs/heads/main/openapi/beds24-openapi.yml
- filename: beds24-openapi.yml
  format: yaml
  label: Beds24 Booking Messages API
  slug: beds24-booking-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beds24/refs/heads/main/openapi/beds24-openapi.yml
- filename: beds24-openapi.yml
  format: yaml
  label: Beds24 Properties API
  slug: beds24-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beds24/refs/heads/main/openapi/beds24-openapi.yml
- filename: beds24-openapi.yml
  format: yaml
  label: Beds24 Availability & Calendar API
  slug: beds24-availability-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beds24/refs/heads/main/openapi/beds24-openapi.yml
- filename: beds24-openapi.yml
  format: yaml
  label: Beds24 Rates & Prices API
  slug: beds24-rates-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beds24/refs/heads/main/openapi/beds24-openapi.yml
- filename: beds24-openapi.yml
  format: yaml
  label: Beds24 Channels API
  slug: beds24-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beds24/refs/heads/main/openapi/beds24-openapi.yml
- filename: beds24-openapi.yml
  format: yaml
  label: Beds24 Accounts API
  slug: beds24-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beds24/refs/heads/main/openapi/beds24-openapi.yml
consequence_counts:
  physical: 1
  read: 13
  safety-critical: 1
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Beds24 Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /authentication/token
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /bookings/invoiceitems
operation_count: 23
overview: 'Beds24 exposes 23 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read, 8 write, 1 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Beds24
provider_slug: beds24
slug: beds24-agentic-access
source_filename: beds24-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/beds24-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 13\n    acting: 10\n  by_consequence:\n    read: 13\n    safety-critical: 1\n    write: 8\n    physical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /authentication/setup\n  method: get\n  operationId: getSetup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authentication/token\n  method: get\n  operationId: getToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /authentication/token\n  method: delete\n  operationId: deleteToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /authentication/details\n  method: get\n  operationId: getAuthenticationDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bookings\n  method: get\n  operationId: getBookings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bookings\n  method: post\n  operationId: postBookings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bookings/messages\n  method: get\n  operationId: getBookingMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bookings/messages\n  method: post\n  operationId: postBookingMessages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bookings/invoiceitems\n  method: get\n  operationId: getInvoiceItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bookings/invoiceitems\n\
  \  method: post\n  operationId: postInvoiceItems\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /properties\n  method: get\n  operationId: getProperties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /properties\n  method: post\n  operationId: postProperties\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /properties/offers\n  method: get\n  operationId: getPropertyOffers\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inventory/rooms/calendar\n  method: get\n  operationId: getRoomCalendar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inventory/rooms/calendar\n  method: post\n  operationId: postRoomCalendar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inventory/rooms/availability\n  method: get\n  operationId: getRoomAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inventory/rooms/availability\n\
  \  method: post\n  operationId: postRoomAvailability\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inventory/fixedPrices\n  method: get\n  operationId: getFixedPrices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inventory/fixedPrices\n  method: post\n  operationId: postFixedPrices\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inventory/fixedPrices\n  method: delete\n  operationId: deleteFixedPrices\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /channels\n  method: get\n  operationId: getChannels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /channels\n  method: post\n  operationId: postChannels\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts\n  method: get\n  operationId: getAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beds24/refs/heads/main/agentic-access/beds24-agentic-access.yml
summary_line: 23 operations · 10 acting · 1 human-in-the-loop
tags:
- Vacation Rental
- Hotel
- Channel Manager
- Property Management System
- Booking Engine
- Hospitality
- Reservations
---
