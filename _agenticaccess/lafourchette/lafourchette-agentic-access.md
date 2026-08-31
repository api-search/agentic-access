---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 11
api_specs:
- filename: lafourchette-booking-flow-api-openapi.yml
  format: yaml
  label: LaFourchette Booking flow API
  slug: lafourchette-booking-flow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lafourchette/refs/heads/main/openapi/lafourchette-booking-flow-api-openapi.yml
- filename: lafourchette-data-api-openapi.yml
  format: yaml
  label: LaFourchette Data API
  slug: lafourchette-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lafourchette/refs/heads/main/openapi/lafourchette-data-api-openapi.yml
- filename: lafourchette-phone-api-openapi.yml
  format: yaml
  label: LaFourchette Phone API
  slug: lafourchette-phone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lafourchette/refs/heads/main/openapi/lafourchette-phone-api-openapi.yml
- filename: lafourchette-review-flow-api-openapi.yml
  format: yaml
  label: LaFourchette Review flow API
  slug: lafourchette-review-flow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lafourchette/refs/heads/main/openapi/lafourchette-review-flow-api-openapi.yml
- filename: lafourchette-v1-api-openapi.yml
  format: yaml
  label: LaFourchette V1 API
  slug: lafourchette-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lafourchette/refs/heads/main/openapi/lafourchette-v1-api-openapi.yml
consequence_counts:
  physical: 1
  read: 11
  safety-critical: 1
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Lafourchette Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v1/restaurants/{id}/availabilities/override
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/orders/{orderUuid}
operation_count: 21
overview: 'LaFourchette exposes 21 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 8 write, 1 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: LaFourchette
provider_slug: lafourchette
slug: lafourchette-agentic-access
source_filename: lafourchette-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: generated\nsource: openapi/lafourchette-b2b-api-openapi.yml, openapi/lafourchette-pos-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    acting: 10\n    connected: 11\n  by_consequence:\n    write: 8\n    read: 11\n    safety-critical: 1\n    physical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /v1/callCenter/callRecognitions\n  method: post\n  operationId: postV1CallCenterCallRecognitions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/customers\n  method: get\n  operationId: getV1Customers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customers/{id}\n  method: get\n  operationId: getV1CustomersId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/integrationStatus\n  method: patch\n  operationId: patchV1IntegrationStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/reservations\n  method: get\n  operationId: getV1Reservations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/reservations/{id}\n  method: get\n  operationId: getV1ReservationsId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reservations/{id}\n  method: patch\n  operationId: patchV1ReservationsId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/reservations/{id}/cancel\n  method: patch\n  operationId: patchV1ReservationsIdCancel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /v1/restaurants/{id}/availabilities\n  method: get\n  operationId: getV1RestaurantsIdAvailabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/restaurants/{id}/availabilities/override\n  method: put\n  operationId: putV1RestaurantsIdAvailabilitiesOverride\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/restaurants/{id}/customers/phone/{phoneNumber}\n  method: get\n  operationId: getV1RestaurantsIdCustomersPhonePhoneNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/restaurants/{id}/offers\n\
  \  method: get\n  operationId: getV1RestaurantsIdOffers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/restaurants/{id}/partySizes\n  method: get\n  operationId: getV1RestaurantsIdPartySizes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/restaurants/{id}/reservations\n  method: post\n  operationId: postV1RestaurantsIdReservations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/restaurants/{id}/timeslots\n  method: get\n  operationId: getV1RestaurantsIdTimeslots\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reviews\n  method: get\n  operationId: getV1Reviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reviews/{id}\n  method: get\n  operationId: getV1ReviewsId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reviews/{id}/reply\n  method: put\n  operationId: putV1ReviewsIdReply\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/create\n  method: post\n  operationId: postV1Create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/orders/{orderUuid}\n  method: put\n  operationId: putV1OrdersOrderuuid\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/{posUuid}/logo\n  method: put\n  operationId: putV1PosuuidLogo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lafourchette/refs/heads/main/agentic-access/lafourchette-agentic-access.yml
summary_line: 21 operations · 10 acting · 1 human-in-the-loop
tags:
- Company
- Consumer
- Restaurant
- Reservations
- Booking
- Hospitality
- Point-of-Sale
- Reviews
- Marketplace
- Travel and Dining
- Webhook
- France
---
