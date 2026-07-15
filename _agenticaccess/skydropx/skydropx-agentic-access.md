---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 18
api_specs:
- filename: skydropx-openapi.yml
  format: yaml
  label: Skydropx Quotations API
  slug: skydropx-quotations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydropx/refs/heads/main/openapi/skydropx-openapi.yml
- filename: skydropx-openapi.yml
  format: yaml
  label: Skydropx Shipments API
  slug: skydropx-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydropx/refs/heads/main/openapi/skydropx-openapi.yml
- filename: skydropx-openapi.yml
  format: yaml
  label: Skydropx Orders and Labels API
  slug: skydropx-orders-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydropx/refs/heads/main/openapi/skydropx-openapi.yml
- filename: skydropx-openapi.yml
  format: yaml
  label: Skydropx Pickups API
  slug: skydropx-pickups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydropx/refs/heads/main/openapi/skydropx-openapi.yml
- filename: skydropx-openapi.yml
  format: yaml
  label: Skydropx Address Templates API
  slug: skydropx-address-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydropx/refs/heads/main/openapi/skydropx-openapi.yml
- filename: skydropx-openapi.yml
  format: yaml
  label: Skydropx Tracking API
  slug: skydropx-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydropx/refs/heads/main/openapi/skydropx-openapi.yml
- filename: skydropx-openapi.yml
  format: yaml
  label: Skydropx Finance API
  slug: skydropx-finance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydropx/refs/heads/main/openapi/skydropx-openapi.yml
- filename: skydropx-openapi.yml
  format: yaml
  label: Skydropx Catalog API
  slug: skydropx-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydropx/refs/heads/main/openapi/skydropx-openapi.yml
consequence_counts:
  physical: 6
  read: 18
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Skydropx Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /orders/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /shipments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /shipments/tracking
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /shipments/{id}/cancellations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /shipments/{id}/protect
operation_count: 32
overview: 'Skydropx exposes 32 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read, 8 write, and 6 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Skydropx
provider_slug: skydropx
slug: skydropx-agentic-access
source_filename: skydropx-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/skydropx-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 32\n  by_action_class:\n    acting: 14\n    connected: 18\n  by_consequence:\n    write: 8\n    read: 18\n    physical: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /oauth/token\n  method: post\n  operationId: createToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /quotations\n  method: post\n  operationId: createQuotation\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /quotations/{id}\n  method: get\n  operationId: getQuotation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shipments\n  method: get\n  operationId: listShipments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shipments\n  method: post\n  operationId: createShipment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n \
  \     - abnormal\n      - high-value\n    audit: required\n- path: /shipments/{id}\n  method: get\n  operationId: getShipment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shipments/{id}/cancellations\n  method: post\n  operationId: cancelShipment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shipments/{id}/protect\n  method: post\n  operationId: protectShipment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shipments/tracking/{tracking_number}\n  method: get\n  operationId: trackShipment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shipments/tracking\n  method: post\n  operationId: reportTrackingEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders\n  method: get\n  operationId: listOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders\n  method: post\n  operationId: createOrder\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{id}\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{id}\n  method: patch\n  operationId: updateOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{id}/labels\n  method: get\n  operationId: getOrderLabels\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pickups\n  method: get\n  operationId: listPickups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pickups\n  method: post\n  operationId: createPickup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pickups/{id}\n  method: get\n  operationId: getPickup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pickups/reschedule\n  method: post\n  operationId: reschedulePickup\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pickups/coverage\n  method: get\n  operationId: getPickupCoverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /address_templates\n  method: get\n  operationId: listAddressTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /address_templates\n  method: post\n  operationId: createAddressTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /address_templates/{id}\n  method: get\n  operationId: getAddressTemplate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /address_templates/{id}\n  method: patch\n  operationId: updateAddressTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /address_templates/{id}\n  method: delete\n  operationId: deleteAddressTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /address_templates/{id}/verify_by_carriers\n  method: post\n  operationId: verifyAddressByCarriers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /finance/credits\n  method: get\n  operationId: getCredits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /finance/extra-charges\n  method: get\n  operationId: listExtraCharges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shipments/carrier_services\n  method: get\n  operationId: listCarrierServices\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shipments/packagings\n  method: get\n  operationId: listPackagings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shipments/consignment_notes\n  method: get\n  operationId: listConsignmentNotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /office_points\n  method: get\n  operationId: listOfficePoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skydropx/refs/heads/main/agentic-access/skydropx-agentic-access.yml
summary_line: 32 operations · 14 acting
tags:
- Shipping
- Logistics
- Multi-Carrier
- Mexico
- Latin America
- Labels
- Rates
- Parcels
- Tracking
- Fulfillment
- SaaS
---
