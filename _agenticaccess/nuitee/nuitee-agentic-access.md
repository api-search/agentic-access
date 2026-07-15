---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 13
api_specs:
- filename: nuitee-openapi.yml
  format: yaml
  label: LiteAPI Hotel Data API
  slug: hotel-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuitee/refs/heads/main/openapi/nuitee-openapi.yml
- filename: nuitee-openapi.yml
  format: yaml
  label: LiteAPI Rates Search API
  slug: rates-search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuitee/refs/heads/main/openapi/nuitee-openapi.yml
- filename: nuitee-openapi.yml
  format: yaml
  label: LiteAPI Booking API
  slug: booking
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuitee/refs/heads/main/openapi/nuitee-openapi.yml
- filename: nuitee-openapi.yml
  format: yaml
  label: LiteAPI Loyalty and Vouchers API
  slug: loyalty-vouchers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuitee/refs/heads/main/openapi/nuitee-openapi.yml
- filename: nuitee-openapi.yml
  format: yaml
  label: LiteAPI Webhooks
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuitee/refs/heads/main/openapi/nuitee-openapi.yml
consequence_counts:
  read: 13
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Nuitee Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 20
overview: 'Nuitée (LiteAPI) exposes 20 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Nuitée (LiteAPI)
provider_slug: nuitee
slug: nuitee-agentic-access
source_filename: nuitee-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/nuitee-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    connected: 13\n    acting: 7\n  by_consequence:\n    read: 13\n    write: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /data/hotels\n  method: get\n  operationId: getHotels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/hotel\n  method: get\n  operationId: getHotelDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/reviews\n  method: get\n  operationId:\
  \ getHotelReviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/countries\n  method: get\n  operationId: getCountries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/cities\n  method: get\n  operationId: getCities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/currencies\n  method: get\n  operationId: getCurrencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/iatacodes\n  method: get\n  operationId: getIataCodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /hotels/rates\n  method: post\n  operationId: searchRates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rates/prebook\n  method: post\n  operationId: prebook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rates/book\n  method: post\n  operationId: book\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n  \
  \    - high-value\n    audit: required\n- path: /bookings\n  method: get\n  operationId: listBookings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bookings/{bookingId}\n  method: get\n  operationId: getBooking\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bookings/{bookingId}\n  method: put\n  operationId: cancelBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /loyalties\n  method: get\n  operationId: getLoyalty\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /loyalties\n  method: put\n  operationId: updateLoyalty\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /guests/{guestId}/bookings\n  method: get\n  operationId: getGuestBookings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vouchers\n  method: get\n  operationId: listVouchers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vouchers\n  method: post\n  operationId: createVoucher\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n  \
  \    max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vouchers/{voucherId}\n  method: get\n  operationId: getVoucher\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vouchers/{voucherId}\n  method: delete\n  operationId: deleteVoucher\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nuitee/refs/heads/main/agentic-access/nuitee-agentic-access.yml
summary_line: 20 operations · 7 acting
tags:
- Travel
- Hotels
- Booking
- Distribution
- Hospitality
---
