---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 10
api_specs:
- filename: sendle-orders-api-openapi.yml
  format: yaml
  label: Sendle Orders API
  slug: sendle-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendle/refs/heads/main/openapi/sendle-orders-api-openapi.yml
- filename: sendle-products-api-openapi.yml
  format: yaml
  label: Sendle Products & Quoting API
  slug: sendle-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendle/refs/heads/main/openapi/sendle-products-api-openapi.yml
- filename: sendle-tracking-api-openapi.yml
  format: yaml
  label: Sendle Tracking API
  slug: sendle-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendle/refs/heads/main/openapi/sendle-tracking-api-openapi.yml
- filename: sendle-manifests-api-openapi.yml
  format: yaml
  label: Sendle Shipping Manifests API
  slug: sendle-manifests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendle/refs/heads/main/openapi/sendle-manifests-api-openapi.yml
- filename: sendle-ping-api-openapi.yml
  format: yaml
  label: Sendle Ping API
  slug: sendle-ping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendle/refs/heads/main/openapi/sendle-ping-api-openapi.yml
consequence_counts:
  physical: 4
  read: 10
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sendle Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /manifests
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/{id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/{id}/return
operation_count: 17
overview: 'Sendle exposes 17 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read, 3 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Sendle
provider_slug: sendle
slug: sendle-agentic-access
source_filename: sendle-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/sendle-manifests-api-openapi.yml, openapi/sendle-orders-api-openapi.yml, openapi/sendle-ping-api-openapi.yml,\n  openapi/sendle-products-api-openapi.yml, openapi/sendle-tracking-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    acting: 7\n    connected: 10\n  by_consequence:\n    physical: 4\n    read: 10\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /manifests\n  method: post\n  operationId: createShippingManifest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /manifests\n  method: get\n  operationId: getShippingManifests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /manifests/{id}/download\n  method: get\n  operationId: downloadShippingManifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /manifests/{id}/orders\n  method: get\n  operationId: getShippingManifestOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /manifests/{id}/status\n  method: get\n  operationId: getShippingManifestStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /orders\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{id}\n  method: get\n  operationId: viewOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{id}/cancel\n  method: post\n  operationId: cancelOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /orders/{id}/return\n  method: post\n  operationId: returnOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{id}/return\n  method: get\n  operationId: viewReturnOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ping\n  method: get\n  operationId: ping\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products\n  method: get\n  operationId: getProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products\n  method: post\n  operationId: postProducts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /quote\n  method: get\n  operationId: getQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /parcels/{ref}/tracking\n  method: get\n  operationId: trackParcel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /parcels/{ref}/tracking/subscribe\n  method: post\n  operationId: subscribeToTrackingEvents\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /parcels/{ref}/tracking/subscribe\n  method: delete\n  operationId: unsubscribeFromTrackingEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sendle/refs/heads/main/agentic-access/sendle-agentic-access.yml
summary_line: 17 operations · 7 acting
tags:
- Shipping
- Logistics
- Last Mile
- Parcels
- E-commerce
- Carbon Neutral
- Small Business
- Australia
- United States
- Canada
---
