---
acting_count: 30
action_class_counts:
  acting: 30
  connected: 17
api_specs:
- filename: payu-europe-rest-api.yaml
  format: yaml
  label: PayU Europe REST API
  slug: payu-europe-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payu/refs/heads/main/openapi/payu-europe-rest-api.yaml
consequence_counts:
  physical: 12
  read: 17
  write: 18
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Payu Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/aml-verification/v1/dataloading/payouts/bankAccountData
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/aml-verification/v1/dataloading/payouts/payoneer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/aml-verification/v1/dataloading/payouts/worldfirst
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/aml-verification/v1/verification-transfers/manual
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2_1/customers/ext/{extCustomerId}/feeCreditTransfer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2_1/customers/ext/{extCustomerId}/feeDebitTransfer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2_1/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/v2_1/orders/{orderId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2_1/orders/{orderId}/captures
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2_1/orders/{orderId}/refunds
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/v2_1/orders/{orderId}/status
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2_1/payouts
operation_count: 47
overview: 'PayU exposes 47 API operations that an AI agent could call, of which 30 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read, 18 write, and 12 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: PayU
provider_slug: payu
slug: payu-agentic-access
source_filename: payu-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/payu-europe-rest-api.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 47\n  by_action_class:\n    acting: 30\n    connected: 17\n  by_consequence:\n    write: 18\n    read: 17\n    physical: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /pl/standard/user/oauth/authorize\n  method: post\n  operationId: oauth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - client_credentials\n- path: /api/v2_1/paymethods\n  method: get\n  operationId:\
  \ retrieve-payment-methods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - client_credentials\n    - trusted_merchant\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2_1/orders\n  method: post\n  operationId: create-an-order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - client_credentials\n    - trusted_merchant\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2_1/orders/{orderId}\n  method: get\n  operationId: retrieve-an-order\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - client_credentials\n- path: /api/v2_1/orders/{orderId}\n\
  \  method: delete\n  operationId: cancel-an-order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - client_credentials\n- path: /api/v2_1/orders/{orderId}/captures\n  method: post\n  operationId: capture-authorized-order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - client_credentials\n- path: /api/v2_1/orders/{orderId}/status\n  method: put\n  operationId: capture-authorized-order-deprecated\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - client_credentials\n- path: /api/v2_1/orders/{orderId}/transactions\n  method: get\n  operationId: retrieve-a-transaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - oAuth token\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2_1/shops/{shopId}\n  method: get\n  operationId: retrieve-shop-data\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - client_credentials\n- path: /api/v2_1/orders/{orderId}/refunds\n  method: post\n  operationId: create-a-refund\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - client_credentials\n- path: /api/v2_1/orders/{orderId}/refunds\n  method: get\n  operationId: retrieve-all-refunds-for-the-specified-order\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - client_credentials\n- path: /api/v2_1/orders/{orderId}/refunds/{refundId}\n  method: get\n  operationId: retrieve-specific-refund\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - client_credentials\n- path: /api/v2_1/payouts\n  method:\
  \ post\n  operationId: create-a-payout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - client_credentials\n- path: /api/v2_1/payouts/{payoutId}\n  method: get\n  operationId: retrieve-a-payout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - client_credentials\n- path: /api/v2_1/tokens/{token}\n  method: delete\n  operationId: delete-a-token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - trusted_merchant\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2_1/mcp-partners/{mcpPartnerId}/fx-table\n  method: get\n  operationId: retrieve-rate-table\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - client_credentials\n- path: /api/v2_1/fx-providers/ecb/fx-rates\n  method: get\n  operationId: retrieve-reference-rates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - client_credentials\n- path: /api/v2_1/customers/ext/{extCustomerId}/status\n  method: get\n  operationId: retrieve-seller-status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - client_credentials\n- path: /api/v2_1/customers/ext/{extCustomerId}/balances\n\
  \  method: get\n  operationId: retrieve-seller-balance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - client_credentials\n- path: /api/v2_1/customers/ext/{extCustomerId}/operations\n  method: get\n  operationId: retrieve-seller-operation-history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - client_credentials\n- path: /api/v2_1/customers/ext/{extCustomerId}/feeDebitTransfer\n  method: post\n  operationId: transfer-funds-from-seller-to-marketplace-balance\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n    scope:\n    - client_credentials\n- path: /api/v2_1/customers/ext/{extCustomerId}/feeCreditTransfer\n  method: post\n  operationId: transfer-funds-from-marketplace-to-seller-balance\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - client_credentials\n- path: /api/aml-verification/v1/verification-advice\n  method: get\n  operationId: retrieve-marketplace-verification-advice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - client_credentials\n- path: /api/aml-verification/v1/verification\n  method: get\n  operationId: retrieve-marketplace-verification-status\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - client_credentials\n- path: /api/aml-verification/v1/verification\n  method: post\n  operationId: create-marketplace-verification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - client_credentials\n- path: /api/aml-verification/v1/dataloading/seller\n  method: post\n  operationId: add-sellers-data\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n\
  \    - client_credentials\n- path: /api/aml-verification/v1/dataloading/associates\n  method: post\n  operationId: add-associates-data\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - client_credentials\n- path: /api/aml-verification/v1/dataloading/files\n  method: post\n  operationId: add-files\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - client_credentials\n- path: /api/aml-verification/v1/dataloading/seller/documents\n  method: post\n  operationId: add-sellers-documents\n  x-agentic-access:\n \
  \   action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - client_credentials\n- path: /api/aml-verification/v1/dataloading/associates/documents\n  method: post\n  operationId: add-associates-documents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - client_credentials\n- path: /api/aml-verification/v1/verification-transfers/manual\n  method: post\n  operationId: create-order-for-verification-transfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n  \
  \    max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - client_credentials\n- path: /api/aml-verification/v1/dataloading/payouts/bankAccountData\n  method: post\n  operationId: add-bank-account-for-payouts\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - client_credentials\n- path: /api/aml-verification/v1/dataloading/payouts/payoneer\n  method: post\n  operationId: add-payoneer-account-for-payouts\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n \
  \     max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - client_credentials\n- path: /api/aml-verification/v1/dataloading/payouts/worldfirst\n  method: post\n  operationId: add-worldfirst-account-for-payouts\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - client_credentials\n- path: /api/aml-verification/v1/verification/complete\n  method: post\n  operationId: complete-marketplace-verification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - client_credentials\n- path: /api/aml-verification/v1/verification/cancel\n  method: post\n  operationId: cancel-marketplace-verification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - client_credentials\n- path: /api/front/card-installments-options\n  method: post\n  operationId: retrieve-card-installments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n\
  \    - client_credentials\n- path: /api/v2_1/reports/{reportId}\n  method: get\n  operationId: retrieve-statement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2_1/firms\n  method: post\n  operationId: create-a-firm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - client_credentials\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2_1/firms/{firmId}/urls\n  method: post\n  operationId: create-a-url-for-the-partners-firm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - partner\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n \
  \     - abnormal\n      - high-value\n    audit: required\n- path: /api/v2_1/firms{firmId}/shops\n  method: post\n  operationId: create-a-shop-for-the-partner\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - partner\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2_1/shops/{shopId}/poses\n  method: post\n  operationId: create-pos-for-partner\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - partner\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2_1/poses/{posId}\n  method: get\n  operationId: retrieve-partners-pos-data\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    scope:\n    - partner\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2_1/firms/{posId}/users\n  method: post\n  operationId: create-a-user\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - partner\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2_1/firms/{firmPublicId}/submerchants\n  method: post\n  operationId: create-a-submerchant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - client_credentials\n- path: /api/v2_1/firms/{firmPublicId}/submerchants/{submerchantId}\n\
  \  method: put\n  operationId: update-submerchants-data\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - client_credentials\n- path: /api/v2_1/firms/{firmPublicId}/submerchants/{submerchantId}\n  method: get\n  operationId: retrieve-submerchant-data\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - client_credentials\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payu/refs/heads/main/agentic-access/payu-agentic-access.yml
summary_line: 47 operations · 30 acting
tags:
- Payments
- Payment Processing
- Fintech
- Financial Services
- Subscriptions
- Fraud Detection
- Checkout
- Marketplace
- Tokenization
- Emerging Markets
---
