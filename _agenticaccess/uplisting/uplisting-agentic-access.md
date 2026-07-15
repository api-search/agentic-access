---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 11
api_specs:
- filename: uplisting-openapi.yml
  format: yaml
  label: Uplisting Bookings API
  slug: uplisting-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uplisting/refs/heads/main/openapi/uplisting-openapi.yml
- filename: uplisting-openapi.yml
  format: yaml
  label: Uplisting Properties API
  slug: uplisting-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uplisting/refs/heads/main/openapi/uplisting-openapi.yml
- filename: uplisting-openapi.yml
  format: yaml
  label: Uplisting Availability API
  slug: uplisting-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uplisting/refs/heads/main/openapi/uplisting-openapi.yml
- filename: uplisting-openapi.yml
  format: yaml
  label: Uplisting Calendar API
  slug: uplisting-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uplisting/refs/heads/main/openapi/uplisting-openapi.yml
- filename: uplisting-openapi.yml
  format: yaml
  label: Uplisting Rates API
  slug: uplisting-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uplisting/refs/heads/main/openapi/uplisting-openapi.yml
- filename: uplisting-openapi.yml
  format: yaml
  label: Uplisting Guests API
  slug: uplisting-guests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uplisting/refs/heads/main/openapi/uplisting-openapi.yml
- filename: uplisting-openapi.yml
  format: yaml
  label: Uplisting Messages API
  slug: uplisting-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uplisting/refs/heads/main/openapi/uplisting-openapi.yml
- filename: uplisting-openapi.yml
  format: yaml
  label: Uplisting Webhooks API
  slug: uplisting-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uplisting/refs/heads/main/openapi/uplisting-openapi.yml
consequence_counts:
  physical: 1
  read: 11
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Uplisting Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /bookings/{bookingId}/messages
operation_count: 18
overview: 'Uplisting exposes 18 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 6 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Uplisting
provider_slug: uplisting
slug: uplisting-agentic-access
source_filename: uplisting-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/uplisting-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    connected: 11\n    acting: 7\n  by_consequence:\n    read: 11\n    write: 6\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /users/me\n  method: get\n  operationId: getCurrentUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /properties\n  method: get\n  operationId: listProperties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /properties/{propertyId}\n\
  \  method: get\n  operationId: getProperty\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bookings\n  method: get\n  operationId: listBookings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bookings\n  method: post\n  operationId: createBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bookings/{bookingId}\n  method: get\n  operationId: getBooking\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bookings/{bookingId}\n  method:\
  \ patch\n  operationId: updateBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /availability\n  method: get\n  operationId: listAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /properties/{propertyId}/calendar\n  method: get\n  operationId: getCalendar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /properties/{propertyId}/calendar\n  method: put\n  operationId: updateCalendar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /properties/{propertyId}/rates\n  method: put\n  operationId: updateRates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /guests\n  method: get\n  operationId: listGuests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /guests/{guestId}\n  method: get\n  operationId: getGuest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bookings/{bookingId}/messages\n  method: get\n  operationId: listMessages\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bookings/{bookingId}/messages\n  method: post\n  operationId: sendMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{webhookId}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uplisting/refs/heads/main/agentic-access/uplisting-agentic-access.yml
summary_line: 18 operations · 7 acting
tags:
- Vacation Rental
- Short-Term Rental
- Channel Manager
- Property Management
- Bookings
- Hospitality
---
