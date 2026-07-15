---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 8
api_specs:
- filename: lbank-spot-market-rest-api.json
  format: json
  label: LBank Spot Market REST API
  slug: spot-market-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lbank/refs/heads/main/openapi/lbank-spot-market-rest-api.json
- filename: lbank-spot-trading-rest-api.json
  format: json
  label: LBank Spot Trading REST API
  slug: spot-trading-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lbank/refs/heads/main/openapi/lbank-spot-trading-rest-api.json
- filename: lbank-wallet-rest-api.json
  format: json
  label: LBank Wallet REST API
  slug: wallet-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lbank/refs/heads/main/openapi/lbank-wallet-rest-api.json
consequence_counts:
  physical: 9
  read: 8
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Lbank Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/cancel_order.do
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/create_order.do
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/order_transaction_detail.do
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/orders_info.do
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/orders_info_history.do
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/orders_info_no_deal.do
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/withdraw.do
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/withdrawCancel.do
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/withdraws.do
operation_count: 19
overview: 'LBank exposes 19 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 2 write, and 9 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: LBank
provider_slug: lbank
slug: lbank-agentic-access
source_filename: lbank-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/lbank-spot-market-rest-api.json, openapi/lbank-spot-trading-rest-api.json, openapi/lbank-wallet-rest-api.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    connected: 8\n    acting: 11\n  by_consequence:\n    read: 8\n    write: 2\n    physical: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/ticker.do\n  method: get\n  operationId: getMarketTicker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/currencyPairs.do\n  method: get\n  operationId: getCurrencyPairs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/depth.do\n  method: get\n  operationId: getMarketDepth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/trades.do\n  method: get\n  operationId: getHistoricalTrades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/kline.do\n  method: get\n  operationId: getKlineData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accuracy.do\n  method: get\n  operationId: getTradingPairInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/usdToCny.do\n  method: get\n  operationId: getUsdToCnyRate\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/user_info.do\n  method: post\n  operationId: getUserInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/create_order.do\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/cancel_order.do\n  method: post\n  operationId: cancelOrder\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/orders_info.do\n  method: post\n  operationId: getOrderInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/orders_info_history.do\n  method: post\n  operationId: getOrderHistory\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/orders_info_no_deal.do\n  method: post\n  operationId: getOpenOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/order_transaction_detail.do\n  method: post\n  operationId: getOrderTransactionDetail\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transaction_history.do\n  method:\
  \ post\n  operationId: getTransactionHistory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/withdrawConfigs.do\n  method: get\n  operationId: getWithdrawConfigs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/withdraw.do\n  method: post\n  operationId: withdraw\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/withdrawCancel.do\n  method: post\n  operationId:\
  \ cancelWithdraw\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/withdraws.do\n  method: post\n  operationId: getWithdrawalHistory\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lbank/refs/heads/main/agentic-access/lbank-agentic-access.yml
summary_line: 19 operations · 11 acting
tags:
- Cryptocurrency
- Exchange
- Trading
- Market Data
- Finance
- Blockchain
---
