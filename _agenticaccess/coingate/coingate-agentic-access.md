---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 6
api_specs:
- filename: coingate-conversions-api-openapi.yml
  format: yaml
  label: CoinGate Conversions API
  slug: coingate-conversions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingate/openapi/coingate-conversions-api-openapi.yml
- filename: coingate-currencies-api-openapi.yml
  format: yaml
  label: CoinGate Currencies API
  slug: coingate-currencies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingate/openapi/coingate-currencies-api-openapi.yml
- filename: coingate-orders-api-openapi.yml
  format: yaml
  label: CoinGate Orders API
  slug: coingate-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingate/openapi/coingate-orders-api-openapi.yml
- filename: coingate-refunds-api-openapi.yml
  format: yaml
  label: CoinGate Refunds API
  slug: coingate-refunds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingate/openapi/coingate-refunds-api-openapi.yml
- filename: coingate-send-requests-api-openapi.yml
  format: yaml
  label: CoinGate Send Requests API
  slug: coingate-send-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingate/openapi/coingate-send-requests-api-openapi.yml
- filename: coingate-beneficiaries-api-openapi.yml
  format: yaml
  label: CoinGate Beneficiaries API
  slug: coingate-beneficiaries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingate/openapi/coingate-beneficiaries-api-openapi.yml
- filename: coingate-beneficiary-payout-settings-api-openapi.yml
  format: yaml
  label: CoinGate Beneficiary Payout Settings API
  slug: coingate-beneficiary-payout-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingate/openapi/coingate-beneficiary-payout-settings-api-openapi.yml
- filename: coingate-billing-api-openapi.yml
  format: yaml
  label: CoinGate Billing API
  slug: coingate-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingate/openapi/coingate-billing-api-openapi.yml
- filename: coingate-contacts-api-openapi.yml
  format: yaml
  label: CoinGate Contacts API
  slug: coingate-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingate/openapi/coingate-contacts-api-openapi.yml
- filename: coingate-countries-api-openapi.yml
  format: yaml
  label: CoinGate Countries API
  slug: coingate-countries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingate/openapi/coingate-countries-api-openapi.yml
- filename: coingate-deposits-api-openapi.yml
  format: yaml
  label: CoinGate Deposits API
  slug: coingate-deposits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingate/openapi/coingate-deposits-api-openapi.yml
- filename: coingate-industries-api-openapi.yml
  format: yaml
  label: CoinGate Industries API
  slug: coingate-industries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingate/openapi/coingate-industries-api-openapi.yml
- filename: coingate-invoice-api-openapi.yml
  format: yaml
  label: CoinGate Invoice API
  slug: coingate-invoice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingate/openapi/coingate-invoice-api-openapi.yml
- filename: coingate-ledger-api-openapi.yml
  format: yaml
  label: CoinGate Ledger API
  slug: coingate-ledger-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingate/openapi/coingate-ledger-api-openapi.yml
- filename: coingate-mass-payouts-api-openapi.yml
  format: yaml
  label: CoinGate Mass Payouts API
  slug: coingate-mass-payouts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingate/openapi/coingate-mass-payouts-api-openapi.yml
- filename: coingate-new-endpoint-api-openapi.yml
  format: yaml
  label: CoinGate New Endpoint API
  slug: coingate-new-endpoint-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingate/openapi/coingate-new-endpoint-api-openapi.yml
- filename: coingate-payment-channels-api-openapi.yml
  format: yaml
  label: CoinGate Payment Channels API
  slug: coingate-payment-channels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingate/openapi/coingate-payment-channels-api-openapi.yml
- filename: coingate-payout-links-api-openapi.yml
  format: yaml
  label: CoinGate Payout Links API
  slug: coingate-payout-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingate/openapi/coingate-payout-links-api-openapi.yml
- filename: coingate-ping-api-openapi.yml
  format: yaml
  label: CoinGate Ping API
  slug: coingate-ping-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingate/openapi/coingate-ping-api-openapi.yml
- filename: coingate-platforms-api-openapi.yml
  format: yaml
  label: CoinGate Platforms API
  slug: coingate-platforms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingate/openapi/coingate-platforms-api-openapi.yml
- filename: coingate-rates-api-openapi.yml
  format: yaml
  label: CoinGate Rates API
  slug: coingate-rates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingate/openapi/coingate-rates-api-openapi.yml
consequence_counts:
  physical: 3
  read: 6
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Coingate Agentic Access
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
  method: POST
  path: /orders/{order_id}/refunds
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /send_requests
operation_count: 10
overview: 'CoinGate exposes 10 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 1 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CoinGate
provider_slug: coingate
slug: coingate-agentic-access
source_filename: coingate-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    acting: 4\n    connected: 6\n  by_consequence:\n    physical: 3\n    read: 6\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /orders\n  method: post\n  operationId: create-order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders\n  method: get\n  operationId: list-orders\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{id}\n  method: get\n  operationId: get-order\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{order_id}/refunds\n  method: post\n  operationId: create-refund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /send_requests\n  method: post\n  operationId: create-send\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /send_requests\n  method: get\n  operationId: list-send\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /send_requests/{id}\n  method: get\n  operationId: get-send\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ledger/conversions\n  method: post\n  operationId: create-conversion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ledger/conversions\n  method: get\n  operationId: list-conversions\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /currencies\n  method: get\n  operationId: currencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/coingate/agentic-access/coingate-agentic-access.yml
summary_line: 10 operations · 4 acting
tags:
- Cryptocurrency
- Payments
- Payment Gateway
- Fintech
- Bitcoin
- Ethereum
- Merchant Services
---
