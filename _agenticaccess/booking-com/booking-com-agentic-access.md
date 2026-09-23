---
acting_count: 164
action_class_counts:
  acting: 164
  connected: 46
api_specs:
- filename: booking-com-demand-api-3-2-openapi.yml
  format: yaml
  label: Booking.com Demand API
  slug: booking-com-demand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-demand-api-3-2-openapi.yml
- filename: booking-com-connect-api-openapi.yml
  format: yaml
  label: Booking.com Connect API
  slug: booking-com-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-connect-api-openapi.yml
- filename: booking-com-status-api-openapi.yml
  format: yaml
  label: Booking.com Status API
  slug: booking-com-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-status-api-openapi.yml
- filename: booking-com-charges-api-openapi.yml
  format: yaml
  label: Booking.com Charges API
  slug: booking-com-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-charges-api-openapi.yml
- filename: booking-com-contacts-api-openapi.yml
  format: yaml
  label: Booking.com Contacts API
  slug: booking-com-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-contacts-api-openapi.yml
- filename: booking-com-contracting-api-openapi.yml
  format: yaml
  label: Booking.com Contracting API
  slug: booking-com-contracting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-contracting-api-openapi.yml
- filename: booking-com-facilities-api-openapi.yml
  format: yaml
  label: Booking.com Facilities API
  slug: booking-com-facilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-facilities-api-openapi.yml
- filename: booking-com-historical-reservations-api-openapi.yml
  format: yaml
  label: Booking.com Historical Reservations API
  slug: booking-com-historical-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-historical-reservations-api-openapi.yml
- filename: booking-com-payments-api-openapi.yml
  format: yaml
  label: Booking.com Payments API
  slug: booking-com-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-payments-api-openapi.yml
- filename: booking-com-payments-by-booking-onboarding-api-openapi.yml
  format: yaml
  label: Booking.com Payments by Booking Onboarding API
  slug: booking-com-payments-by-booking-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-payments-by-booking-onboarding-api-openapi.yml
- filename: booking-com-property-api-openapi.yml
  format: yaml
  label: Booking.com Property API
  slug: booking-com-property-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-property-api-openapi.yml
- filename: booking-com-property-health-api-openapi.yml
  format: yaml
  label: Booking.com Property Health API
  slug: booking-com-property-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-property-health-api-openapi.yml
- filename: booking-com-reconciliation-api-openapi.yml
  format: yaml
  label: Booking.com Reconciliation API
  slug: booking-com-reconciliation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-reconciliation-api-openapi.yml
- filename: booking-com-rooms-api-openapi.yml
  format: yaml
  label: Booking.com Rooms API
  slug: booking-com-rooms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-rooms-api-openapi.yml
- filename: booking-com-valueadds-api-openapi.yml
  format: yaml
  label: Booking.com Value Adds Catalog API
  slug: booking-com-valueadds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/openapi/booking-com-valueadds-api-openapi.yml
consequence_counts:
  physical: 44
  read: 46
  write: 120
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Booking Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /charges-api/properties/{propertyId}/charges
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /common/payments/cards
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /common/payments/cards
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /common/payments/cards
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /common/payments/currencies
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /common/payments/currencies
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /common/payments/currencies
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /connectivity-payments/pbb/configurations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /connectivity-payments/pbb/configurations/status
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /connectivity-payments/pbb/eligibility
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /connectivity-payments/recon-reports
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /messages/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /messages/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/create
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/create
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/create
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/details
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/details
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/details
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/details/accommodations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/details/accommodations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/details/accommodations
operation_count: 210
overview: 'Booking.com exposes 210 API operations that an AI agent could call, of which 164 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 46 read, 120 write, and 44 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Booking.com
provider_slug: booking-com
slug: booking-com-agentic-access
source_filename: booking-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: generated\nsource: openapi/booking-com-charges-api-openapi.yml, openapi/booking-com-connect-api-openapi.yml,\n  openapi/booking-com-contacts-api-openapi.yml, openapi/booking-com-contracting-api-openapi.yml,\n  openapi/booking-com-demand-api-3-1-openapi.yml, openapi/booking-com-demand-api-3-2-beta-openapi.yml,\n  openapi/booking-com-demand-api-3-2-openapi.yml, openapi/booking-com-facilities-api-openapi.yml,\n  openapi/booking-com-facilities-api-remote-sync-openapi.yml, openapi/booking-com-historical-reservations-api-openapi.yml,\n  openapi/booking-com-payments-api-openapi.yml, openapi/booking-com-payments-by-booking-onboarding-api-openapi.yml,\n  openapi/booking-com-property-api-openapi.yml, openapi/booking-com-property-health-api-openapi.yml,\n  openapi/booking-com-reconciliation-api-openapi.yml, openapi/booking-com-rooms-api-bulk-openapi.yml,\n  openapi/booking-com-rooms-api-generated-names-openapi.yml, openapi/booking-com-rooms-api-openapi.yml,\n\
  \  openapi/booking-com-status-api-openapi.yml, openapi/booking-com-valueadds-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 210\n  by_action_class:\n    connected: 46\n    acting: 164\n  by_consequence:\n    read: 46\n    physical: 44\n    write: 120\n  human_in_the_loop_required: 0\noperations:\n- path: /charges-api/properties/{propertyId}/charges\n  method: get\n  operationId: getChargesForProperty\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /charges-api/properties/{propertyId}/charges\n  method: post\n  operationId: updateChargesForProperty\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /charges-api/meta\n  method: get\n  operationId: meta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/conversions\n  method: post\n  operationId: getConversions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inventory/properties\n  method: post\n  operationId: streamProperties\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /demand-api-v2-compatible/reviews\n  method: get\n  operationId: getHotelsReviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /demand-api-v2-compatible/reviewScores\n  method: get\n  operationId: getHotelsReviewScores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /demand-api-v2-compatible/hotels\n  method: get\n  operationId: getHotels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /demand-api-v2-compatible/hotelTypes\n  method: get\n  operationId: getHotelTypes\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /demand-api-v2-compatible/hotelThemeTypes\n  method: get\n  operationId: getHotelThemeTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /demand-api-v2-compatible/hotelFacilityTypes\n  method: get\n  operationId: getRoomFacilityTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /demand-api-v2-compatible/hotelAvailability\n  method: get\n  operationId: getHotelAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /demand-api-v2-compatible/blockAvailability\n  method: get\n  operationId: getBlockAvailability\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /properties/{propertyId}/contacts\n  method: get\n  operationId: getAllContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /properties/{propertyId}/contacts\n  method: put\n  operationId: overwriteContacts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partners/invite\n  method: post\n  operationId: postPartnersInvite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /partners/addendum\n  method: post\n  operationId: postPartnersAddendum\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partners/legal-details\n  method: post\n  operationId: postPartnersLegalDetails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partners/legal-details/legal-entity/{id}\n  method: get\n  operationId: getPartnersLegalDetailsLegalEntityById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /partners/request_access\n  method: post\n  operationId: postPartnersRequestAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partners/resend-invite\n  method: post\n  operationId: postPartnersResendInvite\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partners/resend-addendum\n  method: post\n  operationId: postPartnersResendAddendum\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accommodations/search\n  method: post\n  operationId: /accommodations/search\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accommodations/availability\n  method: post\n  operationId: /accommodations/availability\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /accommodations/bulk-availability\n  method: post\n  operationId: /accommodations/bulk-availability\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accommodations/chains\n  method: post\n  operationId: /accommodations/chains\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accommodations/constants\n  method: post\n  operationId: /accommodations/constants\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accommodations/details\n  method: post\n  operationId: /accommodations/details\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accommodations/details/changes\n  method: post\n  operationId: /accommodations/details/changes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accommodations/reviews\n  method: post\n  operationId: /accommodations/reviews\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accommodations/reviews/scores\n  method: post\n  operationId: /accommodations/reviews/scores\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /common/languages\n  method: post\n  operationId: /common/languages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /common/locations/airports\n\
  \  method: post\n  operationId: /common/locations/airports\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /common/locations/cities\n  method: post\n  operationId: /common/locations/cities\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /common/locations/countries\n  method: post\n  operationId: /common/locations/countries\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /common/locations/districts\n  method: post\n  operationId: /common/locations/districts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /common/locations/landmarks\n  method: post\n  operationId: /common/locations/landmarks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /common/locations/regions\n  method: post\n  operationId: /common/locations/regions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /common/payments/cards\n  method: post\n  operationId: /common/payments/cards\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /common/payments/currencies\n  method: post\n  operationId: /common/payments/currencies\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /orders/preview\n  method: post\n  operationId: /orders/preview\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/create\n  method: post\n  operationId: /orders/create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/details\n  method: post\n  operationId: /orders/details\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n  \
  \  subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/details/accommodations\n  method: post\n  operationId: /orders/details/accommodations\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/details/cars\n  method: post\n  operationId: /orders/details/cars\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/details/flights\n  method: post\n  operationId: /orders/details/flights\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/modify\n  method: post\n  operationId: /orders/modify\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/cancel\n  method: post\n  operationId: /orders/cancel\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cars/search\n  method: post\n  operationId: /search\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cars/depots\n  method: post\n  operationId: /depots\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cars/depots/reviews/scores\n\
  \  method: post\n  operationId: /depots/reviews/scores\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cars/details\n  method: post\n  operationId: /details\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cars/suppliers\n  method: post\n  operationId: /suppliers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n \
  \   audit: required\n- path: /cars/constants\n  method: post\n  operationId: /constants\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages/send\n  method: post\n  operationId: sendMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages/conversations\n  method: post\n  operationId: retrieve-conversation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages/latest\n  method: post\n  operationId: fetchLatestMessages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages/latest/confirm\n  method: post\n  operationId: confirmMessageReceipt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages/attachments/upload\n  method: post\n  operationId: uploadAttachment\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages/attachments/download\n  method: post\n  operationId: downloadMessageAttachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages/attachments/metadata\n  method: post\n  operationId: getAttachmentMetadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accommodations/search\n  method:\
  \ post\n  operationId: /accommodations/search\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accommodations/availability\n  method: post\n  operationId: /accommodations/availability\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accommodations/chains\n  method: post\n  operationId: /accommodations/chains\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /accommodations/constants\n  method: post\n  operationId: /accommodations/constants\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accommodations/details\n  method: post\n  operationId: /accommodations/details\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accommodations/details/changes\n  method: post\n  operationId: /accommodations/details/changes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accommodations/reviews\n  method: post\n  operationId: /accommodations/reviews\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accommodations/reviews/scores\n  method: post\n  operationId: /accommodations/reviews/scores\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accommodations/smart-search\n  method: post\n  operationId: /accommodations/smart-search\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accommodations/third-party-suppliers\n  method: post\n  operationId: /accommodations/third-party-suppliers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /attractions/search\n  method: post\n  operationId: /search\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n  \
  \  audit: required\n- path: /attractions/details\n  method: post\n  operationId: /attractions/details\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /attractions/reviews\n  method: post\n  operationId: /attractions/reviews\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /attractions/reviews/scores\n  method: post\n  operationId: /attractions/reviews/scores\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /attractions/constants\n  method: post\n  operationId: constants\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cars/search\n  method: post\n  operationId: search\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cars/availability\n  method: post\n  operationId: /availability\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cars/constants\n  method: post\n  operationId: constants\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cars/depots\n  method: post\n  operationId: depots\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cars/depots/reviews/scores\n  method: post\n  operationId: depotScores\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cars/details\n  method: post\n  operationId: details\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cars/suppliers\n  method: post\n  operationId: suppliers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cars/terms-and-conditions\n  method: post\n  operationId: terms-and-conditions\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /common/autocomplete\n  method: post\n  operationId: /common/autocomplete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /common/languages\n  method: post\n  operationId: /common/languages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /common/locations/airports\n  method: post\n  operationId:\
  \ /common/locations/airports\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /common/locations/cities\n  method: post\n  operationId: /common/locations/cities\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /common/locations/countries\n  method: post\n  operationId: /common/locations/countries\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /common/locations/districts\n  method: post\n  operationId: /common/locations/districts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /common/locations/landmarks\n  method: post\n  operationId: /common/locations/landmarks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\n\n# --- truncated at 32 KB (70 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/agentic-access/booking-com-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/booking-com/refs/heads/main/agentic-access/booking-com-agentic-access.yml
summary_line: 210 operations · 164 acting
tags:
- Travel
- Hospitality
- Accommodation
- Booking
- Car Rental
- Payments
- Connectivity
- Marketplace
- OTA
- Attractions
---
