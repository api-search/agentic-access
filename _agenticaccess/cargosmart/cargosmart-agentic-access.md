---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 7
api_specs:
- filename: cargosmart-shipment-tracking-openapi.yml
  format: yaml
  label: CargoSmart Container Booking API
  slug: cargosmart-container-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargosmart/refs/heads/main/openapi/cargosmart-shipment-tracking-openapi.yml
- filename: cargosmart-shipment-tracking-openapi.yml
  format: yaml
  label: CargoSmart Shipment Tracking API
  slug: cargosmart-shipment-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargosmart/refs/heads/main/openapi/cargosmart-shipment-tracking-openapi.yml
- filename: cargosmart-shipment-tracking-openapi.yml
  format: yaml
  label: CargoSmart Vessel Schedule API
  slug: cargosmart-vessel-schedule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargosmart/refs/heads/main/openapi/cargosmart-shipment-tracking-openapi.yml
- filename: cargosmart-shipment-tracking-openapi.yml
  format: yaml
  label: CargoSmart Shipping Documentation API
  slug: cargosmart-shipping-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargosmart/refs/heads/main/openapi/cargosmart-shipment-tracking-openapi.yml
consequence_counts:
  read: 7
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cargosmart Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'CargoSmart exposes 8 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CargoSmart
provider_slug: cargosmart
slug: cargosmart-agentic-access
source_filename: cargosmart-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/cargosmart-shipment-tracking-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 7\n    acting: 1\n  by_consequence:\n    read: 7\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /tracking/v1/containers/{containerId}\n  method: get\n  operationId: trackContainer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tracking/v1/containers\n  method: get\n  operationId: listContainerTracking\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /tracking/v1/shipments/{billOfLadingNumber}\n  method: get\n  operationId: getShipment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vessels/v1/schedules\n  method: get\n  operationId: searchVesselSchedules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vessels/v1/{vesselIMO}/position\n  method: get\n  operationId: getVesselPosition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bookings/v1\n  method: post\n  operationId: createBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n   \
  \   triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bookings/v1\n  method: get\n  operationId: listBookings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/v1/bills-of-lading/{blNumber}\n  method: get\n  operationId: getBillOfLading\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cargosmart/refs/heads/main/agentic-access/cargosmart-agentic-access.yml
summary_line: 8 operations · 1 acting
tags:
- Booking
- Container
- Documentation
- GSBN
- IQAX
- Logistics
- Maritime
- Ocean Freight
- Schedule
- Shipping
- Supply Chain
- Tracking
- Visibility
- Vessel
---
