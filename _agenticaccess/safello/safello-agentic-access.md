---
acting_count: 21
action_class_counts:
  acting: 21
  connected: 31
api_specs:
- filename: safello-institutional-openapi.json
  format: json
  label: Safello Institutional API
  slug: safello-institutional-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/safello/refs/heads/main/openapi/safello-institutional-openapi.json
- filename: safello-app-openapi.json
  format: json
  label: Safello App API
  slug: safello-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/safello/refs/heads/main/openapi/safello-app-openapi.json
consequence_counts:
  physical: 11
  read: 31
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Safello Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/email
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/order/sell
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/account/email
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/compliance/verify/orders/buy
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/compliance/verify/orders/sell
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/orders/buy
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/orders/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/orders/sell
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/orders/trade
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/orders/{orderId}/edit
operation_count: 52
overview: 'Safello exposes 52 API operations that an AI agent could call, of which 21 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 31 read, 10 write, and 11 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Safello
provider_slug: safello
slug: safello-agentic-access
source_filename: safello-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/safello-app-openapi.json, openapi/safello-institutional-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 52\n  by_action_class:\n    connected: 31\n    acting: 21\n  by_consequence:\n    read: 31\n    write: 10\n    physical: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /api/prices\n  method: get\n  operationId: getPriceHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/rate\n  method: get\n  operationId: getPrice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n \
  \   audit: none\n- path: /v1/auth\n  method: post\n  operationId: startAuth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth\n  method: get\n  operationId: checkAuthStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/auth/user\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/system/acceptTerms\n  method: post\n  operationId: acceptTerms\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/email\n  method: post\n  operationId: sendVerificationEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/email/verify\n  method: put\n  operationId: verifyEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/kyc/require\n  method: get\n  operationId: requireKyc\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/kyc\n  method: get\n  operationId: kycQuestions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/kyc\n  method: post\n  operationId: answerKYC\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/order\n  method: post\n  operationId: createBuyOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/order\n  method: get\n  operationId: checkOrderStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/order/sell\n  method: post\n  operationId: createSellOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/wallet\n  method: get\n  operationId: getWallet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/market/symbols/crypto\n  method: get\n  operationId: listCryptoSymbols\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    scope:\n    - market\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/market/symbols/fiat\n  method: get\n  operationId: listFiatSymbols\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - market\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/market/symbols/pairs\n  method: get\n  operationId: listTradingPairs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - market\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/market/chart/{pair}\n  method: get\n  operationId: getMarketChart\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - market\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/market/prices/rates/{crypto}\n  method: get\n  operationId: getPrice\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    scope:\n    - market\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/market/prices/rates\n  method: get\n  operationId: getPrices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - market\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/market/ticker/{pair}\n  method: get\n  operationId: getTradePairTicker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - market\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/market/tickers\n  method: get\n  operationId: getTradePairTickers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - market\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/market/best-performers\n  method: get\n  operationId: getBestPerformers\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    scope:\n    - market\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/market/popular-cryptos\n  method: get\n  operationId: getPopularCryptos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - market\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/market/ohlcv\n  method: get\n  operationId: getMarketCandlestickData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - market\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/market/24h-data/{pair}\n  method: get\n  operationId: get24HDataForPair\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - market\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/market/order-book/{pair}\n  method: get\n  operationId: getTradePairOrderBook\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    scope:\n    - market\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth2/bankid\n  method: post\n  operationId: startAuth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth2/token\n  method: post\n  operationId: obtainToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/user\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    -\
  \ account.base\n    - account.base:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/account/terms\n  method: put\n  operationId: acceptTerms\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - account.base\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/email\n  method: post\n  operationId: sendVerificationEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - account.base\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/email\n  method: put\n  operationId: verifyEmail\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - account.base\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/kyc\n  method: get\n  operationId: requireKyc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - account.base\n    - account.base:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/account/kyc-questions\n  method: get\n  operationId: kycQuestions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - account.base\n    - account.base:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/account/kyc-questions\n  method: post\n  operationId: answerKyc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    scope:\n    - account.base\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/bank-account\n  method: get\n  operationId: getBankAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - account.bank-account\n    - account.bank-account:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/account/bank-account\n  method: put\n  operationId: addBankAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - account.bank-account\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/orders\n  method: get\n  operationId: listOrders\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - order\n    - order:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/orders/buy\n  method: post\n  operationId: createBuyOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - order\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/orders/trade\n  method: post\n  operationId: createTradeOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - order\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v2/orders/cancel\n  method: post\n  operationId: cancelTradeOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - order\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/orders/{orderId}/edit\n  method: post\n  operationId: editTradeOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - order\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/orders/sell\n  method: post\n  operationId: createSellOrder\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    scope:\n    - order\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/orders/{orderId}\n  method: get\n  operationId: checkOrderStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - order\n    - order:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/orders/fees\n  method: get\n  operationId: getFees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - order\n    - order:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/wallet\n  method: get\n  operationId: getWallet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  scope:\n    - wallet\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/wallet/performance\n  method: get\n  operationId: getWalletPerformance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - wallet\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/wallet/performance-history\n  method: get\n  operationId: getWalletPerformanceHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - wallet\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/compliance/verify/orders/sell\n  method: post\n  operationId: verifySellOrderCompliance\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - order\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v2/compliance/verify/orders/buy\n  method: post\n  operationId: verifyBuyOrderCompliance\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - order\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/safello/refs/heads/main/agentic-access/safello-agentic-access.yml
summary_line: 52 operations · 21 acting
tags:
- Company
- Fintech
- Cryptocurrency
- Bitcoin
- Brokerage
- Payments
- Sweden
- Trading
- KYC
- BankID
---
