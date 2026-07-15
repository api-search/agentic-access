---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 11
api_specs:
- filename: hotelrunner-openapi.yml
  format: yaml
  label: HotelRunner Inventory API
  slug: hotelrunner-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotelrunner/refs/heads/main/openapi/hotelrunner-openapi.yml
- filename: hotelrunner-openapi.yml
  format: yaml
  label: HotelRunner Reservations API
  slug: hotelrunner-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotelrunner/refs/heads/main/openapi/hotelrunner-openapi.yml
- filename: hotelrunner-openapi.yml
  format: yaml
  label: HotelRunner Channels API
  slug: hotelrunner-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotelrunner/refs/heads/main/openapi/hotelrunner-openapi.yml
- filename: hotelrunner-openapi.yml
  format: yaml
  label: HotelRunner Reference Data API
  slug: hotelrunner-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotelrunner/refs/heads/main/openapi/hotelrunner-openapi.yml
consequence_counts:
  read: 11
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Hotelrunner Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'HotelRunner exposes 15 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: HotelRunner
provider_slug: hotelrunner
slug: hotelrunner-agentic-access
source_filename: hotelrunner-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/hotelrunner-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 11\n    acting: 4\n  by_consequence:\n    read: 11\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /rooms\n  method: get\n  operationId: listRooms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rooms/~\n  method: put\n  operationId: updateRoomDateRange\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rooms/daily\n  method: put\n  operationId: updateRoomsMultiDates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reservations\n  method: get\n  operationId: listReservations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reservations/fire\n  method: put\n  operationId: updateReservationState\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /reservations/~\n  method: put\n  operationId: confirmReservationDelivery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /infos/connected_channels\n  method: get\n  operationId: listConnectedChannels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/property/types.json\n  method: get\n  operationId: getPropertyKinds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/room/types.json\n  method: get\n  operationId: getRoomKinds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/currency/currencies.json\n  method: get\n  operationId: getCurrencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/get-property-services\n  method: get\n  operationId: getPropertyServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/get-property-facilities\n  method: get\n  operationId: getPropertyFacilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/get-room-amenities\n  method: get\n  operationId: getRoomAmenities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/country-codes\n\
  \  method: get\n  operationId: getCountryCodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/channel-list\n  method: get\n  operationId: getChannelList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hotelrunner/refs/heads/main/agentic-access/hotelrunner-agentic-access.yml
summary_line: 15 operations · 4 acting
tags:
- Hospitality
- Hotel
- Channel Manager
- Booking Engine
- PMS
- Travel
---
