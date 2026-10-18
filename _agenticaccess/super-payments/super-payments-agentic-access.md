---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 16
api_specs:
- filename: super-payments-checkout-sessions-api-openapi.yml
  format: yaml
  label: Super Payments Checkout Sessions API
  slug: super-payments-checkout-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/super-payments/refs/heads/main/openapi/super-payments-checkout-sessions-api-openapi.yml
- filename: super-payments-customer-api-openapi.yml
  format: yaml
  label: Super Payments Customer API
  slug: super-payments-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/super-payments/refs/heads/main/openapi/super-payments-customer-api-openapi.yml
- filename: super-payments-payment-links-api-openapi.yml
  format: yaml
  label: Super Payments Payment Links API
  slug: super-payments-payment-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/super-payments/refs/heads/main/openapi/super-payments-payment-links-api-openapi.yml
- filename: super-payments-payment-methods-api-openapi.yml
  format: yaml
  label: Super Payments Payment Methods API
  slug: super-payments-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/super-payments/refs/heads/main/openapi/super-payments-payment-methods-api-openapi.yml
- filename: super-payments-payments-api-openapi.yml
  format: yaml
  label: Super Payments API
  slug: super-payments-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/super-payments/refs/heads/main/openapi/super-payments-payments-api-openapi.yml
- filename: super-payments-refunds-api-openapi.yml
  format: yaml
  label: Super Payments Refunds API
  slug: super-payments-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/super-payments/refs/heads/main/openapi/super-payments-refunds-api-openapi.yml
- filename: super-payments-rewards-api-openapi.yml
  format: yaml
  label: Super Payments Rewards API
  slug: super-payments-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/super-payments/refs/heads/main/openapi/super-payments-rewards-api-openapi.yml
- filename: super-payments-settlements-api-openapi.yml
  format: yaml
  label: Super Payments Settlements API
  slug: super-payments-settlements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/super-payments/refs/heads/main/openapi/super-payments-settlements-api-openapi.yml
- filename: super-payments-webhooks-api-openapi.yml
  format: yaml
  label: Super Payments Webhooks API
  slug: super-payments-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/super-payments/refs/heads/main/openapi/super-payments-webhooks-api-openapi.yml
consequence_counts:
  physical: 11
  read: 16
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Super Payments Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkout-sessions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkout-sessions/{checkoutSessionId}/order-details
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkout-sessions/{checkoutSessionId}/proceed
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment-links
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /payment-links/{linkId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /payment-links/{linkId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment-methods
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment-methods/{id}/setup-intents
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /refunds
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /refunds/payouts
operation_count: 31
overview: 'Super Payments exposes 31 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read, 4 write, and 11 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Super Payments
provider_slug: super-payments
slug: super-payments-agentic-access
source_filename: super-payments-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: generated\nsource: openapi/super-payments-checkout-sessions-api-openapi.yml, openapi/super-payments-customer-api-openapi.yml,\n  openapi/super-payments-payment-links-api-openapi.yml, openapi/super-payments-payment-methods-api-openapi.yml,\n  openapi/super-payments-payments-api-openapi.yml, openapi/super-payments-refunds-api-openapi.yml,\n  openapi/super-payments-rewards-api-openapi.yml, openapi/super-payments-settlements-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 31\n  by_action_class:\n    acting: 15\n    connected: 16\n  by_consequence:\n    physical: 11\n    read: 16\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /checkout-sessions\n  method: post\n  operationId:\
  \ create-checkout-session\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /checkout-sessions/{checkoutSessionId}\n  method: get\n  operationId: get-checkout-session\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /checkout-sessions/{checkoutSessionId}/proceed\n  method: post\n  operationId: proceed-payment-via-checkout-session\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /checkout-sessions/{checkoutSessionId}/order-details\n  method: post\n  operationId: upsert-order-details\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers\n  method: post\n  operationId: create-customer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers\n  method: get\n  operationId: list-customers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{id}\n  method: get\n  operationId: get-customer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{id}\n  method: patch\n  operationId: patch-customer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment-links\n  method: post\n  operationId: create-link\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /payment-links\n  method: get\n  operationId: list-links\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment-links/{linkId}\n  method: delete\n  operationId: delete-link\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment-links/{linkId}\n  method: get\n  operationId: get-link\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment-links/{linkId}\n  method: put\n  operationId: update-link\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment-methods\n  method: post\n  operationId: create-payment-method\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment-methods\n  method: get\n  operationId: list-payment-methods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment-methods/{id}/setup-intents\n  method: post\n  operationId: create-setup-intent\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment-methods/{id}\n  method: get\n  operationId: get-payment-method\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment-methods/setup-intents\n  method: get\n  operationId: list-setup-intents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments\n  method: post\n  operationId: create-payment-intent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n \
  \     max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/{transactionId}\n  method: get\n  operationId: get-payment-transaction-2025-11-01\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/search\n  method: get\n  operationId: search-payment-transactions-2025-11-01\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /refunds/payouts\n  method: post\n  operationId: create-payout-refund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /refunds\n  method: post\n  operationId: create-refund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /refunds/{transactionId}\n  method: get\n  operationId: get-refund-transaction-2025-11-01\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /refunds/search\n  method: get\n  operationId: search-refund-transactions-2025-11-01\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reward-calculations\n\
  \  method: post\n  operationId: generate-reward-calculation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /brands/{brandId}/reward-configuration\n  method: get\n  operationId: get-reward-configuration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /brands/{brandId}/reward-configuration\n  method: put\n  operationId: upsert-brand-reward-configuration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settlements/{settlementId}\n\
  \  method: get\n  operationId: get-settlement-detail-2025-11-01\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /settlements/{settlementId}/reconciliation\n  method: get\n  operationId: get-settlement-reconciliation-2025-11-01\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /settlements\n  method: get\n  operationId: list-settlements-2025-11-01\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/super-payments/refs/heads/main/agentic-access/super-payments-agentic-access.yml
summary_line: 31 operations · 15 acting
tags:
- Company
- Payments
- Open Banking
- Cash Rewards
- Checkout
- Fintech
- United Kingdom
- Pay by Bank
---
