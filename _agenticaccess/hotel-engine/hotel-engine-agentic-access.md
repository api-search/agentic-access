---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 1
api_specs:
- filename: hotel-engine-catalogservice-api-openapi.yml
  format: yaml
  label: Engine Catalog Service API
  slug: hotel-engine-catalogservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotel-engine/refs/heads/main/openapi/hotel-engine-catalogservice-api-openapi.yml
- filename: hotel-engine-contentservice-api-openapi.yml
  format: yaml
  label: Engine Content Service API
  slug: hotel-engine-contentservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotel-engine/refs/heads/main/openapi/hotel-engine-contentservice-api-openapi.yml
- filename: hotel-engine-lodgingbookingservice-api-openapi.yml
  format: yaml
  label: Engine Lodging Booking Service API
  slug: hotel-engine-lodgingbookingservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotel-engine/refs/heads/main/openapi/hotel-engine-lodgingbookingservice-api-openapi.yml
- filename: hotel-engine-lodgingshoppingservice-api-openapi.yml
  format: yaml
  label: Engine Lodging Shopping Service API
  slug: hotel-engine-lodgingshoppingservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotel-engine/refs/heads/main/openapi/hotel-engine-lodgingshoppingservice-api-openapi.yml
consequence_counts:
  physical: 2
  read: 1
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Hotel Engine Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /book/v1/lodging/booking
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /book/v1/lodging/booking/preview-cancellation
operation_count: 11
overview: 'Engine exposes 11 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read, 8 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Engine
provider_slug: hotel-engine
slug: hotel-engine-agentic-access
source_filename: hotel-engine-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: generated\nsource: openapi/hotel-engine-omni-partner-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    acting: 10\n    connected: 1\n  by_consequence:\n    write: 8\n    read: 1\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /shop/v1/lodging/availability\n  method: post\n  operationId: LodgingShoppingService_FindAvailability\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shop/v1/lodging/best-offers\n  method:\
  \ post\n  operationId: LodgingShoppingService_FindBestOffers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /content/v1/catalog/property\n  method: post\n  operationId: CatalogService_ListPropertyCatalog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /content/v1/properties\n  method: post\n  operationId: ContentService_GetProperties\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /content/v1/property\n  method: get\n  operationId: ContentService_ListProperties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /book/v1/lodging/booking\n  method: post\n  operationId: LodgingBookingService_GetBookings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /book/v1/lodging/booking\n  method: put\n  operationId: LodgingBookingService_Book\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n \
  \   escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /book/v1/lodging/booking/generate-folio\n  method: post\n  operationId: LodgingBookingService_GenerateFolio\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /book/v1/lodging/booking/preview-cancellation\n  method: post\n  operationId: LodgingBookingService_PreviewCancellation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /book/v1/lodging/booking/submit-cancellation\n\
  \  method: post\n  operationId: LodgingBookingService_SubmitCancellation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /book/v1/lodging/confirm-offer\n  method: post\n  operationId: LodgingBookingService_ConfirmOffer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hotel-engine/refs/heads/main/agentic-access/hotel-engine-agentic-access.yml
summary_line: 11 operations · 10 acting
tags:
- Company
- Travel
- Business Travel
- Lodging
- Hotels
- Booking
- Travel Management
- Expense Management
- Payments
- gRPC
- Protobuf
- Partner API
---
