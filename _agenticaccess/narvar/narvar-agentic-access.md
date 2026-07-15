---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 1
api_specs:
- filename: narvar-order-openapi.yml
  format: yaml
  label: Narvar Order API
  slug: narvar-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/narvar/refs/heads/main/openapi/narvar-order-openapi.yml
consequence_counts:
  physical: 2
  read: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Narvar Agentic Access
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
  method: PUT
  path: /orders/{OrderNumber}/shipments
operation_count: 3
overview: 'Narvar exposes 3 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Narvar
provider_slug: narvar
slug: narvar-agentic-access
source_filename: narvar-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/narvar-order-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 3\n  by_action_class:\n    acting: 2\n    connected: 1\n  by_consequence:\n    physical: 2\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /orders\n  method: post\n  operationId: PostCreateUpdateOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{OrderNumber}\n  method: get\n  operationId: GetRetrieveOrder\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{OrderNumber}/shipments\n  method: put\n  operationId: PutCreateUpdateShipments\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/narvar/refs/heads/main/agentic-access/narvar-agentic-access.yml
summary_line: 3 operations · 2 acting
tags:
- Post-Purchase
- Order Tracking
- Delivery Notifications
- Returns
- Exchanges
- Ecommerce
- Shipments
- Customer Experience
---
