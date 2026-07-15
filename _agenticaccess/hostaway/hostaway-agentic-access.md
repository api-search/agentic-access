---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 12
api_specs:
- filename: hostaway-listings-api-openapi.yml
  format: yaml
  label: Hostaway Listings API
  slug: hostaway-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostaway/refs/heads/main/openapi/hostaway-listings-api-openapi.yml
- filename: hostaway-reservations-api-openapi.yml
  format: yaml
  label: Hostaway Reservations API
  slug: hostaway-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostaway/refs/heads/main/openapi/hostaway-reservations-api-openapi.yml
- filename: hostaway-calendar-api-openapi.yml
  format: yaml
  label: Hostaway Calendar API
  slug: hostaway-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostaway/refs/heads/main/openapi/hostaway-calendar-api-openapi.yml
- filename: hostaway-webhooks-api-openapi.yml
  format: yaml
  label: Hostaway Webhooks API
  slug: hostaway-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostaway/refs/heads/main/openapi/hostaway-webhooks-api-openapi.yml
consequence_counts:
  read: 12
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Hostaway Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 23
overview: 'Hostaway exposes 23 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read and 11 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Hostaway
provider_slug: hostaway
slug: hostaway-agentic-access
source_filename: hostaway-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/hostaway-calendar-api-openapi.yml, openapi/hostaway-listings-api-openapi.yml,\n  openapi/hostaway-reservations-api-openapi.yml, openapi/hostaway-webhooks-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 12\n    acting: 11\n  by_consequence:\n    read: 12\n    write: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /listings/{listingId}/calendar\n  method: get\n  operationId: getCalendarDays\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /listings/{listingId}/calendar\n  method: put\n  operationId: updateCalendarDay\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listings/{listingId}/calendar/batch\n  method: post\n  operationId: batchUpdateCalendar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listings\n  method: get\n  operationId: listListings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /listings\n  method: post\n  operationId: createListing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n \
  \   subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listings/{listingId}\n  method: get\n  operationId: getListing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /listings/{listingId}\n  method: put\n  operationId: updateListing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listings/{listingId}/amenities\n  method: get\n  operationId: listListingAmenities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /listings/{listingId}/bedTypes\n  method: get\n  operationId: listListingBedTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /listings/{listingId}/images\n  method: get\n  operationId: listListingImages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /listings/{listingId}/images\n  method: post\n  operationId: addListingImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reservations\n  method: get\n  operationId: listReservations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reservations\n  method: post\n  operationId: createReservation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reservations/{reservationId}\n  method: get\n  operationId: getReservation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reservations/{reservationId}\n  method: put\n  operationId: updateReservation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /reservations/{reservationId}/coupons\n  method: post\n  operationId: createReservationCoupon\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reservations/{reservationId}/fees\n  method: get\n  operationId: listReservationFees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reservations/{reservationId}/units\n  method: get\n  operationId: listReservationUnits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/unifiedWebhooks\n  method: get\n  operationId: listUnifiedWebhooks\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/unifiedWebhooks\n  method: post\n  operationId: createUnifiedWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/unifiedWebhooks/{webhookId}\n  method: get\n  operationId: getUnifiedWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/unifiedWebhooks/{webhookId}\n  method: put\n  operationId: updateUnifiedWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/unifiedWebhooks/{webhookId}\n  method: delete\n  operationId: deleteUnifiedWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hostaway/refs/heads/main/agentic-access/hostaway-agentic-access.yml
summary_line: 23 operations · 11 acting
tags:
- Vacation Rentals
- Short-Term Rentals
- Property Management
- Channel Manager
- Airbnb
- Vrbo
- Booking.com
- Expedia
- SaaS
---
