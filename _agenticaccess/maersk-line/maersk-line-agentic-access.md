---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 14
api_specs:
- filename: maersk-line-airbookings-api-openapi.yml
  format: yaml
  label: Maersk AirBookings API
  slug: maersk-line-airbookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maersk-line/refs/heads/main/openapi/maersk-line-airbookings-api-openapi.yml
- filename: maersk-line-billoflading-api-openapi.yml
  format: yaml
  label: Maersk BillOfLading API
  slug: maersk-line-billoflading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maersk-line/refs/heads/main/openapi/maersk-line-billoflading-api-openapi.yml
- filename: maersk-line-bookings-api-openapi.yml
  format: yaml
  label: Maersk Bookings API
  slug: maersk-line-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maersk-line/refs/heads/main/openapi/maersk-line-bookings-api-openapi.yml
- filename: maersk-line-containers-api-openapi.yml
  format: yaml
  label: Maersk Containers API
  slug: maersk-line-containers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maersk-line/refs/heads/main/openapi/maersk-line-containers-api-openapi.yml
- filename: maersk-line-demurragedetention-api-openapi.yml
  format: yaml
  label: Maersk DemurrageDetention API
  slug: maersk-line-demurragedetention-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maersk-line/refs/heads/main/openapi/maersk-line-demurragedetention-api-openapi.yml
- filename: maersk-line-locations-api-openapi.yml
  format: yaml
  label: Maersk Locations API
  slug: maersk-line-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maersk-line/refs/heads/main/openapi/maersk-line-locations-api-openapi.yml
- filename: maersk-line-offers-api-openapi.yml
  format: yaml
  label: Maersk Offers API
  slug: maersk-line-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maersk-line/refs/heads/main/openapi/maersk-line-offers-api-openapi.yml
- filename: maersk-line-schedules-api-openapi.yml
  format: yaml
  label: Maersk Schedules API
  slug: maersk-line-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maersk-line/refs/heads/main/openapi/maersk-line-schedules-api-openapi.yml
- filename: maersk-line-tracking-api-openapi.yml
  format: yaml
  label: Maersk Tracking API
  slug: maersk-line-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maersk-line/refs/heads/main/openapi/maersk-line-tracking-api-openapi.yml
- filename: maersk-line-vgm-api-openapi.yml
  format: yaml
  label: Maersk VGM API
  slug: maersk-line-vgm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maersk-line/refs/heads/main/openapi/maersk-line-vgm-api-openapi.yml
consequence_counts:
  physical: 1
  read: 14
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Maersk Line Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /export-shipments/vgm/v1/shipments/{transportDocumentReference}/vgm
operation_count: 20
overview: 'Maersk exposes 20 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read, 5 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Maersk
provider_slug: maersk-line
slug: maersk-line-agentic-access
source_filename: maersk-line-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/maersk-air-booking-api-openapi.yml, openapi/maersk-bill-of-lading-api-openapi.yml,\n  openapi/maersk-demurrage-detention-api-openapi.yml, openapi/maersk-ocean-booking-api-openapi.yml,\n  openapi/maersk-product-offers-api-openapi.yml, openapi/maersk-schedules-api-openapi.yml, openapi/maersk-track-and-trace-api-openapi.yml,\n  openapi/maersk-vgm-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    acting: 6\n    connected: 14\n  by_consequence:\n    write: 5\n    read: 14\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /air-booking/v1/bookings\n  method: post\n  operationId: createAirBooking\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /air-booking/v1/bookings/{bookingReference}\n  method: get\n  operationId: getAirBooking\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dcsa/ebl/v3/transport-documents/{transportDocumentReference}\n  method: get\n  operationId: getTransportDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - ebl\n- path: /dcsa/ebl/v3/transport-documents/{transportDocumentReference}/approve\n  method: patch\n  operationId: approveTransportDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - ebl\n- path: /demurrage-detention/v1/charges\n  method: get\n  operationId: getDemurrageDetention\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dcsa/bkg/v2/bookings\n  method: post\n  operationId: createBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - booking\n- path: /dcsa/bkg/v2/bookings/{carrierBookingReference}\n  method: get\n  operationId: getBooking\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - booking\n- path: /dcsa/bkg/v2/bookings/{carrierBookingReference}\n  method: patch\n  operationId: amendBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - booking\n- path: /dcsa/bkg/v2/bookings/{carrierBookingReference}\n  method: delete\n  operationId: cancelBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - booking\n- path: /offers/v2/offers/brand/{brandScac}/departuredate/{departureDate}\n  method:\
  \ get\n  operationId: listAvailableOffers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /offers/v2/offers/brand/{brandScac}/locations\n  method: get\n  operationId: getPortPairs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /offers/v2/offers/brand/{brandScac}/locations/origins\n  method: get\n  operationId: getOriginPorts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /offers/v2/offers/brand/{brandScac}/locations/destinations\n  method: get\n  operationId: getDestinationPorts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /offers/v2/offers/containers\n  method:\
  \ get\n  operationId: listContainers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/ocean-products/point-to-point\n  method: get\n  operationId: getPointToPointSchedules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dcsa/cs/v1/service-schedules\n  method: get\n  operationId: getServiceSchedules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /track-and-trace-private/shipments\n  method: get\n  operationId: listShipmentEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n- path: /track-and-trace-private/events\n  method: get\n  operationId:\
  \ listContainerEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n- path: /export-shipments/vgm/v1/shipments/{transportDocumentReference}/vgm\n  method: post\n  operationId: submitVgm\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - vgm\n- path: /export-shipments/vgm/v1/shipments/{transportDocumentReference}/vgm\n  method: get\n  operationId: getVgm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - vgm\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maersk-line/refs/heads/main/agentic-access/maersk-line-agentic-access.yml
summary_line: 20 operations · 6 acting
tags:
- Shipping
- Logistics
- Container Shipping
- Ocean Freight
- Air Freight
- Supply Chain
- DCSA
- Maritime
---
