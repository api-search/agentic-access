---
acting_count: 11
action_class_counts:
  acting: 11
api_specs:
- filename: cloudprinter-openapi.yml
  format: yaml
  label: Cloudprinter Orders API
  slug: cloudprinter-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudprinter/refs/heads/main/openapi/cloudprinter-openapi.yml
- filename: cloudprinter-openapi.yml
  format: yaml
  label: Cloudprinter Products & Pricing API
  slug: cloudprinter-products-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudprinter/refs/heads/main/openapi/cloudprinter-openapi.yml
- filename: cloudprinter-openapi.yml
  format: yaml
  label: Cloudprinter Quotes API
  slug: cloudprinter-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudprinter/refs/heads/main/openapi/cloudprinter-openapi.yml
- filename: cloudprinter-openapi.yml
  format: yaml
  label: Cloudprinter Signal Webhooks API
  slug: cloudprinter-signal-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudprinter/refs/heads/main/openapi/cloudprinter-openapi.yml
- filename: cloudprinter-openapi.yml
  format: yaml
  label: Cloudprinter Files API
  slug: cloudprinter-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudprinter/refs/heads/main/openapi/cloudprinter-openapi.yml
consequence_counts:
  physical: 9
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cloudprinter Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/add
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/info
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/log
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/quote
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /shipping/countries
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /shipping/levels
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /shipping/states
operation_count: 11
overview: 'Cloudprinter exposes 11 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 write and 9 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cloudprinter
provider_slug: cloudprinter
slug: cloudprinter-agentic-access
source_filename: cloudprinter-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/cloudprinter-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    acting: 11\n  by_consequence:\n    physical: 9\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /orders/\n  method: post\n  operationId: listOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/info\n  method: post\n  operationId: getOrderInfo\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/add\n  method: post\n  operationId: addOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/cancel\n  method: post\n  operationId: cancelOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/log\n  method: post\n  operationId: getOrderLog\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/quote\n  method: post\n  operationId: getOrderQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /products\n  method: post\n  operationId: listProducts\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /products/info\n  method: post\n  operationId: getProductInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shipping/levels\n  method: post\n  operationId: getShippingLevels\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shipping/countries\n\
  \  method: post\n  operationId: getShippingCountries\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shipping/states\n  method: post\n  operationId: getShippingStates\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudprinter/refs/heads/main/agentic-access/cloudprinter-agentic-access.yml
summary_line: 11 operations · 11 acting
tags:
- Print on Demand
- Print Fulfillment
- Printing
- Orders
- Logistics
---
