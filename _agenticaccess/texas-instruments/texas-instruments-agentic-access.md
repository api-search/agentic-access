---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 7
api_specs:
- filename: texas-instruments-store-openapi.yml
  format: yaml
  label: Texas Instruments Store API
  slug: ti-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/texas-instruments/refs/heads/main/openapi/texas-instruments-store-openapi.yml
- filename: texas-instruments-product-information-openapi.yml
  format: yaml
  label: Texas Instruments Product Information API
  slug: ti-product-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/texas-instruments/refs/heads/main/openapi/texas-instruments-product-information-openapi.yml
consequence_counts:
  physical: 1
  read: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Texas Instruments Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders
operation_count: 8
overview: 'Texas Instruments exposes 8 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Texas Instruments
provider_slug: texas-instruments
slug: texas-instruments-agentic-access
source_filename: texas-instruments-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/texas-instruments-product-information-openapi.yml, openapi/texas-instruments-store-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 7\n    acting: 1\n  by_consequence:\n    read: 7\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /products/{partNumber}\n  method: get\n  operationId: getProductInformation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products-extended/{partNumber}\n  method: get\n  operationId: getProductInformationOrchestrated\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/{partNumber}\n  method: get\n  operationId: getProductInventoryAndPricing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/catalog\n  method: get\n  operationId: getProductCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{orderNumber}\n  method: get\n  operationId: getOrder\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /advanced-ship-notices\n  method: get\n  operationId: getAdvancedShipNotices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /financial-documents\n  method: get\n  operationId: getFinancialDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/texas-instruments/refs/heads/main/agentic-access/texas-instruments-agentic-access.yml
summary_line: 8 operations · 1 acting
tags:
- Electronics
- Ordering
- Semiconductors
- Supply Chain
- Fortune 500
---
