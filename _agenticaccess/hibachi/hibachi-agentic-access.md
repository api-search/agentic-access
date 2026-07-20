---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 19
api_specs:
- filename: hibachi-openapi.yml
  format: yaml
  label: Hibachi API
  slug: hibachi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hibachi/refs/heads/main/openapi/hibachi-openapi.yml
consequence_counts:
  physical: 8
  read: 19
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Hibachi Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /capital/transfer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /capital/withdraw
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /trade/account/leverage
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /trade/order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /trade/order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /trade/order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /trade/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /trade/orders
operation_count: 27
overview: 'Hibachi exposes 27 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read and 8 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Hibachi
provider_slug: hibachi
slug: hibachi-agentic-access
source_filename: hibachi-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/hibachi-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 27\n  by_action_class:\n    connected: 19\n    acting: 8\n  by_consequence:\n    read: 19\n    physical: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /capital/balance\n  method: get\n  operationId: getCapitalBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /capital/history\n  method: get\n  operationId: getCapitalHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /capital/withdraw\n\
  \  method: post\n  operationId: submitWithdraw\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /capital/transfer\n  method: post\n  operationId: submitTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /capital/deposit-info\n  method: get\n  operationId: getDepositInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /trade/account/info\n  method: get\n  operationId: getAccountInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trade/account/trades\n  method: get\n  operationId: getAccountTrades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trade/account/settlements_history\n  method: get\n  operationId: getSettlementsHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trade/orders\n  method: get\n  operationId: listPendingOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trade/orders\n  method: post\n  operationId: placeOrdersBatch\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /trade/orders\n  method: delete\n  operationId: cancelAllOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /trade/order\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trade/order\n  method: post\n  operationId: placeOrder\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /trade/order\n  method: put\n  operationId: modifyOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /trade/order\n  method: delete\n  operationId: cancelOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n    \
  \  human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /trade/account/leverage\n  method: post\n  operationId: setLeverage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /trade/orders/history\n  method: get\n  operationId: getOrdersHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /market/exchange-info\n  method: get\n  operationId: getExchangeInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /market/inventory\n  method:\
  \ get\n  operationId: getInventory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /market/data/prices\n  method: get\n  operationId: getPrices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /market/data/stats\n  method: get\n  operationId: getStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /market/data/trades\n  method: get\n  operationId: getMarketTrades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /market/data/klines\n  method: get\n  operationId: getKlines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /market/data/open-interest\n  method: get\n  operationId: getOpenInterest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /market/data/orderbook\n  method: get\n  operationId: getOrderbook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /market/data/funding-rates\n  method: get\n  operationId: getFundingRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exchange/utc-timestamp\n  method: get\n  operationId: getUtcTimestamp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hibachi/refs/heads/main/agentic-access/hibachi-agentic-access.yml
summary_line: 27 operations · 8 acting
tags:
- Company
- Defi
- Cryptocurrency
- Exchange
- Perpetual Futures
- Trading
- Derivatives
- Stablecoin
- WebSocket
- Blockchain
---
