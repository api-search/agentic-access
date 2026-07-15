---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 6
api_specs:
- filename: ninjavan-openapi.yml
  format: yaml
  label: Ninja Van OAuth API
  slug: ninjavan-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ninjavan/refs/heads/main/openapi/ninjavan-openapi.yml
- filename: ninjavan-openapi.yml
  format: yaml
  label: Ninja Van Order API
  slug: ninjavan-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ninjavan/refs/heads/main/openapi/ninjavan-openapi.yml
- filename: ninjavan-openapi.yml
  format: yaml
  label: Ninja Van Tracking API
  slug: ninjavan-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ninjavan/refs/heads/main/openapi/ninjavan-openapi.yml
- filename: ninjavan-openapi.yml
  format: yaml
  label: Ninja Van Webhooks API
  slug: ninjavan-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ninjavan/refs/heads/main/openapi/ninjavan-openapi.yml
- filename: ninjavan-openapi.yml
  format: yaml
  label: Ninja Van Tariff API
  slug: ninjavan-tariff-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ninjavan/refs/heads/main/openapi/ninjavan-openapi.yml
- filename: ninjavan-openapi.yml
  format: yaml
  label: Ninja Van PUDO API
  slug: ninjavan-pudo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ninjavan/refs/heads/main/openapi/ninjavan-openapi.yml
consequence_counts:
  physical: 4
  read: 6
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ninjavan Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /1.0/send-orders/drop-off
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /2.2/orders/{trackingNo}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /4.1/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /4.2/orders
operation_count: 12
overview: 'Ninja Van exposes 12 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 2 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Ninja Van
provider_slug: ninjavan
slug: ninjavan-agentic-access
source_filename: ninjavan-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/ninjavan-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    acting: 6\n    connected: 6\n  by_consequence:\n    write: 2\n    physical: 4\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /2.0/oauth/access_token\n  method: post\n  operationId: requestAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /4.2/orders\n  method: post\n  operationId: createOrderV42\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /4.1/orders\n  method: post\n  operationId: createOrderV41\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2.2/orders/{trackingNo}\n  method: delete\n  operationId: cancelOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2.0/reports/waybill\n  method: get\n  operationId: generateWaybill\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2.0/reports/international-waybills\n  method: get\n  operationId: generateInternationalWaybill\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1.0/public/price\n  method: post\n  operationId: getPriceEstimate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2.0/pudos\n  method: get\n  operationId: listNinjaPoints\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1.0/send-orders/drop-off\n  method: post\n  operationId: triggerShipperDropOff\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /1.0/send-orders/{trackingId}\n  method: get\n  operationId: scanParcelForDropOff\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1.0/orders/tracking-events/{trackingNumber}\n  method: get\n  operationId: getTrackingEventsForParcel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /1.0/orders/tracking-events\n  method: get\n  operationId: getTrackingEventsForParcels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ninjavan/refs/heads/main/agentic-access/ninjavan-agentic-access.yml
summary_line: 12 operations · 6 acting
tags:
- Logistics
- Last-Mile Delivery
- Shipping
- Southeast Asia
- Parcels
- Tracking
- Fulfillment
- E-commerce Logistics
- Waybill
- SaaS
---
