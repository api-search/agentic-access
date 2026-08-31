---
acting_count: 43
action_class_counts:
  acting: 43
  connected: 4
api_specs:
- filename: 20885222-5fccfe6e-479a-429f-a497-d42a0bb859c9
  format: yaml
  label: Trip Ninja DataStream API
  slug: tripninja-datastream-api
  spec_type: Postman
  url: https://www.postman.com/tripninjadevteam/workspace/trip-ninja-public/collection/20885222-5fccfe6e-479a-429f-a497-d42a0bb859c9
- filename: webjet-adminpanel-api-openapi.yml
  format: yaml
  label: Webjet Adminpanel API
  slug: webjet-adminpanel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webjet/refs/heads/main/openapi/webjet-adminpanel-api-openapi.yml
- filename: webjet-book-api-openapi.yml
  format: yaml
  label: Webjet Book API
  slug: webjet-book-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webjet/refs/heads/main/openapi/webjet-book-api-openapi.yml
- filename: webjet-booking-api-openapi.yml
  format: yaml
  label: Webjet Booking API
  slug: webjet-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webjet/refs/heads/main/openapi/webjet-booking-api-openapi.yml
- filename: webjet-cancel-api-openapi.yml
  format: yaml
  label: Webjet Cancel API
  slug: webjet-cancel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webjet/refs/heads/main/openapi/webjet-cancel-api-openapi.yml
- filename: webjet-details-api-openapi.yml
  format: yaml
  label: Webjet Details API
  slug: webjet-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webjet/refs/heads/main/openapi/webjet-details-api-openapi.yml
- filename: webjet-generate-solutions-api-openapi.yml
  format: yaml
  label: Webjet Generate Solutions API
  slug: webjet-generate-solutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webjet/refs/heads/main/openapi/webjet-generate-solutions-api-openapi.yml
- filename: webjet-get-searches-api-openapi.yml
  format: yaml
  label: Webjet Get Searches API
  slug: webjet-get-searches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webjet/refs/heads/main/openapi/webjet-get-searches-api-openapi.yml
- filename: webjet-msdp-api-openapi.yml
  format: yaml
  label: Webjet Msdp API
  slug: webjet-msdp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webjet/refs/heads/main/openapi/webjet-msdp-api-openapi.yml
- filename: webjet-pre-booking-api-openapi.yml
  format: yaml
  label: Webjet Pre Booking API
  slug: webjet-pre-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webjet/refs/heads/main/openapi/webjet-pre-booking-api-openapi.yml
- filename: webjet-price-api-openapi.yml
  format: yaml
  label: Webjet Price API
  slug: webjet-price-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webjet/refs/heads/main/openapi/webjet-price-api-openapi.yml
- filename: webjet-queue-api-openapi.yml
  format: yaml
  label: Webjet Queue API
  slug: webjet-queue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webjet/refs/heads/main/openapi/webjet-queue-api-openapi.yml
- filename: webjet-report-api-openapi.yml
  format: yaml
  label: Webjet Report API
  slug: webjet-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webjet/refs/heads/main/openapi/webjet-report-api-openapi.yml
- filename: webjet-results-api-openapi.yml
  format: yaml
  label: Webjet Results API
  slug: webjet-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webjet/refs/heads/main/openapi/webjet-results-api-openapi.yml
- filename: webjet-rules-api-openapi.yml
  format: yaml
  label: Webjet Rules API
  slug: webjet-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webjet/refs/heads/main/openapi/webjet-rules-api-openapi.yml
- filename: webjet-search-api-openapi.yml
  format: yaml
  label: Webjet Search API
  slug: webjet-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webjet/refs/heads/main/openapi/webjet-search-api-openapi.yml
- filename: webjet-super-trip-api-openapi.yml
  format: yaml
  label: Webjet Super Trip API
  slug: webjet-super-trip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webjet/refs/heads/main/openapi/webjet-super-trip-api-openapi.yml
- filename: webjet-ticket-api-openapi.yml
  format: yaml
  label: Webjet Ticket API
  slug: webjet-ticket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webjet/refs/heads/main/openapi/webjet-ticket-api-openapi.yml
- filename: webjet-ticketing-api-openapi.yml
  format: yaml
  label: Webjet Ticketing API
  slug: webjet-ticketing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webjet/refs/heads/main/openapi/webjet-ticketing-api-openapi.yml
consequence_counts:
  read: 4
  write: 43
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Webjet Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 47
overview: 'Webjet exposes 47 API operations that an AI agent could call, of which 43 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 43 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Webjet
provider_slug: webjet
slug: webjet-agentic-access
source_filename: webjet-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: generated\nsource: openapi/webjet-tripninja-adminpanel-refresh-token-openapi.yml, openapi/webjet-tripninja-farestructure-generate-solutions-openapi.yml,\n  openapi/webjet-tripninja-farestructure-get-searches-openapi.yml, openapi/webjet-tripninja-farestructure-report-book-openapi.yml,\n  openapi/webjet-tripninja-farestructure-report-cancel-openapi.yml, openapi/webjet-tripninja-flights-core-openapi.yml,\n  openapi/webjet-tripninja-hotels-openapi.yml, openapi/webjet-tripninja-msdp-openapi.yml, openapi/webjet-tripninja-pricing-booking-openapi.yml,\n  openapi/webjet-tripninja-smartflights-generate-solutions-openapi.yml, openapi/webjet-tripninja-smartflights-get-searches-openapi.yml,\n  openapi/webjet-tripninja-smartflights-report-book-openapi.yml, openapi/webjet-tripninja-smartflights-report-cancel-openapi.yml,\n  openapi/webjet-tripninja-v2-booking-openapi.yml, openapi/webjet-tripninja-v2-core-openapi.yml,\n  openapi/webjet-tripninja-virtual-interlining-generate-solutions-openapi.yml,\
  \ openapi/webjet-tripninja-virtual-interlining-get-searches-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 47\n  by_action_class:\n    acting: 43\n    connected: 4\n  by_consequence:\n    write: 43\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /adminpanel/refresh-token/\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/generate-solutions/\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/get-searches/\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/report/book/\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/report/cancel/\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /search/flights/{endpoint}/\n  method: post\n  operationId: FlightSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pre-booking/\n  method: post\n  operationId: PriceConfirmationReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /booking/\n  method: post\n  operationId: BookingReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ticketing/\n  method: post\n  operationId: TicketingReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cancel/\n  method: post\n  operationId: CancelBookingReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /search/hotels/{endpoint}\n  method: post\n  operationId: Search\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /details/hotels/{endpoint}/\n  method: post\n  operationId: Details\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rules/hotels/{endpoint}/\n  method: post\n  operationId: Rules\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /price/hotels/{endpoint}/\n  method: post\n  operationId: PriceConfirm\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /price/hotels/{endpoint}/\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /msdp/search/prod\n  method: post\n  operationId: MSDPSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /msdp/results/flights/?trip_id={trip_id}\n\
  \  method: get\n  operationId: MSDPGetFlightResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /results/hotels/?hotel_trace_id={hotel_trace_id}&rating={rating}&area={area}&min_price={min_price}&max_price={max_price}&min_distance={min_distance}&max_distance={max_distance}&hotel_chain={hotel_chain}&amenities={amenities}&sort_by={sort_by}\n  method: get\n  operationId: MSDPGetHotelResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /msdp/search/removehotel/\n  method: patch\n  operationId: MSDPRemoveHotelResult\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /msdp/detail/hotel/prod\n  method: post\n  operationId: MSDPGetHotelDetails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /msdp/pre-booking/prod\n  method: post\n  operationId: MSDPPriceConfirmationReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /msdp/booking/\n  method: post\n  operationId: MSDPBookingReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /msdp/ticketing/\n  method: post\n  operationId: MSDPTicketingReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /msdp/cancel/\n  method: post\n  operationId: MSDPCancelBookingReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /price/{endpoint}/\n  method: post\n  operationId: PriceConfirm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /book/list/?agency={agency}&user={agent_email}&offset={offset}&limit={limit}\n  method: get\n  operationId: ListBooking\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /book/trip/{super_trip_id}/?agency={agency}\n  method: get\n  operationId: BookingDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /book/{endpoint}/\n  method: post\n  operationId: CreateBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /book/\n  method: delete\n  operationId: CancelBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /queue/\n  method: post\n  operationId: AddBookingToTicketingQueue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ticket/\n  method: post\n  operationId: Ticket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v3/generate-solutions/\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/get-searches/\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/report/book/\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v3/report/cancel/\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /search/flight/{endpoint}/flight/\n  method: post\n  operationId: Search\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /price/flight/{endpoint}/\n  method: post\n  operationId: PriceConfirm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n   \
  \   - high-value\n    audit: required\n- path: /book/flight/{endpoint}/\n  method: post\n  operationId: CreateBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /book/\n  method: delete\n  operationId: CancelBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /queue/\n  method: post\n  operationId: AddBookingToTicketingQueue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ticket/\n  method: post\n  operationId: Ticket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /super_trip/{id}/\n  method: put\n  operationId: SuperTrip\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /super_trip/{id}/part/\n  method: delete\n  operationId: SuperTripPartDeletion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /get-searches/\n  method: post\n  operationId: GetSearchesRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /generate-solutions/\n  method: post\n  operationId: GenerateSolutionsRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/generate-solutions/\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/get-searches/\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/webjet/refs/heads/main/agentic-access/webjet-agentic-access.yml
summary_line: 47 operations · 43 acting
tags:
- Travel
- Australia
- OTA
- Aviation
- Booking
- Distribution
- Flight Search
- Car Rental
- New Zealand
- Travel Technology
---
