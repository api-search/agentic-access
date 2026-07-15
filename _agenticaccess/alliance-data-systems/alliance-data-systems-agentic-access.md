---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 6
api_specs:
- filename: bread-pay-platform-openapi.yml
  format: yaml
  label: Bread Pay Platform API
  slug: bread-pay-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alliance-data-systems/refs/heads/main/openapi/bread-pay-platform-openapi.yml
- filename: bread-classic-merchant-openapi.yml
  format: yaml
  label: Bread Classic Merchant API
  slug: bread-classic-merchant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alliance-data-systems/refs/heads/main/openapi/bread-classic-merchant-openapi.yml
consequence_counts:
  physical: 2
  read: 6
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Alliance Data Systems Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transaction/{transactionID}/refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transactions/{transactionID}/shipping
operation_count: 14
overview: 'Alliance Data Systems (Bread Financial Holdings) exposes 14 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 6 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Alliance Data Systems (Bread Financial Holdings)
provider_slug: alliance-data-systems
slug: alliance-data-systems-agentic-access
source_filename: alliance-data-systems-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/bread-classic-merchant-openapi.yml, openapi/bread-pay-platform-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    acting: 8\n    connected: 6\n  by_consequence:\n    write: 6\n    read: 6\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /carts\n  method: post\n  operationId: createCart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /carts/{cartID}\n  method: get\n  operationId: getCart\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/{transactionID}\n  method: get\n  operationId: getTransactionClassic\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/{transactionID}\n  method: put\n  operationId: updateTransactionClassic\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transactions/{transactionID}/shipping\n  method: post\n  operationId: addTransactionShipping\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transactions/{transactionID}/shipping\n  method: get\n  operationId: getTransactionShipping\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /buyer/{id}\n  method: get\n  operationId: getBuyer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transaction\n  method: post\n  operationId: createTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /transaction/{transactionID}\n  method: get\n  operationId: getTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transaction/{transactionID}/authorize\n  method: post\n  operationId: authorizeTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction/{transactionID}/cancel\n  method: post\n  operationId: cancelTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction/{transactionID}/settle\n\
  \  method: post\n  operationId: settleTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction/{transactionID}/refund\n  method: post\n  operationId: refundTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment-options\n  method: get\n  operationId: listPaymentOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alliance-data-systems/refs/heads/main/agentic-access/alliance-data-systems-agentic-access.yml
summary_line: 14 operations · 8 acting
tags:
- Financial Services
- Fintech
- Buy Now Pay Later
- BNPL
- Bread Pay
- Private Label Credit
- Co Brand Credit Cards
- Loyalty Programs
- Marketing
- Data Driven Marketing
- Payments
- Lending
- Savings
- Personal Loans
- Consumer Banking
- Retail Finance
- Fortune 500
- NYSE BFH
- Comenity Bank
- Rebrand
---
