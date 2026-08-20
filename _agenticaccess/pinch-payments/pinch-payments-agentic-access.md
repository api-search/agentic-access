---
acting_count: 27
action_class_counts:
  acting: 27
  connected: 29
api_specs:
- filename: pinch-payments-core.yml
  format: yaml
  label: Pinch Core API
  slug: pinch-payments-core
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-core.yml
- filename: pinch-payments-payments.yml
  format: yaml
  label: Pinch Payments API
  slug: pinch-payments-payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-payments.yml
- filename: pinch-payments-payers.yml
  format: yaml
  label: Pinch Payers API
  slug: pinch-payments-payers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-payers.yml
- filename: pinch-payments-payment-links.yml
  format: yaml
  label: Pinch Payment Links API
  slug: pinch-payments-payment-links
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-payment-links.yml
- filename: pinch-payments-merchants.yml
  format: yaml
  label: Pinch Merchants API
  slug: pinch-payments-merchants
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-merchants.yml
- filename: pinch-payments-webhooks.yml
  format: yaml
  label: Pinch Webhooks API
  slug: pinch-payments-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-webhooks.yml
- filename: pinch-payments-contacts.yml
  format: yaml
  label: Pinch Contacts API
  slug: pinch-payments-contacts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-contacts.yml
- filename: pinch-payments-transfers.yml
  format: yaml
  label: Pinch Transfers API
  slug: pinch-payments-transfers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-transfers.yml
- filename: pinch-payments-merchant-financial-data.yml
  format: yaml
  label: Pinch Merchant Financial Data API
  slug: pinch-payments-merchant-financial-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-merchant-financial-data.yml
- filename: pinch-payments-authentication.yml
  format: yaml
  label: Pinch Authentication API
  slug: pinch-payments-authentication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-authentication.yml
consequence_counts:
  physical: 11
  read: 29
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Pinch Payments Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payers/{id}/sources
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /payers/{id}/sources/{sourceId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment-links
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /payment-links/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/nonce
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/realtime
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /payments/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /refunds
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /refunds/nonce
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /tokens
operation_count: 56
overview: 'Pinch Payments exposes 56 API operations that an AI agent could call, of which 27 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 29 read, 16 write, and 11 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Pinch Payments
provider_slug: pinch-payments
slug: pinch-payments-agentic-access
source_filename: pinch-payments-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: generated\nsource: openapi/pinch-payments-authentication.yml, openapi/pinch-payments-contacts.yml, openapi/pinch-payments-core.yml,\n  openapi/pinch-payments-merchant-financial-data.yml, openapi/pinch-payments-merchants.yml,\n  openapi/pinch-payments-payers.yml, openapi/pinch-payments-payment-links.yml, openapi/pinch-payments-payments.yml,\n  openapi/pinch-payments-transfers.yml, openapi/pinch-payments-webhooks.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 56\n  by_action_class:\n    acting: 27\n    connected: 29\n  by_consequence:\n    write: 16\n    read: 29\n    physical: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /connect/token\n  method: post\n  operationId: tokens\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/{id}\n  method: delete\n  operationId: delete-contact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/{id}\n  method: get\n  operationId: get-contact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts\n  method: get\n  operationId: get-contacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /contacts\n  method: post\n  operationId: save-contact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fees/calculate\n  method: post\n  operationId: calculate-fees\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /plans/{planId}/calculated-payments\n  method: get\n  operationId: get_plans-planid-calculated-payments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions/{id}\n\
  \  method: delete\n  operationId: cancel-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/{id}\n  method: get\n  operationId: get-subscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /refunds/nonce\n  method: post\n  operationId: check-refund-nonce\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /refunds\n  method: post\n  operationId:\
  \ create-a-refund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /refunds\n  method: get\n  operationId: list-refunds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions\n  method: post\n  operationId: create-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions\n  method: get\n  operationId: list-subscriptions\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /plans/{id}\n  method: delete\n  operationId: delete-plan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /plans/{id}\n  method: get\n  operationId: get-plan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{id}\n  method: get\n  operationId: get-event\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fees\n  method: get\n  operationId: get-fees\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /refund/{id}\n  method: get\n  operationId: get-refund\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health/auth\n  method: get\n  operationId: health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events\n  method: get\n  operationId: list-all-events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /plans\n  method: get\n  operationId: list-plans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /plans\n  method: post\n  operationId: save-plan\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tokens\n  method: post\n  operationId: tokenise\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /merchant-financial-data/current\n  method: get\n  operationId: getCurrentMerchantFinancialData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchant-financial-data\n  method: post\n  operationId: saveMerchantFinancialData\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /merchants/managed\n  method: post\n  operationId: create-managed-merchant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /merchants/managed\n  method: get\n  operationId: list-managed-merchants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchants/update\n  method: post\n  operationId: update-merchant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n \
  \   audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /merchants/documents\n  method: post\n  operationId: upload-document\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payers/{id}/sources\n  method: post\n  operationId: create-payment-source\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payers/{id}\n  method: delete\n  operationId:\
  \ delete-payer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payers/{id}\n  method: get\n  operationId: get-payer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payers/{id}/sources/{sourceId}\n  method: delete\n  operationId: delete-payment-source\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payers\n  method: get\n  operationId: list-payers\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payers\n  method: post\n  operationId: save-payer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment-links\n  method: post\n  operationId: create-payment-link\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment-links\n  method: get\n  operationId: get-payment-links\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment-links/{id}\n  method: delete\n  operationId: delete-payment-link\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment-links/{id}\n  method: get\n  operationId: get-payment-link\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment-links/payer/{payerId}\n  method: get\n  operationId: get-payment-links-by-payer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/nonce\n  method: post\n\
  \  operationId: check-payment-nonce\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/{id}\n  method: delete\n  operationId: delete-payment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/{id}\n  method: get\n  operationId: get-payment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/payer/{id}\n\
  \  method: get\n  operationId: list-payments-for-payer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/processed\n  method: get\n  operationId: list-processed-payments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/scheduled\n  method: get\n  operationId: list-scheduled-payments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/realtime\n  method: post\n  operationId: realtime-payment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n    \
  \  triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments\n  method: post\n  operationId: save-payment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transfers/{id}\n  method: get\n  operationId: get-transfer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transfers\n  method: get\n  operationId: list-all-transfers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transfers/items/{id}\n  method: get\n  operationId: list-transfer-line-items\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: post\n  operationId: create-or-update-webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks\n  method: get\n  operationId: list-webhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/{id}\n  method: delete\n  operationId: delete-webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n \
  \     - high-value\n    audit: required\n- path: /webhooks/{id}\n  method: get\n  operationId: get-webhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/agentic-access/pinch-payments-agentic-access.yml
summary_line: 56 operations · 27 acting
tags:
- Payments
- Australia
- Payment Gateway
- Payment Processing
- Direct Debit
- Card Payments
- Subscription
- Billing
- Payment Facilitator
- Account-to-Account
- New Zealand
---
