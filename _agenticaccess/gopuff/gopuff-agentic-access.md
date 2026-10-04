---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 4
api_specs:
- filename: gopuff-availability-api-openapi.yml
  format: yaml
  label: Gopuff Availability API
  slug: gopuff-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gopuff/refs/heads/main/openapi/gopuff-availability-api-openapi.yml
- filename: gopuff-orders-api-openapi.yml
  format: yaml
  label: Gopuff Orders API
  slug: gopuff-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gopuff/refs/heads/main/openapi/gopuff-orders-api-openapi.yml
- filename: gopuff-rates-api-openapi.yml
  format: yaml
  label: Gopuff Rates API
  slug: gopuff-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gopuff/refs/heads/main/openapi/gopuff-rates-api-openapi.yml
- filename: gopuff-shops-api-openapi.yml
  format: yaml
  label: Gopuff Shops API
  slug: gopuff-shops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gopuff/refs/heads/main/openapi/gopuff-shops-api-openapi.yml
- filename: gopuff-zones-api-openapi.yml
  format: yaml
  label: Gopuff Zones API
  slug: gopuff-zones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gopuff/refs/heads/main/openapi/gopuff-zones-api-openapi.yml
consequence_counts:
  physical: 1
  read: 4
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Gopuff Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /shops/orders
operation_count: 6
overview: 'Gopuff exposes 6 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read, 1 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Gopuff
provider_slug: gopuff
slug: gopuff-agentic-access
source_filename: gopuff-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/gopuff-availability-api-openapi.yml, openapi/gopuff-orders-api-openapi.yml,\n  openapi/gopuff-rates-api-openapi.yml, openapi/gopuff-shops-api-openapi.yml, openapi/gopuff-zones-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 4\n    acting: 2\n  by_consequence:\n    read: 4\n    physical: 1\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /shops/availability\n  method: post\n  operationId: getProductAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shops/orders\n  method: post\n  operationId: createOrder\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shops/orders/{order_id}\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shops/rates\n  method: post\n  operationId: getCarrierRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shops\n  method: get\n  operationId: getShop\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shops/zones/check\n \
  \ method: post\n  operationId: checkDeliveryZone\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gopuff/refs/heads/main/agentic-access/gopuff-agentic-access.yml
summary_line: 6 operations · 2 acting
tags:
- Quick Commerce
- Instant Delivery
- Last Mile Delivery
- Grocery
- Fulfillment
- Retail
- Logistics
---
