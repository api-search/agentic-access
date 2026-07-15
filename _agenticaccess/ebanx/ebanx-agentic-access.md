---
acting_count: 29
action_class_counts:
  acting: 29
api_specs:
- filename: ebanx-pay-in-direct-api-openapi.yml
  format: yaml
  label: EBANX Pay-in Direct API
  slug: ebanx-pay-in-direct-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ebanx/refs/heads/main/openapi/ebanx-pay-in-direct-api-openapi.yml
- filename: ebanx-payment-page-api-openapi.yml
  format: yaml
  label: EBANX Payment Page API
  slug: ebanx-payment-page-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ebanx/refs/heads/main/openapi/ebanx-payment-page-api-openapi.yml
- filename: ebanx-tokenization-api-openapi.yml
  format: yaml
  label: EBANX Tokenization API
  slug: ebanx-tokenization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ebanx/refs/heads/main/openapi/ebanx-tokenization-api-openapi.yml
- filename: ebanx-fx-api-openapi.yml
  format: yaml
  label: EBANX FX API
  slug: ebanx-fx-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ebanx/refs/heads/main/openapi/ebanx-fx-api-openapi.yml
- filename: ebanx-payout-api-openapi.yml
  format: yaml
  label: EBANX Payout API
  slug: ebanx-payout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ebanx/refs/heads/main/openapi/ebanx-payout-api-openapi.yml
- filename: ebanx-notifications-asyncapi.yml
  format: yaml
  label: EBANX Payment Notifications
  slug: ebanx-notifications
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/ebanx/refs/heads/main/asyncapi/ebanx-notifications-asyncapi.yml
consequence_counts:
  physical: 25
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ebanx Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /print
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ws/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ws/capture
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ws/cardbin
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ws/direct
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ws/ewallet-availableEWallets
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ws/getBankList
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ws/instalmentsPlan
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ws/payee/create
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ws/payout/attach
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ws/payout/balance
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ws/payout/bankDetails
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ws/payout/banks
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ws/payout/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ws/payout/commit
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ws/payout/create
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ws/payout/retrieve
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ws/payout/search
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ws/payout/simulate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ws/payout/verify_account
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ws/query
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ws/refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ws/refundOrCancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ws/request
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ws/updatecustomerbankinfo
operation_count: 29
overview: 'EBANX exposes 29 API operations that an AI agent could call, of which 29 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 write and 25 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: EBANX
provider_slug: ebanx
slug: ebanx-agentic-access
source_filename: ebanx-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/ebanx-fx-api-openapi.yml, openapi/ebanx-pay-in-direct-api-openapi.yml, openapi/ebanx-payment-page-api-openapi.yml,\n  openapi/ebanx-payout-api-openapi.yml, openapi/ebanx-tokenization-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 29\n  by_action_class:\n    acting: 29\n  by_consequence:\n    write: 4\n    physical: 25\n  human_in_the_loop_required: 0\noperations:\n- path: /ws/exchange\n  method: post\n  operationId: getExchangeRate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /ws/fxtoken/get\n  method: post\n  operationId: getFxToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ws/direct\n  method: post\n  operationId: createDirectPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ws/capture\n  method: post\n  operationId: capturePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ws/query\n  method: post\n  operationId: queryPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ws/cancel\n  method: post\n  operationId: cancelPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ws/refund\n\
  \  method: post\n  operationId: refundPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ws/refundOrCancel\n  method: post\n  operationId: refundOrCancelPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ws/instalmentsPlan\n  method: post\n  operationId: listInstallmentsPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ws/cardbin\n  method: post\n  operationId: lookupCardBin\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ws/getBankList\n  method: post\n  operationId: listAvailableBanks\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /ws/ewallet-availableEWallets\n  method: post\n  operationId: listAvailableEWallets\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ws/updatecustomerbankinfo\n  method: post\n  operationId: updateCustomerBankInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /print\n  method: post\n  operationId: printVoucherOrSlip\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ws/request\n  method: post\n  operationId: createPaymentPageRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ws/payout/create\n  method: post\n  operationId: createPayout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n  \
  \    triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ws/payout/commit\n  method: post\n  operationId: commitPayout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ws/payout/cancel\n  method: post\n  operationId: cancelPayout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ws/payout/retrieve\n  method: post\n  operationId: retrievePayout\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ws/payout/search\n  method: post\n  operationId: searchPayouts\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ws/payout/simulate\n  method: post\n  operationId: simulatePayout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ws/payout/attach\n  method: post\n  operationId: attachPayoutInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ws/payout/balance\n  method: post\n  operationId: getPayoutBalance\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ws/payout/banks\n  method: post\n  operationId: listPayoutBanks\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ws/payout/bankDetails\n  method: post\n  operationId: getPayoutBankDetails\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ws/payout/verify_account\n  method: post\n  operationId: verifyPayeeBankAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ws/payee/create\n  method: post\n  operationId: createPayee\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ws/token\n  method: post\n  operationId: createCardToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ws/token/setCVV\n  method: post\n  operationId: setTokenCVV\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ebanx/refs/heads/main/agentic-access/ebanx-agentic-access.yml
summary_line: 29 operations · 29 acting
tags:
- Payments
- Pay-in
- Payouts
- Foreign Exchange
- Tokenization
- LATAM
- Emerging Markets
- Pix
- Boleto
- OXXO
- SPEI
- PSE
- Cross-Border
- Webhooks
---
