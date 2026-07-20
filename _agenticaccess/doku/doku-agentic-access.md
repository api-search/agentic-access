---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 8
api_specs:
- filename: doku-openapi.yml
  format: yaml
  label: DOKU Checkout API
  slug: doku-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doku/refs/heads/main/openapi/doku-openapi.yml
- filename: doku-openapi.yml
  format: yaml
  label: DOKU SNAP Access Token API
  slug: doku-snap-access-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doku/refs/heads/main/openapi/doku-openapi.yml
- filename: doku-openapi.yml
  format: yaml
  label: DOKU SNAP Virtual Account API
  slug: doku-snap-virtual-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doku/refs/heads/main/openapi/doku-openapi.yml
- filename: doku-openapi.yml
  format: yaml
  label: DOKU SNAP Direct Debit & e-Wallet API
  slug: doku-snap-direct-debit-ewallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doku/refs/heads/main/openapi/doku-openapi.yml
- filename: doku-openapi.yml
  format: yaml
  label: DOKU SNAP QRIS API
  slug: doku-snap-qris-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doku/refs/heads/main/openapi/doku-openapi.yml
- filename: doku-openapi.yml
  format: yaml
  label: DOKU Kirim Payout API
  slug: doku-kirim-payout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doku/refs/heads/main/openapi/doku-openapi.yml
consequence_counts:
  read: 8
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. Payments move real money in IDR, so money-movement operations default to human-in-the-loop required. See research/curity/agentic-governance/.
human_in_the_loop: 5
kind: agentic-access
layout: agentic-access
method: generated
name: Doku Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 19
overview: 'DOKU exposes 19 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 11 write.


  5 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: DOKU
provider_slug: doku
slug: doku-agentic-access
source_filename: doku-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: generated\nsource: openapi/doku-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. Payments move real money in IDR, so money-movement operations default\n  to human-in-the-loop required. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    acting: 11\n    connected: 8\n  by_consequence:\n    write: 11\n    read: 8\n  human_in_the_loop_required: 5\noperations:\n- path: /checkout/v1/payment\n  method: post\n  operationId: createCheckoutPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - money-movement\n      - high-value\n    audit: required\n- path:\
  \ /authorization/v1/access-token/b2b\n  method: post\n  operationId: getAccessTokenB2B\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    token:\n      max-ttl: 900\n    audit: required\n- path: /authorization/v1/access-token/b2b2c\n  method: post\n  operationId: getAccessTokenB2B2C\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    token:\n      max-ttl: 900\n    audit: required\n- path: /virtual-accounts/bi-snap-va/v1.1/transfer-va/create-va\n  method: post\n  operationId: createVirtualAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /virtual-accounts/bi-snap-va/v1.1/transfer-va/update-va\n  method: put\n  operationId: updateVirtualAccount\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /virtual-accounts/bi-snap-va/v1.1/transfer-va/delete-va\n  method: delete\n  operationId: deleteVirtualAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /virtual-accounts/bi-snap-va/v1.1/transfer-va/inquiry\n  method: post\n  operationId: inquiryVirtualAccountStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /direct-debit/core/v1/registration-account-binding\n  method: post\n\
  \  operationId: bindEwalletAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - account-linking\n      - consent\n    audit: required\n- path: /direct-debit/core/v1/balance-inquiry\n  method: post\n  operationId: ewalletBalanceInquiry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    token:\n      max-ttl: 900\n    audit: required\n- path: /direct-debit/core/v1/debit/payment-host-to-host\n  method: post\n  operationId: debitPaymentHostToHost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - money-movement\n      - high-value\n    audit: required\n- path: /direct-debit/core/v1/debit/refund\n\
  \  method: post\n  operationId: debitRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - money-movement\n      - reversal\n    audit: required\n- path: /direct-debit/core/v1/registration-account-unbinding\n  method: post\n  operationId: unbindEwalletAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    audit: required\n- path: /snap-adapter/b2b/v1.0/qr/qr-mpm-generate\n  method: post\n  operationId: generateQrisMpm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n    \
  \  triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /snap-adapter/b2b/v1.0/qr/qr-mpm-query\n  method: post\n  operationId: queryQrisMpm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /snap-adapter/b2b/v1.0/qr/qr-mpm-refund\n  method: post\n  operationId: refundQrisMpm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - money-movement\n      - reversal\n    audit: required\n- path: /payout/kirim-doku/balance-inquiry\n  method: post\n  operationId: payoutBalanceInquiry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    token:\n      max-ttl: 900\n    audit: required\n- path: /payout/kirim-doku/account-inquiry\n  method: post\n  operationId:\
  \ payoutAccountInquiry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    token:\n      max-ttl: 900\n    audit: required\n- path: /payout/kirim-doku/transfer-bank\n  method: post\n  operationId: payoutTransferBank\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - money-movement\n      - disbursement\n      - high-value\n    audit: required\n- path: /payout/kirim-doku/check-status\n  method: post\n  operationId: payoutCheckStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doku/refs/heads/main/agentic-access/doku-agentic-access.yml
summary_line: 19 operations · 11 acting · 5 human-in-the-loop
tags:
- Payments
- Payment Gateway
- Fintech
- Indonesia
- SEA
- SNAP
- Virtual Account
- E-Wallet
- QRIS
- Direct Debit
- Payouts
---
