---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 8
api_specs:
- filename: bitrefill-account-api-openapi.yml
  format: yaml
  label: Bitrefill Account API
  slug: bitrefill-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitrefill/openapi/bitrefill-account-api-openapi.yml
- filename: bitrefill-checkout-api-openapi.yml
  format: yaml
  label: Bitrefill Checkout API
  slug: bitrefill-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitrefill/openapi/bitrefill-checkout-api-openapi.yml
- filename: bitrefill-discovery-api-openapi.yml
  format: yaml
  label: Bitrefill Discovery API
  slug: bitrefill-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitrefill/openapi/bitrefill-discovery-api-openapi.yml
- filename: bitrefill-payments-api-openapi.yml
  format: yaml
  label: Bitrefill Payments API
  slug: bitrefill-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bitrefill/openapi/bitrefill-payments-api-openapi.yml
consequence_counts:
  physical: 2
  read: 8
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bitrefill Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /x402/invoice/create
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /x402/invoice/pay
operation_count: 11
overview: 'Bitrefill exposes 11 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 1 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bitrefill
provider_slug: bitrefill
slug: bitrefill-agentic-access
source_filename: bitrefill-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/bitrefill-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 8\n    acting: 3\n  by_consequence:\n    read: 8\n    physical: 2\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /x402/checkout/info\n  method: get\n  operationId: getCheckoutInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /x402/gift-cards/search\n  method: get\n  operationId: searchGiftCards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /x402/esims/search\n  method: get\n  operationId: searchEsims\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /x402/topups/search\n  method: get\n  operationId: searchTopups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /x402/products/detail\n  method: get\n  operationId: getProductDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /x402/invoice/create\n  method: post\n  operationId: createInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /x402/invoice/pay\n  method: post\n  operationId: payInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /x402/invoice/status\n  method: get\n  operationId: getInvoiceStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /x402/connect\n  method: post\n  operationId: connectWallet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /x402/my/orders\n  method: get\n  operationId: listMyOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /x402/my/esims\n  method: get\n  operationId: listMyEsims\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/bitrefill/agentic-access/bitrefill-agentic-access.yml
summary_line: 11 operations · 3 acting
tags:
- Company
- Cryptocurrency
- Payments
- Gift Cards
- Mobile Top-Up
---
