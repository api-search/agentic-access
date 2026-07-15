---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 10
api_specs:
- filename: extensiv-openapi.yml
  format: yaml
  label: Extensiv Orders API
  slug: extensiv-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extensiv/refs/heads/main/openapi/extensiv-openapi.yml
- filename: extensiv-openapi.yml
  format: yaml
  label: Extensiv Inventory API
  slug: extensiv-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extensiv/refs/heads/main/openapi/extensiv-openapi.yml
- filename: extensiv-openapi.yml
  format: yaml
  label: Extensiv Items API
  slug: extensiv-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extensiv/refs/heads/main/openapi/extensiv-openapi.yml
- filename: extensiv-openapi.yml
  format: yaml
  label: Extensiv Customers API
  slug: extensiv-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extensiv/refs/heads/main/openapi/extensiv-openapi.yml
- filename: extensiv-openapi.yml
  format: yaml
  label: Extensiv Receivers (ASN) API
  slug: extensiv-receivers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extensiv/refs/heads/main/openapi/extensiv-openapi.yml
- filename: extensiv-openapi.yml
  format: yaml
  label: Extensiv Warehouses API
  slug: extensiv-warehouses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extensiv/refs/heads/main/openapi/extensiv-openapi.yml
- filename: extensiv-openapi.yml
  format: yaml
  label: Extensiv Auth Token API
  slug: extensiv-auth-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extensiv/refs/heads/main/openapi/extensiv-openapi.yml
consequence_counts:
  physical: 2
  read: 10
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Extensiv Agentic Access
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
  path: /orders/{orderId}
operation_count: 14
overview: 'Extensiv exposes 14 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read, 2 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Extensiv
provider_slug: extensiv
slug: extensiv-agentic-access
source_filename: extensiv-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/extensiv-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    acting: 4\n    connected: 10\n  by_consequence:\n    write: 2\n    read: 10\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /AuthServer/api/Token\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n \
  \   token:\n      max-ttl: 3600\n    audit: none\n- path: /orders\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{orderId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{orderId}\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inventory\n  method:\
  \ get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inventory/stockSummaries\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customerId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customerId}/items\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inventory/receivers\n  method: get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inventory/receivers\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inventory/receivers/{receiverId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /facilities\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/extensiv/refs/heads/main/agentic-access/extensiv-agentic-access.yml
summary_line: 14 operations · 4 acting
tags:
- 3PL
- Warehouse Management
- WMS
- Order Management
- Inventory Management
- Fulfillment
- Logistics
- Supply Chain
---
