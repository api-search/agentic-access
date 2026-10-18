---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 5
api_specs:
- filename: paystand-balances-api-openapi.yml
  format: yaml
  label: PayStand Balances API
  slug: paystand-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystand/refs/heads/main/openapi/paystand-balances-api-openapi.yml
- filename: paystand-banks-api-openapi.yml
  format: yaml
  label: PayStand Banks API
  slug: paystand-banks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystand/refs/heads/main/openapi/paystand-banks-api-openapi.yml
- filename: paystand-oauth-api-openapi.yml
  format: yaml
  label: PayStand OAuth API
  slug: paystand-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystand/refs/heads/main/openapi/paystand-oauth-api-openapi.yml
- filename: paystand-payers-api-openapi.yml
  format: yaml
  label: PayStand Payers API
  slug: paystand-payers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystand/refs/heads/main/openapi/paystand-payers-api-openapi.yml
- filename: paystand-payments-api-openapi.yml
  format: yaml
  label: PayStand Payments API
  slug: paystand-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystand/refs/heads/main/openapi/paystand-payments-api-openapi.yml
- filename: paystand-refunds-api-openapi.yml
  format: yaml
  label: PayStand Refunds API
  slug: paystand-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystand/refs/heads/main/openapi/paystand-refunds-api-openapi.yml
- filename: paystand-transfers-api-openapi.yml
  format: yaml
  label: PayStand Transfers API
  slug: paystand-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystand/refs/heads/main/openapi/paystand-transfers-api-openapi.yml
- filename: paystand-withdrawals-api-openapi.yml
  format: yaml
  label: PayStand Withdrawals API
  slug: paystand-withdrawals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystand/refs/heads/main/openapi/paystand-withdrawals-api-openapi.yml
consequence_counts:
  physical: 3
  read: 5
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Paystand Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/secure
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /withdrawals
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /withdrawals/settings
operation_count: 12
overview: 'PayStand exposes 12 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read, 4 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: PayStand
provider_slug: paystand
slug: paystand-agentic-access
source_filename: paystand-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: generated\nsource: openapi/paystand-sandbox-open-api-openapi.yml, openapi/paystand-sandbox-secure-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    acting: 7\n    connected: 5\n  by_consequence:\n    write: 4\n    read: 5\n    physical: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /oauth/token\n  method: post\n  operationId: create-an-access-token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /balances/accounts\n  method:\
  \ post\n  operationId: create-an-account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /balances/summary\n  method: get\n  operationId: balance-summary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banks\n  method: post\n  operationId: create-bank\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payers\n  method: post\n  operationId: create-a-payer\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/all\n  method: get\n  operationId: get-all-payments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/secure\n  method: post\n  operationId: create-payment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /refunds/all\n  method: get\n  operationId: list-all-refunds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /transfers/all\n  method: get\n  operationId: list-all-transfers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /withdrawals\n  method: post\n  operationId: create-withdrawal\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /withdrawals/all\n  method: get\n  operationId: list-all-withdrawals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /withdrawals/settings\n  method: put\n  operationId: update-an-auto-withdrawal-settings\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paystand/refs/heads/main/agentic-access/paystand-agentic-access.yml
summary_line: 12 operations · 7 acting
tags:
- Company
- Payments
- B2B Payments
- Accounts Receivable
- Accounts Payable
- Fintech
- Blockchain
- ACH
- Billing
- Checkout
---
