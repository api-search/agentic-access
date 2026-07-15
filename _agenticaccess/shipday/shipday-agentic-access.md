---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 2
api_specs:
- filename: shipday-openapi.yml
  format: yaml
  label: Shipday Orders API
  slug: orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipday/refs/heads/main/openapi/shipday-openapi.yml
- filename: shipday-openapi.yml
  format: yaml
  label: Shipday Drivers / Carriers API
  slug: drivers-carriers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipday/refs/heads/main/openapi/shipday-openapi.yml
- filename: shipday-openapi.yml
  format: yaml
  label: Shipday Order Assignment API
  slug: order-assignment
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipday/refs/heads/main/openapi/shipday-openapi.yml
- filename: shipday-openapi.yml
  format: yaml
  label: Shipday On-Demand Delivery API
  slug: on-demand-delivery
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipday/refs/heads/main/openapi/shipday-openapi.yml
- filename: shipday-openapi.yml
  format: yaml
  label: Shipday Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipday/refs/heads/main/openapi/shipday-openapi.yml
consequence_counts:
  physical: 6
  read: 2
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Shipday Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /on-demand/assign
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /order/edit/{orderId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /orders/assign/{orderId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /orders/assign/{orderId}/{carrierId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /orders/{orderId}
operation_count: 11
overview: 'Shipday exposes 11 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read, 3 write, and 6 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Shipday
provider_slug: shipday
slug: shipday-agentic-access
source_filename: shipday-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/shipday-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 2\n    acting: 9\n  by_consequence:\n    read: 2\n    physical: 6\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /orders\n  method: get\n  operationId: retrieveActiveOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders\n  method: post\n  operationId: insertOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /order/edit/{orderId}\n  method: put\n  operationId: editOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{orderId}\n  method: delete\n  operationId: deleteOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /carriers\n  method: get\n  operationId: retrieveCarriers\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /carriers\n  method: post\n  operationId: addCarrier\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /carriers/{carrierId}\n  method: delete\n  operationId: deleteCarrier\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/assign/{orderId}/{carrierId}\n  method: put\n  operationId: assignOrderToCarrier\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/assign/{orderId}\n  method: delete\n  operationId: unassignOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /on-demand/availability\n  method: post\n  operationId: checkOnDemandAvailability\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /on-demand/assign\n  method: post\n  operationId: assignOnDemand\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shipday/refs/heads/main/agentic-access/shipday-agentic-access.yml
summary_line: 11 operations · 9 acting
tags:
- Delivery
- Logistics
- Last Mile
- Local Delivery
- Dispatch
---
