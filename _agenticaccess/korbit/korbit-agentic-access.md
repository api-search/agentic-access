---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 27
api_specs:
- filename: korbit-openapi.yml
  format: yaml
  label: Korbit Open API v2
  slug: korbit-open-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/korbit/refs/heads/main/openapi/korbit-openapi.yml
- filename: korbit-websocket-asyncapi.yml
  format: yaml
  label: Korbit Open API v2 WebSocket
  slug: korbit-open-api-v2-websocket
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/korbit/refs/heads/main/asyncapi/korbit-websocket-asyncapi.yml
consequence_counts:
  physical: 7
  read: 27
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Korbit Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/coin/depositAddress
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/coin/withdrawal
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v2/coin/withdrawal
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/krw/sendKrwDepositPush
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/krw/sendKrwWithdrawalPush
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v2/orders
operation_count: 34
overview: 'Korbit exposes 34 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 27 read and 7 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Korbit
provider_slug: korbit
slug: korbit-agentic-access
source_filename: korbit-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/korbit-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 34\n  by_action_class:\n    connected: 27\n    acting: 7\n  by_consequence:\n    read: 27\n    physical: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/tickers\n  method: get\n  operationId: getTickers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/orderbook\n  method: get\n  operationId: getOrderbook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/trades\n  method: get\n  operationId:\
  \ getTrades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/candles\n  method: get\n  operationId: getCandles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/currencyPairs\n  method: get\n  operationId: getCurrencyPairs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/tickSizePolicy\n  method: get\n  operationId: getTickSizePolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/orders\n  method: get\n  operationId: getOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v2/orders\n  method: post\n  operationId: createOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/orders\n  method: delete\n  operationId: deleteOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/openOrders\n  method: get\n  operationId: getOpenOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v2/allOrders\n  method: get\n  operationId: getAllOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/myTrades\n  method: get\n  operationId: getMyTrades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/balance\n  method: get\n  operationId: getBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/coin/depositAddresses\n  method: get\n  operationId: getCoinDepositAddresses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/coin/depositAddress\n  method: get\n  operationId: getCoinDepositAddress\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/coin/depositAddress\n  method: post\n  operationId: createCoinDepositAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/coin/recentDeposits\n  method: get\n  operationId: getCoinRecentDeposits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/coin/deposit\n  method: get\n  operationId: getCoinDeposit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /v2/coin/withdrawableAddresses\n  method: get\n  operationId: getCoinWithdrawableAddresses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/coin/withdrawableAmount\n  method: get\n  operationId: getCoinWithdrawableAmount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/coin/withdrawal\n  method: post\n  operationId: createCoinWithdrawal\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/coin/withdrawal\n  method: delete\n  operationId: deleteCoinWithdrawal\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/coin/withdrawal\n  method: get\n  operationId: getCoinWithdrawal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/coin/recentWithdrawals\n  method: get\n  operationId: getCoinRecentWithdrawals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/krw/sendKrwDepositPush\n  method: post\n  operationId: createKrwSendKrwDepositPush\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/krw/sendKrwWithdrawalPush\n  method: post\n  operationId: createKrwSendKrwWithdrawalPush\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/krw/recentDeposits\n  method: get\n  operationId: getKrwRecentDeposits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/krw/recentWithdrawals\n  method: get\n  operationId: getKrwRecentWithdrawals\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/currencies\n  method: get\n  operationId: getCurrencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/time\n  method: get\n  operationId: getTime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/tradingFeePolicy\n  method: get\n  operationId: getTradingFeePolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/currentKeyInfo\n  method: get\n  operationId: getCurrentKeyInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/notices\n  method: get\n\
  \  operationId: getNotices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/marketAlerts\n  method: get\n  operationId: getMarketAlerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/korbit/refs/heads/main/agentic-access/korbit-agentic-access.yml
summary_line: 34 operations · 7 acting
tags:
- Company
- Crypto
- Cryptocurrency Exchange
- Digital Assets
- Trading
- Market Data
- Financial Services
- WebSocket
- South Korea
- Blockchain
---
