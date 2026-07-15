---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 6
api_specs:
- filename: llms.txt
  format: yaml
  label: Bithumb REST API
  slug: bithumb-rest-api
  spec_type: OpenAPI
  url: https://apidocs.bithumb.com/llms.txt
consequence_counts:
  physical: 12
  read: 6
  write: 1
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
  path: /spot/myTrades
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /spot/openOrders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /spot/orderDetail
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /spot/orderList
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
  path: /spot/singleOrder
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
overview: 'Bithumb exposes 19 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 1 write, and 12 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bithumb
provider_slug: bithumb
slug: bithumb-agentic-access
source_filename: bithumb-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    connected: 6\n    acting: 13\n  by_consequence:\n    read: 6\n    physical: 12\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /serverTime\n  method: get\n  operationId: getServerTime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spot/config\n  method: get\n  operationId: getSpotConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spot/ticker\n  method: get\n\
  \  operationId: getSpotTicker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spot/orderBook\n  method: get\n  operationId: getSpotOrderBook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spot/trades\n  method: get\n  operationId: getSpotTrades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spot/kline\n  method: get\n  operationId: getSpotKline\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spot/placeOrder\n  method: post\n  operationId: placeSpotOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spot/cancelOrder\n  method: post\n  operationId: cancelSpotOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spot/cancelOrder/batch\n  method: post\n  operationId: batchCancelSpotOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /spot/placeOrders\n  method: post\n  operationId: batchPlaceSpotOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spot/singleOrder\n  method: post\n  operationId: getSpotSingleOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spot/openOrders\n  method: post\n  operationId: getSpotOpenOrders\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spot/orderList\n  method: post\n  operationId: getSpotOrderList\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spot/orderDetail\n  method: post\n  operationId: getSpotOrderDetail\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spot/myTrades\n  method: post\n  operationId: getSpotMyTrades\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spot/assetList\n  method: post\n  operationId: getSpotAssetList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wallet/depositHistory\n  method: post\n  operationId: getDepositHistory\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wallet/withdrawHistory\n  method: post\n  operationId: getWithdrawHistory\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /withdraw\n  method: post\n  operationId: submitWithdraw\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bithumb/refs/heads/main/agentic-access/bithumb-agentic-access.yml
summary_line: 19 operations · 13 acting
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
