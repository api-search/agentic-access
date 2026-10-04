---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 12
api_specs:
- filename: bithumb-account-api-openapi.yml
  format: yaml
  label: Bithumb Account API
  slug: bithumb-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bithumb/refs/heads/main/openapi/bithumb-account-api-openapi.yml
- filename: bithumb-general-api-openapi.yml
  format: yaml
  label: Bithumb General API
  slug: bithumb-general-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bithumb/refs/heads/main/openapi/bithumb-general-api-openapi.yml
- filename: bithumb-market-data-api-openapi.yml
  format: yaml
  label: Bithumb Market Data API
  slug: bithumb-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bithumb/refs/heads/main/openapi/bithumb-market-data-api-openapi.yml
- filename: bithumb-spot-trading-api-openapi.yml
  format: yaml
  label: Bithumb Spot Trading API
  slug: bithumb-spot-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bithumb/refs/heads/main/openapi/bithumb-spot-trading-api-openapi.yml
- filename: bithumb-wallet-api-openapi.yml
  format: yaml
  label: Bithumb Wallet API
  slug: bithumb-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bithumb/refs/heads/main/openapi/bithumb-wallet-api-openapi.yml
consequence_counts:
  physical: 7
  read: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bithumb Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /spot/cancelOrder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /spot/cancelOrder/batch
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /spot/placeOrder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /spot/placeOrders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /wallet/depositHistory
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /wallet/withdrawHistory
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /withdraw
operation_count: 19
overview: 'Bithumb exposes 19 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read and 7 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bithumb
provider_slug: bithumb
slug: bithumb-agentic-access
source_filename: bithumb-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/bithumb-account-api-openapi.yml, openapi/bithumb-general-api-openapi.yml, openapi/bithumb-market-data-api-openapi.yml,\n  openapi/bithumb-spot-trading-api-openapi.yml, openapi/bithumb-wallet-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    connected: 12\n    acting: 7\n  by_consequence:\n    read: 12\n    physical: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /spot/assetList\n  method: post\n  operationId: getSpotAssetList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /serverTime\n  method: get\n  operationId: getServerTime\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spot/config\n  method: get\n  operationId: getSpotConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spot/ticker\n  method: get\n  operationId: getSpotTicker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spot/orderBook\n  method: get\n  operationId: getSpotOrderBook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spot/trades\n  method: get\n  operationId: getSpotTrades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /spot/kline\n  method: get\n  operationId: getSpotKline\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spot/placeOrder\n  method: post\n  operationId: placeSpotOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spot/cancelOrder\n  method: post\n  operationId: cancelSpotOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /spot/cancelOrder/batch\n  method: post\n  operationId: batchCancelSpotOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spot/placeOrders\n  method: post\n  operationId: batchPlaceSpotOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spot/singleOrder\n  method: post\n  operationId: getSpotSingleOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spot/openOrders\n  method: post\n  operationId: getSpotOpenOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spot/orderList\n  method: post\n  operationId: getSpotOrderList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spot/orderDetail\n  method: post\n  operationId: getSpotOrderDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spot/myTrades\n  method: post\n  operationId: getSpotMyTrades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wallet/depositHistory\n  method:\
  \ post\n  operationId: getDepositHistory\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wallet/withdrawHistory\n  method: post\n  operationId: getWithdrawHistory\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /withdraw\n  method: post\n  operationId: submitWithdraw\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bithumb/refs/heads/main/agentic-access/bithumb-agentic-access.yml
summary_line: 19 operations · 7 acting
tags:
- Cryptocurrency
- Exchange
- Trading
- South Korea
- KRW
- Bitcoin
- Market Data
- WebSocket
---
