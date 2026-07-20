---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 7
api_specs:
- filename: einride-auth-openapi-original.yml
  format: yaml
  label: 'Einride Extend: Authentication API'
  slug: einride-extend-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/einride/refs/heads/main/openapi/einride-auth-openapi-original.yml
- filename: einride-book-openapi-original.yml
  format: yaml
  label: 'Einride Extend: Shipment & Booking API'
  slug: einride-extend-shipment-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/einride/refs/heads/main/openapi/einride-book-openapi-original.yml
consequence_counts:
  physical: 4
  read: 7
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Einride Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1beta1/{shipment.name}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1beta1/{shipment}:cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1beta1/{shipment}:release
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1beta1/{space}/shipments
operation_count: 14
overview: 'Einride exposes 14 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read, 3 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Einride
provider_slug: einride
slug: einride-agentic-access
source_filename: einride-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/einride-auth-openapi-original.yml, openapi/einride-book-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    acting: 7\n    connected: 7\n  by_consequence:\n    write: 3\n    read: 7\n    physical: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /v1beta1/auth:exchangeSecret\n  method: post\n  operationId: AuthenticationService_ExchangeSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1beta1/{parent}/shipments\n\
  \  method: get\n  operationId: ShipmentService_ListShipments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1beta1/{parent}/tours\n  method: get\n  operationId: BookingService_ListTours\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1beta1/{parent}/tours:search\n  method: get\n  operationId: BookingService_SearchTours\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1beta1/{shipment.name}\n  method: patch\n  operationId: ShipmentService_UpdateShipment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1beta1/{shipment}\n  method: get\n  operationId: ShipmentService_GetShipment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1beta1/{shipment}:cancel\n  method: post\n  operationId: ShipmentService_CancelShipment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1beta1/{shipment}:release\n  method: post\n  operationId: ShipmentService_ReleaseShipment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1beta1/{space}/shipments\n  method: post\n  operationId: ShipmentService_CreateShipment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1beta1/{space}/tours\n  method: post\n  operationId: BookingService_CreateTour\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v1beta1/{tour.name}\n  method: patch\n  operationId: BookingService_UpdateTour\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1beta1/{tour}\n  method: get\n  operationId: BookingService_GetTour\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1beta1/{tour}:cancel\n  method: get\n  operationId: BookingService_CancelTour\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1beta1/{tour}:confirm\n  method: get\n  operationId: BookingService_ConfirmTour\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/einride/refs/heads/main/agentic-access/einride-agentic-access.yml
summary_line: 14 operations · 7 acting
tags:
- Company
- Sustainable Transport
- Freight
- Logistics
- Autonomous Vehicles
- Electric Vehicles
- Shipping
- gRPC
---
