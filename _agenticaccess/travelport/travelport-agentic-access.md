---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 12
api_specs:
- filename: travelport-booking-api-openapi.yml
  format: yaml
  label: Travelport Booking API
  slug: travelport-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelport/refs/heads/main/openapi/travelport-booking-api-openapi.yml
- filename: travelport-emds-api-openapi.yml
  format: yaml
  label: Travelport EMDs API
  slug: travelport-emds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelport/refs/heads/main/openapi/travelport-emds-api-openapi.yml
- filename: travelport-fare-rules-api-openapi.yml
  format: yaml
  label: Travelport Fare Rules API
  slug: travelport-fare-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelport/refs/heads/main/openapi/travelport-fare-rules-api-openapi.yml
- filename: travelport-modifications-api-openapi.yml
  format: yaml
  label: Travelport Modifications API
  slug: travelport-modifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelport/refs/heads/main/openapi/travelport-modifications-api-openapi.yml
- filename: travelport-pricing-api-openapi.yml
  format: yaml
  label: Travelport Pricing API
  slug: travelport-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelport/refs/heads/main/openapi/travelport-pricing-api-openapi.yml
- filename: travelport-queues-api-openapi.yml
  format: yaml
  label: Travelport Queues API
  slug: travelport-queues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelport/refs/heads/main/openapi/travelport-queues-api-openapi.yml
- filename: travelport-reservations-api-openapi.yml
  format: yaml
  label: Travelport Reservations API
  slug: travelport-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelport/refs/heads/main/openapi/travelport-reservations-api-openapi.yml
- filename: travelport-search-api-openapi.yml
  format: yaml
  label: Travelport Search API
  slug: travelport-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelport/refs/heads/main/openapi/travelport-search-api-openapi.yml
- filename: travelport-seats-and-ancillaries-api-openapi.yml
  format: yaml
  label: Travelport Seats and Ancillaries API
  slug: travelport-seats-and-ancillaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelport/refs/heads/main/openapi/travelport-seats-and-ancillaries-api-openapi.yml
- filename: travelport-ticketing-api-openapi.yml
  format: yaml
  label: Travelport Ticketing API
  slug: travelport-ticketing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelport/refs/heads/main/openapi/travelport-ticketing-api-openapi.yml
- filename: travelport-workbench-api-openapi.yml
  format: yaml
  label: Travelport Workbench API
  slug: travelport-workbench-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelport/refs/heads/main/openapi/travelport-workbench-api-openapi.yml
consequence_counts:
  read: 12
  write: 18
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Travelport Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 30
overview: 'Travelport exposes 30 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read and 18 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Travelport
provider_slug: travelport
slug: travelport-agentic-access
source_filename: travelport-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/travelport-booking-api-openapi.yml, openapi/travelport-emds-api-openapi.yml,\n  openapi/travelport-fare-rules-api-openapi.yml, openapi/travelport-modifications-api-openapi.yml,\n  openapi/travelport-pricing-api-openapi.yml, openapi/travelport-queues-api-openapi.yml, openapi/travelport-reservations-api-openapi.yml,\n  openapi/travelport-search-api-openapi.yml, openapi/travelport-seats-and-ancillaries-api-openapi.yml,\n  openapi/travelport-ticketing-api-openapi.yml, openapi/travelport-workbench-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 30\n  by_action_class:\n    acting: 18\n    connected: 12\n  by_consequence:\n    write: 18\n    read: 12\n  human_in_the_loop_required:\
  \ 0\noperations:\n- path: /air/book/reservation/reservations/build\n  method: post\n  operationId: postAirBookReservationReservationsBuild\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /air/emds/{Identifier}\n  method: get\n  operationId: getAirEmdsByIdentifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /air/emds/{Identifier}\n  method: put\n  operationId: putAirEmdsByIdentifier\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /air/emds/getbylocator\n  method: get\n  operationId: getAirEmdsGetbylocator\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /air/farerule/farerules/fromoffer\n  method: get\n  operationId: getAirFareruleFarerulesFromoffer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /air/farerule/farerules/fromreservation\n  method: get\n  operationId: getAirFareruleFarerulesFromreservation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /air/book/reservation/reservations/divide\n  method: post\n  operationId: postAirBookReservationReservationsDivide\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /air/modify/reservations/{Identifier}\n  method: post\n  operationId: postAirModifyReservationsByIdentifier\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /air/change/catalogofferingsairchange\n  method: post\n  operationId: postAirChangeCatalogofferingsairchange\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /air/price/offers/buildfromcatalogproductofferings\n\
  \  method: post\n  operationId: postAirPriceOffersBuildfromcatalogproductofferings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /air/price/offers/buildfromproducts\n  method: post\n  operationId: postAirPriceOffersBuildfromproducts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /air/queue/queue\n  method: post\n  operationId: postAirQueueQueue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /air/queue/queue/remove\n  method: post\n  operationId: postAirQueueQueueRemove\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /air/queue/queue/list\n  method: post\n  operationId: postAirQueueQueueList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /air/book/reservation/reservations/{Identifier}\n  method: get\n  operationId: getAirBookReservationReservationsByIdentifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /air/book/reservation/reservations/{Identifier}\n\
  \  method: post\n  operationId: postAirBookReservationReservationsByIdentifier\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /air/book/reservation/reservations/getbylocator\n  method: get\n  operationId: getAirBookReservationReservationsGetbylocator\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /air/search/airAvailability\n  method: post\n  operationId: postAirSearchAirAvailability\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /air/catalog/search/catalogproductofferings\n  method: post\n  operationId: postAirCatalogSearchCatalogproductofferings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /air/catalog/search/catalogproductofferings/buildnext\n  method: post\n  operationId: postAirCatalogSearchCatalogproductofferingsBuildnext\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /air/search/seat/catalogofferingsancillaries/seatavailabilities\n  method: post\n  operationId: postAirSearchSeatCatalogofferingsancillariesSeatavailabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /air/ancillaryshop/catalogofferingsancillaries\n  method: post\n  operationId: postAirAncillaryshopCatalogofferingsancillaries\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /air/ticket/tickets/getbylocator\n  method: post\n  operationId: postAirTicketTicketsGetbylocator\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /air/ticket/tickets/{Identifier}\n  method: get\n  operationId: getAirTicketTicketsByIdentifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /air/ticket/tickets/updatestatus/{Identifier}\n  method:\
  \ put\n  operationId: putAirTicketTicketsUpdatestatusByIdentifier\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/void\n  method: post\n  operationId: postDocumentsVoid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /air/book/session/reservationworkbench\n  method: post\n  operationId: postAirBookSessionReservationworkbench\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /air/book/session/reservationworkbench/buildfromlocator\n  method: post\n  operationId: postAirBookSessionReservationworkbenchBuildfromlocator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /air/book/session/reservationworkbench/{Identifier}\n  method: get\n  operationId: getAirBookSessionReservationworkbenchByIdentifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /air/book/session/reservationworkbench/{Identifier}\n  method: delete\n  operationId: deleteAirBookSessionReservationworkbenchByIdentifier\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/travelport/refs/heads/main/agentic-access/travelport-agentic-access.yml
summary_line: 30 operations · 18 acting
tags:
- Travel
- Travel Technology
- Reservations
- GDS
- NDC
- Flights
- Hotels
- Payments
---
