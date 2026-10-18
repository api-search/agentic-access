---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 15
api_specs:
- filename: thefork-customers-api-openapi.yml
  format: yaml
  label: TheFork Customers API
  slug: thefork-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thefork/refs/heads/main/openapi/thefork-customers-api-openapi.yml
- filename: thefork-orders-api-openapi.yml
  format: yaml
  label: TheFork Orders API
  slug: thefork-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thefork/refs/heads/main/openapi/thefork-orders-api-openapi.yml
- filename: thefork-reservations-api-openapi.yml
  format: yaml
  label: TheFork Reservations API
  slug: thefork-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thefork/refs/heads/main/openapi/thefork-reservations-api-openapi.yml
- filename: thefork-reviews-api-openapi.yml
  format: yaml
  label: TheFork Reviews API
  slug: thefork-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thefork/refs/heads/main/openapi/thefork-reviews-api-openapi.yml
- filename: thefork-booking-flow-api-openapi.yml
  format: yaml
  label: TheFork Booking flow API
  slug: thefork-booking-flow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thefork/refs/heads/main/openapi/thefork-booking-flow-api-openapi.yml
- filename: thefork-create-api-openapi.yml
  format: yaml
  label: TheFork Create API
  slug: thefork-create-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thefork/refs/heads/main/openapi/thefork-create-api-openapi.yml
- filename: thefork-data-api-openapi.yml
  format: yaml
  label: TheFork Data API
  slug: thefork-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thefork/refs/heads/main/openapi/thefork-data-api-openapi.yml
- filename: thefork-logo-api-openapi.yml
  format: yaml
  label: TheFork Logo API
  slug: thefork-logo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thefork/refs/heads/main/openapi/thefork-logo-api-openapi.yml
- filename: thefork-phone-api-openapi.yml
  format: yaml
  label: TheFork Phone API
  slug: thefork-phone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thefork/refs/heads/main/openapi/thefork-phone-api-openapi.yml
- filename: thefork-review-flow-api-openapi.yml
  format: yaml
  label: TheFork Review flow API
  slug: thefork-review-flow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thefork/refs/heads/main/openapi/thefork-review-flow-api-openapi.yml
consequence_counts:
  physical: 3
  read: 15
  safety-critical: 1
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Thefork Agentic Access
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
  method: POST
  path: /orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/{orderId}/close
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/orders/{orderUuid}
operation_count: 29
overview: 'TheFork exposes 29 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read, 10 write, 3 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: TheFork
provider_slug: thefork
slug: thefork-agentic-access
source_filename: thefork-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-24'\nmethod: generated\nsource: openapi/lafourchette-booking-flow-api-openapi.yml, openapi/lafourchette-data-api-openapi.yml,\n  openapi/lafourchette-phone-api-openapi.yml, openapi/lafourchette-review-flow-api-openapi.yml,\n  openapi/lafourchette-v1-api-openapi.yml, openapi/thefork-customers-api-openapi.yml, openapi/thefork-orders-api-openapi.yml,\n  openapi/thefork-reservations-api-openapi.yml, openapi/thefork-reviews-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 29\n  by_action_class:\n    acting: 14\n    connected: 15\n  by_consequence:\n    write: 10\n    read: 15\n    safety-critical: 1\n    physical: 3\n  human_in_the_loop_required: 1\noperations:\n- path: /v1/reservations/{id}\n  method: patch\n \
  \ operationId: patchV1ReservationsId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/reservations/{id}/cancel\n  method: patch\n  operationId: patchV1ReservationsIdCancel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/restaurants/{id}/availabilities\n  method: get\n  operationId: getV1RestaurantsIdAvailabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/restaurants/{id}/availabilities/override\n\
  \  method: put\n  operationId: putV1RestaurantsIdAvailabilitiesOverride\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/restaurants/{id}/offers\n  method: get\n  operationId: getV1RestaurantsIdOffers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/restaurants/{id}/partySizes\n  method: get\n  operationId: getV1RestaurantsIdPartySizes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/restaurants/{id}/reservations\n  method: post\n  operationId: postV1RestaurantsIdReservations\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/restaurants/{id}/timeslots\n  method: get\n  operationId: getV1RestaurantsIdTimeslots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customers\n  method: get\n  operationId: getV1Customers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customers/{id}\n  method: get\n  operationId: getV1CustomersId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reservations\n  method: get\n  operationId: getV1Reservations\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reservations/{id}\n  method: get\n  operationId: getV1ReservationsId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/callCenter/callRecognitions\n  method: post\n  operationId: postV1CallCenterCallRecognitions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/integrationStatus\n  method: patch\n  operationId: patchV1IntegrationStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/restaurants/{id}/customers/phone/{phoneNumber}\n  method: get\n  operationId: getV1RestaurantsIdCustomersPhonePhoneNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reviews\n  method: get\n  operationId: getV1Reviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reviews/{id}\n  method: get\n  operationId: getV1ReviewsId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reviews/{id}/reply\n  method: put\n  operationId: putV1ReviewsIdReply\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/create\n  method: post\n  operationId: postV1Create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/orders/{orderUuid}\n  method: put\n  operationId: putV1OrdersOrderuuid\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/{posUuid}/logo\n  method: put\n  operationId:\
  \ putV1PosuuidLogo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restaurants/{id}/customers/phone/{phoneNumber}\n  method: get\n  operationId: findCustomerByPhone\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers\n  method: get\n  operationId: listCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders\n  method: post\n  operationId: openOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{orderId}/close\n  method: post\n  operationId: closeOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restaurants/{id}/reservations\n  method: post\n  operationId: createReservation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reservations/{id}\n  method: get\n  operationId: getReservation\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reservations/{id}\n  method: patch\n  operationId: updateReservation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reviews/{id}\n  method: get\n  operationId: getReview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thefork/refs/heads/main/agentic-access/thefork-agentic-access.yml
summary_line: 29 operations · 14 acting · 1 human-in-the-loop
tags:
- Restaurant
- Reservations
- Booking
- Dining
- Point-of-Sale
- Marketplace
---
