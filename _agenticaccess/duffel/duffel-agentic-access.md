---
acting_count: 21
action_class_counts:
  acting: 21
  connected: 18
api_specs:
- filename: duffel-openapi.yml
  format: yaml
  label: Duffel Offer Requests API
  slug: duffel-offer-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duffel/refs/heads/main/openapi/duffel-openapi.yml
- filename: duffel-openapi.yml
  format: yaml
  label: Duffel Offers API
  slug: duffel-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duffel/refs/heads/main/openapi/duffel-openapi.yml
- filename: duffel-openapi.yml
  format: yaml
  label: Duffel Orders API
  slug: duffel-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duffel/refs/heads/main/openapi/duffel-openapi.yml
- filename: duffel-openapi.yml
  format: yaml
  label: Duffel Seat Maps API
  slug: duffel-seat-maps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duffel/refs/heads/main/openapi/duffel-openapi.yml
- filename: duffel-openapi.yml
  format: yaml
  label: Duffel Order Changes API
  slug: duffel-order-changes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duffel/refs/heads/main/openapi/duffel-openapi.yml
- filename: duffel-openapi.yml
  format: yaml
  label: Duffel Order Cancellations API
  slug: duffel-order-cancellations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duffel/refs/heads/main/openapi/duffel-openapi.yml
- filename: duffel-openapi.yml
  format: yaml
  label: Duffel Payments API
  slug: duffel-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duffel/refs/heads/main/openapi/duffel-openapi.yml
- filename: duffel-openapi.yml
  format: yaml
  label: Duffel Stays API
  slug: duffel-stays-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duffel/refs/heads/main/openapi/duffel-openapi.yml
- filename: duffel-openapi.yml
  format: yaml
  label: Duffel Webhooks API
  slug: duffel-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duffel/refs/heads/main/openapi/duffel-openapi.yml
consequence_counts:
  physical: 9
  read: 18
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Duffel Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /air/order_cancellations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /air/order_cancellations/{id}/actions/confirm
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /air/order_change_requests
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /air/order_changes
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /air/order_changes/{id}/actions/confirm
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /air/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /air/orders/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /air/orders/{id}/services
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /air/payments
operation_count: 39
overview: 'Duffel exposes 39 API operations that an AI agent could call, of which 21 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read, 12 write, and 9 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Duffel
provider_slug: duffel
slug: duffel-agentic-access
source_filename: duffel-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/duffel-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 39\n  by_action_class:\n    acting: 21\n    connected: 18\n  by_consequence:\n    write: 12\n    read: 18\n    physical: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /air/offer_requests\n  method: post\n  operationId: createOfferRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /air/offer_requests\n  method: get\n  operationId: listOfferRequests\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /air/offer_requests/{id}\n  method: get\n  operationId: getOfferRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /air/offers\n  method: get\n  operationId: listOffers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /air/offers/{id}\n  method: get\n  operationId: getOffer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /air/offers/{id}/actions/price\n  method: post\n  operationId: priceOffer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /air/offers/{offer_id}/passengers/{offer_passenger_id}\n  method: patch\n  operationId: updateOfferPassenger\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /air/orders\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /air/orders\n  method: get\n  operationId: listOrders\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /air/orders/{id}\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /air/orders/{id}\n  method: patch\n  operationId: updateOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /air/orders/{id}/available_services\n  method: get\n  operationId: listAvailableServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /air/orders/{id}/services\n\
  \  method: post\n  operationId: addServiceToOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /air/order_change_requests\n  method: post\n  operationId: createOrderChangeRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /air/order_change_requests/{id}\n  method: get\n  operationId: getOrderChangeRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n \
  \   token:\n      max-ttl: 3600\n    audit: none\n- path: /air/order_changes\n  method: post\n  operationId: createOrderChange\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /air/order_changes/{id}\n  method: get\n  operationId: getOrderChange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /air/order_changes/{id}/actions/confirm\n  method: post\n  operationId: confirmOrderChange\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /air/order_cancellations\n  method: post\n  operationId: createOrderCancellation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /air/order_cancellations\n  method: get\n  operationId: listOrderCancellations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /air/order_cancellations/{id}\n  method: get\n  operationId: getOrderCancellation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /air/order_cancellations/{id}/actions/confirm\n  method: post\n  operationId: confirmOrderCancellation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /air/payments\n  method: post\n  operationId: createPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /air/payments\n  method: get\n  operationId: listPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /air/payments/{id}\n  method: get\n  operationId: getPayment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /air/seat_maps\n  method: get\n  operationId: getSeatMaps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /air/webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /air/webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /air/webhooks/{id}\n  method: patch\n  operationId: updateWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /air/webhooks/{id}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /air/webhooks/{id}/actions/ping\n  method: post\n  operationId: pingWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stays/search\n  method: post\n  operationId: searchStays\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stays/search_results/{id}/actions/fetch_all_rates\n  method: post\n  operationId: fetchAllRates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stays/quotes\n  method: post\n  operationId: createStaysQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stays/quotes/{id}\n  method: get\n  operationId: getStaysQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stays/bookings\n  method: post\n  operationId: createStaysBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stays/bookings\n  method: get\n  operationId: listStaysBookings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stays/bookings/{id}\n\
  \  method: get\n  operationId: getStaysBooking\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stays/bookings/{id}/actions/cancel\n  method: post\n  operationId: cancelStaysBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/duffel/refs/heads/main/agentic-access/duffel-agentic-access.yml
summary_line: 39 operations · 21 acting
tags:
- Travel
- Flights
- Hotels
- Booking
- Payments
---
