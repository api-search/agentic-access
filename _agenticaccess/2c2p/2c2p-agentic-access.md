---
acting_count: 10
action_class_counts:
  acting: 10
api_specs:
- filename: 2c2p-openapi.yml
  format: yaml
  label: 2C2P Payment Token API
  slug: 2c2p-payment-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2c2p/refs/heads/main/openapi/2c2p-openapi.yml
- filename: 2c2p-openapi.yml
  format: yaml
  label: 2C2P Do Payment API
  slug: 2c2p-do-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2c2p/refs/heads/main/openapi/2c2p-openapi.yml
- filename: 2c2p-openapi.yml
  format: yaml
  label: 2C2P Payment Option API
  slug: 2c2p-payment-option-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2c2p/refs/heads/main/openapi/2c2p-openapi.yml
- filename: 2c2p-openapi.yml
  format: yaml
  label: 2C2P Payment Inquiry API
  slug: 2c2p-payment-inquiry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2c2p/refs/heads/main/openapi/2c2p-openapi.yml
- filename: 2c2p-openapi.yml
  format: yaml
  label: 2C2P Payment Maintenance API
  slug: 2c2p-payment-maintenance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2c2p/refs/heads/main/openapi/2c2p-openapi.yml
- filename: 2c2p-openapi.yml
  format: yaml
  label: 2C2P Card Token & Recurring API
  slug: 2c2p-card-token-recurring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2c2p/refs/heads/main/openapi/2c2p-openapi.yml
- filename: 2c2p-openapi.yml
  format: yaml
  label: 2C2P Exchange Rate API
  slug: 2c2p-exchange-rate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2c2p/refs/heads/main/openapi/2c2p-openapi.yml
consequence_counts:
  physical: 5
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: 2C2P Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /paymentInquiry
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /paymentOption
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /paymentOptionDetails
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /paymentToken
operation_count: 10
overview: '2C2P exposes 10 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 write and 5 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: 2C2P
provider_slug: 2c2p
slug: 2c2p-agentic-access
source_filename: 2c2p-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/2c2p-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    acting: 10\n  by_consequence:\n    physical: 5\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /paymentToken\n  method: post\n  operationId: paymentToken\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment\n  method: post\n  operationId: doPayment\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /paymentOption\n  method: post\n  operationId: paymentOption\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /paymentOptionDetails\n  method: post\n  operationId: paymentOptionDetails\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /paymentInquiry\n  method: post\n  operationId: paymentInquiry\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transactionStatus\n  method: post\n  operationId: transactionStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cancelTransaction\n  method: post\n  operationId: cancelTransaction\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cardTokenInfo\n  method: post\n  operationId: cardTokenInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cardInstallmentPlanInfo\n  method: post\n  operationId: cardInstallmentPlanInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /exchangeRate\n  method: post\n  operationId: exchangeRate\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/2c2p/refs/heads/main/agentic-access/2c2p-agentic-access.yml
summary_line: 10 operations · 10 acting
tags:
- Payments
- Payment Gateway
- Southeast Asia
- Singapore
- Thailand
- Cards
- E-Wallet
- Payment Token
- Cross-Border
- Fintech
---
