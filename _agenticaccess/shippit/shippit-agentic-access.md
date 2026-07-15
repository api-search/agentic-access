---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 5
api_specs:
- filename: shippit-openapi.yml
  format: yaml
  label: Shippit Quote API
  slug: shippit-quote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippit/refs/heads/main/openapi/shippit-openapi.yml
- filename: shippit-openapi.yml
  format: yaml
  label: Shippit Orders API
  slug: shippit-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippit/refs/heads/main/openapi/shippit-openapi.yml
- filename: shippit-openapi.yml
  format: yaml
  label: Shippit Book API
  slug: shippit-book-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippit/refs/heads/main/openapi/shippit-openapi.yml
- filename: shippit-openapi.yml
  format: yaml
  label: Shippit Label API
  slug: shippit-label-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippit/refs/heads/main/openapi/shippit-openapi.yml
- filename: shippit-openapi.yml
  format: yaml
  label: Shippit Tracking API
  slug: shippit-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippit/refs/heads/main/openapi/shippit-openapi.yml
- filename: shippit-openapi.yml
  format: yaml
  label: Shippit Merchant API
  slug: shippit-merchant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippit/refs/heads/main/openapi/shippit-openapi.yml
consequence_counts:
  physical: 4
  read: 5
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Shippit Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /book
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /orders/{tracking_number}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /quote
operation_count: 10
overview: 'Shippit exposes 10 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read, 1 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Shippit
provider_slug: shippit
slug: shippit-agentic-access
source_filename: shippit-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/shippit-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    acting: 5\n    connected: 5\n  by_consequence:\n    physical: 4\n    read: 5\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /quote\n  method: post\n  operationId: createQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /order\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{tracking_number}\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{tracking_number}\n  method: delete\n  operationId: cancelOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{tracking_number}/tracking\n  method:\
  \ get\n  operationId: getOrderTracking\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /book\n  method: post\n  operationId: bookOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /label/{tracking_number}\n  method: get\n  operationId: getLabel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchant\n  method: get\n  operationId: getMerchant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /merchant\n  method: put\n  operationId: updateMerchant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /merchant/operating-hours\n  method: get\n  operationId: getOperatingHours\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shippit/refs/heads/main/agentic-access/shippit-agentic-access.yml
summary_line: 10 operations · 5 acting
tags:
- Shipping
- Logistics
- Fulfillment
- Australia
- APAC
- Multi-Carrier
- Labels
- Tracking
- Parcels
- E-commerce Logistics
- SaaS
---
