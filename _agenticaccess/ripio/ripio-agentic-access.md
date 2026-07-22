---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 36
api_specs:
- filename: ripio-trade-openapi.yml
  format: yaml
  label: Ripio Trade API v4
  slug: ripio-trade-api-v4
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ripio/refs/heads/main/openapi/ripio-trade-openapi.yml
consequence_counts:
  physical: 8
  read: 36
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ripio Agentic Access
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
  method: DELETE
  path: /orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /orders/all
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /orders/by-external-id
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/cancel-by-external-id
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /withdrawals
operation_count: 46
overview: 'Ripio exposes 46 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 36 read, 2 write, and 8 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Ripio
provider_slug: ripio
slug: ripio-agentic-access
source_filename: ripio-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/ripio-trade-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 46\n  by_action_class:\n    connected: 36\n    acting: 10\n  by_consequence:\n    read: 36\n    physical: 8\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /public/tickers\n  method: get\n  operationId: GetTicker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/tickers/{pair}\n  method: get\n  operationId: GetTickerByPair\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/orders/level-3\n\
  \  method: get\n  operationId: GetPublicOrdersLevel3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/orders/level-2\n  method: get\n  operationId: GetPublicOrdersLevel2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/trades\n  method: get\n  operationId: GetTrades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/currencies\n  method: get\n  operationId: GetCurrencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/pairs\n  method: get\n  operationId: GetPairs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/countries\n  method: get\n  operationId: GetCountries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/server-time\n  method: get\n  operationId: GetServerTime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pairs\n  method: get\n  operationId: GetPairs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trades\n  method: get\n  operationId: GetTrades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /currencies\n  method: get\n\
  \  operationId: GetCurrencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ticker\n  method: get\n  operationId: GetTicker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ticker/{pair}\n  method: get\n  operationId: GetTickerByPair\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /book/orders/level-3\n  method: get\n  operationId: GetBookOrdersLevel3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /book/orders/level-2\n  method: get\n  operationId: GetBookOrdersLevel2\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders\n  method: get\n  operationId: GetUserOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders\n  method: post\n  operationId: CreateOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - Buy/Sell\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders\n  method: delete\n  operationId: CancelOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n   \
  \ - Buy/Sell\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders\n  method: put\n  operationId: UpdatePriceAmountOrderOnMarket\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - Read\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/open\n  method: get\n  operationId: GetUserOpenOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/trades\n  method: get\n  operationId: GetTrades\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{id}\n  method: get\n  operationId: GetOrderById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/by-external-id/{external_id}\n  method: get\n  operationId: GetOrderByExternalId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/cancel\n  method: post\n  operationId: CancelOrderByPost\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - Buy/Sell\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/by-external-id\n  method: delete\n  operationId: CancelOrderByExternalId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - Buy/Sell\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/cancel-by-external-id\n  method: post\n  operationId: CancelOrderByExternalIdByPost\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - Buy/Sell\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/all\n\
  \  method: delete\n  operationId: CancelAllOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - Buy/Sell\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/estimate-price/{pair}\n  method: get\n  operationId: EstimatePrice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deposits\n  method: get\n  operationId: GetUserDeposits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deposits/deposit\n  method: get\n  operationId: GetUserDeposit\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    scope:\n    - Read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /withdrawals\n  method: get\n  operationId: GetUserWithdrawals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /withdrawals\n  method: post\n  operationId: CreateWithdrawal\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - Crypto Withdrawals\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /withdrawals/estimate-fee/{currency_code}\n  method: get\n  operationId: GetWithdrawalFee\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    scope:\n    - Read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /withdrawals/withdrawal\n  method: get\n  operationId: GetUserCryptocurrencyWithdraw\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ticket\n  method: post\n  operationId: GetWebSocketTicket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - Read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/balances\n  method: get\n  operationId: ListBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/balances/{date}\n  method: get\n\
  \  operationId: GetUserBalanceOnDate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/trading-fees\n  method: get\n  operationId: GetUserPairFee\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/statement\n  method: get\n  operationId: GetStatement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/statement/{currency_code}\n  method: get\n  operationId: GetStatementByCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/trades\n  method: get\n  operationId:\
  \ GetUserTrades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/sync\n  method: post\n  operationId: SyncTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - Read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wallets/is-internal\n  method: get\n  operationId: IsInternalWallet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wallets\n  method: get\n  operationId: GetUserWallets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Read\n   \
  \ token:\n      max-ttl: 3600\n    audit: none\n- path: /wallets/{currency_code}/{network}\n  method: get\n  operationId: GetUserWalletAndCreateIfNotExists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Read\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ripio/refs/heads/main/agentic-access/ripio-agentic-access.yml
summary_line: 46 operations · 10 acting
tags:
- Company
- Crypto
- Cryptocurrency
- Exchange
- Trading
- Blockchain
- Latin America
- Bitcoin
- Stablecoins
- API
---
