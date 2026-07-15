---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 22
api_specs:
- filename: prestmit-openapi.yml
  format: yaml
  label: Prestmit Partner API
  slug: prestmit-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prestmit/refs/heads/main/openapi/prestmit-openapi.yml
consequence_counts:
  physical: 4
  read: 22
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Prestmit Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/partners/v1/giftcard/trade/buy/calculate-payment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/partners/v1/giftcard/trade/buy/create
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/partners/v1/giftcard/trade/sell/create
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/partners/v1/wallet/fiat/create-withdrawal
operation_count: 31
overview: 'Prestmit exposes 31 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read, 5 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Prestmit
provider_slug: prestmit
slug: prestmit-agentic-access
source_filename: prestmit-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/prestmit-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 31\n  by_action_class:\n    connected: 22\n    acting: 9\n  by_consequence:\n    read: 22\n    write: 5\n    physical: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /api/partners/v1/general/user\n  method: get\n  operationId: getAccountProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/partners/v1/general/commissions-and-fees\n  method: get\n  operationId: getCommissionsAndFees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /api/partners/v1/general/service-availability\n  method: get\n  operationId: getServiceAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/partners/v1/general/nigerian-banks\n  method: get\n  operationId: listNigerianBanksGeneral\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/partners/v1/lookup/nigerian-banks\n  method: get\n  operationId: lookupNigerianBanks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/partners/v1/lookup/ghanian-banks\n  method: get\n  operationId: lookupGhanaianBanks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/partners/v1/lookup/sell-giftcard-categories\n  method: get\n  operationId: lookupSellGiftcardCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/partners/v1/lookup/sell-giftcard-subcategories\n  method: get\n  operationId: lookupSellGiftcardSubcategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/partners/v1/lookup/sell-giftcard-filters\n  method: get\n  operationId: lookupSellGiftcardFilters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/partners/v1/lookup/sell-giftcard-payout-methods\n  method: get\n  operationId: lookupSellGiftcardPayoutMethods\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/partners/v1/bank-accounts/naira/list\n  method: get\n  operationId: listNairaBankAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/partners/v1/bank-accounts/naira/create\n  method: post\n  operationId: createNairaBankAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/partners/v1/bank-accounts/naira/{id}\n  method: delete\n  operationId: deleteNairaBankAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/partners/v1/bank-accounts/cedis/list\n  method: get\n  operationId: listCedisBankAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/partners/v1/bank-accounts/cedis/create\n  method: post\n  operationId: createCedisBankAccountV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/partners/v1/bank-accounts/cedis/create-v2\n  method: post\n  operationId: createCedisBankAccountV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/partners/v1/bank-accounts/cedis/{id}\n  method: delete\n  operationId: deleteCedisBankAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/partners/v1/wallet/fiat/details\n  method: get\n  operationId: getWalletDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/partners/v1/wallet/fiat/create-withdrawal\n  method: post\n  operationId: createWalletWithdrawal\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n\
  \      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/partners/v1/wallet/fiat/withdrawal-history\n  method: get\n  operationId: getWalletWithdrawalHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/partners/v1/wallet/fiat/withdrawal-history/{withdrawalId}/receipt\n  method: get\n  operationId: getWalletWithdrawalReceipt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/partners/v1/giftcard/trade/buy/config\n  method: get\n  operationId: getBuyConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/partners/v1/giftcard/trade/buy/calculate-payment\n\
  \  method: post\n  operationId: calculateBuyPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/partners/v1/giftcard/trade/buy/create\n  method: post\n  operationId: createBuyOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/partners/v1/giftcard/trade/buy/crypto-payment-status/{reference}\n  method: get\n  operationId: getBuyCryptoPaymentStatus\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/partners/v1/giftcard/trade/buy/fetch-codes/{reference}\n  method: get\n  operationId: fetchBuyCodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/partners/v1/giftcard/trade/buy/history\n  method: get\n  operationId: getBuyHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/partners/v1/giftcard/trade/sell/rate-calculator-data\n  method: get\n  operationId: getSellRateCalculatorData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/partners/v1/giftcard/trade/sell/payout-methods\n  method: get\n  operationId: getSellPayoutMethods\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/partners/v1/giftcard/trade/sell/create\n  method: post\n  operationId: createSellTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/partners/v1/giftcard/trade/sell/history\n  method: get\n  operationId: getSellHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prestmit/refs/heads/main/agentic-access/prestmit-agentic-access.yml
summary_line: 31 operations · 9 acting
tags:
- Bills
- Crypto
- Fintech
- Gift Cards
- Payments
---
