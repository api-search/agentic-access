---
acting_count: 45
action_class_counts:
  acting: 45
  connected: 26
api_specs:
- filename: kraken-spot-rest-openapi.yml
  format: yaml
  label: Kraken Spot REST API
  slug: kraken-spot-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kraken/refs/heads/main/openapi/kraken-spot-rest-openapi.yml
- filename: kraken-asyncapi.yml
  format: yaml
  label: Kraken Spot WebSocket API v2
  slug: kraken-spot-websocket-api-v2
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/kraken/refs/heads/main/asyncapi/kraken-asyncapi.yml
- filename: kraken-futures-rest-openapi.yml
  format: yaml
  label: Kraken Futures REST API
  slug: kraken-futures-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kraken/refs/heads/main/openapi/kraken-futures-rest-openapi.yml
consequence_counts:
  physical: 32
  read: 26
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Kraken Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /0/private/AccountTransfer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /0/private/AddOrder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /0/private/AddOrderBatch
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /0/private/AmendOrder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /0/private/CancelAll
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /0/private/CancelAllOrdersAfter
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /0/private/CancelOrder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /0/private/CancelOrderBatch
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /0/private/ClosedOrders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /0/private/DepositAddresses
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /0/private/DepositMethods
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /0/private/DepositStatus
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /0/private/EditOrder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /0/private/OpenOrders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /0/private/QueryOrders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /0/private/QueryTrades
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /0/private/TradeBalance
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /0/private/TradeVolume
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /0/private/TradesHistory
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /0/private/WalletTransfer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /0/private/Withdraw
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /0/private/WithdrawCancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /0/private/WithdrawInfo
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /0/private/WithdrawStatus
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /batchorder
operation_count: 71
overview: 'Kraken exposes 71 API operations that an AI agent could call, of which 45 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 26 read, 13 write, and 32 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Kraken
provider_slug: kraken
slug: kraken-agentic-access
source_filename: kraken-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/kraken-futures-rest-openapi.yml, openapi/kraken-spot-rest-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 71\n  by_action_class:\n    connected: 26\n    acting: 45\n  by_consequence:\n    read: 26\n    physical: 32\n    write: 13\n  human_in_the_loop_required: 0\noperations:\n- path: /instruments\n  method: get\n  operationId: getInstruments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instruments/status\n  method: get\n  operationId: getInstrumentsStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /tickers\n  method: get\n  operationId: getTickers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tickers/{symbol}\n  method: get\n  operationId: getTickerForSymbol\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orderbook\n  method: get\n  operationId: getOrderBookFutures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /history\n  method: get\n  operationId: getMarketHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts\n  method: get\n  operationId: getAccounts\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openpositions\n  method: get\n  operationId: getOpenPositionsFutures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openorders\n  method: get\n  operationId: getOpenOrdersFutures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fills\n  method: get\n  operationId: getFills\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sendorder\n  method: post\n  operationId: sendOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /editorder\n  method: post\n  operationId: editOrderFutures\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cancelorder\n  method: post\n  operationId: cancelOrderFutures\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cancelallorders\n  method: post\n  operationId:\
  \ cancelAllOrdersFutures\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cancelallordersafter\n  method: post\n  operationId: cancelAllOrdersAfterFutures\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /batchorder\n  method: post\n  operationId: batchOrderFutures\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n\
  \      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transfer\n  method: post\n  operationId: transferFutures\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /withdrawal\n  method: post\n  operationId: withdrawalFutures\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /notifications\n\
  \  method: get\n  operationId: getNotifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /historicalorders\n  method: get\n  operationId: getHistoricalOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /historicalexecutions\n  method: get\n  operationId: getHistoricalExecutions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /historicaltriggers\n  method: get\n  operationId: getHistoricalTriggers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accountlog\n  method: get\n  operationId: getAccountLog\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /charts/{tickSize}/{symbol}/{interval}\n  method: get\n  operationId: getChartCandles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apikey/v3\n  method: get\n  operationId: checkApiKeyV3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /0/public/Time\n  method: get\n  operationId: getServerTime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /0/public/SystemStatus\n  method: get\n  operationId: getSystemStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /0/public/Assets\n\
  \  method: get\n  operationId: getAssetInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /0/public/AssetPairs\n  method: get\n  operationId: getTradableAssetPairs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /0/public/Ticker\n  method: get\n  operationId: getTickerInformation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /0/public/OHLC\n  method: get\n  operationId: getOHLCData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /0/public/Depth\n  method: get\n  operationId: getOrderBook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /0/public/Trades\n  method: get\n  operationId: getRecentTrades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /0/public/Spread\n  method: get\n  operationId: getRecentSpreads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /0/private/Balance\n  method: post\n  operationId: getAccountBalance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /0/private/BalanceEx\n  method: post\n  operationId: getExtendedBalance\n  x-agentic-access:\n    action-class: acting\n   \
  \ consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /0/private/TradeBalance\n  method: post\n  operationId: getTradeBalance\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /0/private/OpenOrders\n  method: post\n  operationId: getOpenOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /0/private/ClosedOrders\n  method: post\n  operationId: getClosedOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /0/private/QueryOrders\n  method: post\n  operationId: queryOrdersInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /0/private/TradesHistory\n  method: post\n  operationId: getTradesHistory\n  x-agentic-access:\n    action-class: acting\n  \
  \  consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /0/private/QueryTrades\n  method: post\n  operationId: queryTradesInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /0/private/OpenPositions\n  method: post\n  operationId: getOpenPositions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n  \
  \    - abnormal\n      - high-value\n    audit: required\n- path: /0/private/Ledgers\n  method: post\n  operationId: getLedgersInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /0/private/QueryLedgers\n  method: post\n  operationId: queryLedgers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /0/private/TradeVolume\n  method: post\n  operationId: getTradeVolume\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /0/private/AddOrder\n  method: post\n  operationId: addOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /0/private/AddOrderBatch\n  method: post\n  operationId: addOrderBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /0/private/EditOrder\n\
  \  method: post\n  operationId: editOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /0/private/AmendOrder\n  method: post\n  operationId: amendOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /0/private/CancelOrder\n  method: post\n  operationId: cancelOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /0/private/CancelAll\n  method: post\n  operationId: cancelAllOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /0/private/CancelAllOrdersAfter\n  method: post\n  operationId: cancelAllOrdersAfter\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /0/private/CancelOrderBatch\n  method: post\n  operationId: cancelOrderBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /0/private/DepositMethods\n  method: post\n  operationId: getDepositMethods\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /0/private/DepositAddresses\n  method: post\n  operationId: getDepositAddresses\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /0/private/DepositStatus\n  method: post\n  operationId: getDepositStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /0/private/WithdrawInfo\n  method: post\n  operationId: getWithdrawalInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /0/private/Withdraw\n  method: post\n  operationId: withdrawFunds\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /0/private/WithdrawStatus\n  method: post\n  operationId: getWithdrawalStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /0/private/WithdrawCancel\n  method: post\n  operationId: cancelWithdrawal\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /0/private/WalletTransfer\n  method: post\n  operationId: walletTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /0/private/CreateSubaccount\n  method: post\n  operationId: createSubaccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n   \
  \   human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /0/private/AccountTransfer\n  method: post\n  operationId: accountTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /0/private/Earn/Allocate\n  method: post\n  operationId: allocateEarnFunds\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /0/private/Earn/Deallocate\n  method: post\n  operationId: deallocateEarnFunds\n  x-agentic-access:\n \
  \   action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /0/private/Earn/AllocateStatus\n  method: post\n  operationId: getEarnAllocateStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /0/private/Earn/DeallocateStatus\n  method: post\n  operationId: getEarnDeallocateStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /0/private/Earn/Strategies\n  method: post\n  operationId: listEarnStrategies\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /0/private/Earn/Allocations\n  method: post\n  operationId: listEarnAllocations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /0/private/GetWebSocketsToken\n  method: post\n  operationId: getWebSocketsToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kraken/refs/heads/main/agentic-access/kraken-agentic-access.yml
summary_line: 71 operations · 45 acting
tags:
- Cryptocurrency
- Exchange
- Trading
- Market Data
- Spot Trading
- Futures
- Derivatives
- Staking
- Earn
- NFT
- WebSocket
- FIX
- Custody
- OTC
- Prime Brokerage
- Embed
- OAuth
- Public APIs
---
