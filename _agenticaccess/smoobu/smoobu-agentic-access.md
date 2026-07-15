---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 11
api_specs:
- filename: smoobu-openapi.yml
  format: yaml
  label: Smoobu Reservations API
  slug: smoobu-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smoobu/refs/heads/main/openapi/smoobu-openapi.yml
- filename: smoobu-openapi.yml
  format: yaml
  label: Smoobu Apartments API
  slug: smoobu-apartments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smoobu/refs/heads/main/openapi/smoobu-openapi.yml
- filename: smoobu-openapi.yml
  format: yaml
  label: Smoobu Rates and Availability API
  slug: smoobu-rates-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smoobu/refs/heads/main/openapi/smoobu-openapi.yml
- filename: smoobu-openapi.yml
  format: yaml
  label: Smoobu Guests API
  slug: smoobu-guests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smoobu/refs/heads/main/openapi/smoobu-openapi.yml
- filename: smoobu-openapi.yml
  format: yaml
  label: Smoobu Messaging API
  slug: smoobu-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smoobu/refs/heads/main/openapi/smoobu-openapi.yml
- filename: smoobu-openapi.yml
  format: yaml
  label: Smoobu Webhooks
  slug: smoobu-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smoobu/refs/heads/main/openapi/smoobu-openapi.yml
consequence_counts:
  physical: 2
  read: 11
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Smoobu Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/reservations/{reservationId}/messages/send-message-to-guest
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/reservations/{reservationId}/messages/send-message-to-host
operation_count: 19
overview: 'Smoobu exposes 19 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 6 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Smoobu
provider_slug: smoobu
slug: smoobu-agentic-access
source_filename: smoobu-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/smoobu-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    connected: 11\n    acting: 8\n  by_consequence:\n    read: 11\n    write: 6\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/me\n  method: get\n  operationId: getMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/apartments\n  method: get\n  operationId: listApartments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/apartments/{apartmentId}\n\
  \  method: get\n  operationId: getApartment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/reservations\n  method: get\n  operationId: listReservations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/reservations\n  method: post\n  operationId: createReservation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/reservations/{reservationId}\n  method: get\n  operationId: getReservation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/reservations/{reservationId}\n  method: put\n  operationId: updateReservation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/reservations/{reservationId}\n  method: delete\n  operationId: deleteReservation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/reservations/{reservationId}/price-elements\n  method: get\n  operationId: listPriceElements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/reservations/{reservationId}/price-elements\n  method: post\n  operationId: createPriceElement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/rates\n  method: get\n  operationId: getRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rates\n  method: post\n  operationId: updateRates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /booking/checkApartmentAvailability\n  method: post\n  operationId:\
  \ checkApartmentAvailability\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/guests\n  method: get\n  operationId: listGuests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/guests/{guestId}\n  method: get\n  operationId: getGuest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/reservations/{reservationId}/messages\n  method: get\n  operationId: listReservationMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/reservations/{reservationId}/messages/send-message-to-guest\n\
  \  method: post\n  operationId: sendMessageToGuest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/reservations/{reservationId}/messages/send-message-to-host\n  method: post\n  operationId: sendMessageToHost\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/threads\n  method: get\n  operationId: listThreads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smoobu/refs/heads/main/agentic-access/smoobu-agentic-access.yml
summary_line: 19 operations · 8 acting
tags:
- Vacation Rental
- Channel Manager
- Property Management
- Short-Term Rental
- Reservations
- Hospitality
---
