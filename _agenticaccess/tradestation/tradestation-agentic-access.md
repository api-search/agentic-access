---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 16
api_specs:
- filename: tradestation-api-openapi.yml
  format: yaml
  label: TradeStation API
  slug: tradestation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradestation/refs/heads/main/openapi/tradestation-api-openapi.yml
- filename: tradestation-streaming-asyncapi.yml
  format: yaml
  label: TradeStation Streaming API
  slug: tradestation-streaming
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradestation/refs/heads/main/asyncapi/tradestation-streaming-asyncapi.yml
consequence_counts:
  physical: 6
  read: 16
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tradestation Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/orderexecution/orderconfirm
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/orderexecution/ordergroupconfirm
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/orderexecution/ordergroups
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/orderexecution/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v3/orderexecution/orders/{orderId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v3/orderexecution/orders/{orderId}
operation_count: 23
overview: 'TradeStation exposes 23 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read, 1 write, and 6 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: TradeStation
provider_slug: tradestation
slug: tradestation-agentic-access
source_filename: tradestation-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/tradestation-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 16\n    acting: 7\n  by_consequence:\n    read: 16\n    write: 1\n    physical: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /v3/brokerage/accounts\n  method: get\n  operationId: getAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/brokerage/accounts/{accountIds}/balances\n  method: get\n  operationId: getBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v3/brokerage/accounts/{accountIds}/bodbalances\n  method: get\n  operationId: getBalancesBOD\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/brokerage/accounts/{accountIds}/positions\n  method: get\n  operationId: getPositions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/brokerage/accounts/{accountIds}/orders\n  method: get\n  operationId: getOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/brokerage/accounts/{accountIds}/historicalorders\n  method: get\n  operationId: getHistoricalOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v3/brokerage/accounts/{accountId}/wallets\n  method: get\n  operationId: getWallets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/marketdata/quotes/{symbols}\n  method: get\n  operationId: getQuotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/marketdata/barcharts/{symbol}\n  method: get\n  operationId: getBars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/marketdata/symbols/{symbols}\n  method: get\n  operationId: getSymbols\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/marketdata/symbollists/cryptopairs/symbolnames\n  method:\
  \ get\n  operationId: getCryptoPairs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/marketdata/options/expirations/{underlying}\n  method: get\n  operationId: getOptionExpirations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/marketdata/options/strikes/{underlying}\n  method: get\n  operationId: getOptionStrikes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/marketdata/options/spreadtypes\n  method: get\n  operationId: getOptionSpreadTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/marketdata/options/riskreward\n  method: post\n  operationId:\
  \ calculateOptionRiskReward\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/orderexecution/orders\n  method: post\n  operationId: placeOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/orderexecution/orders/{orderId}\n  method: put\n  operationId: replaceOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/orderexecution/orders/{orderId}\n  method: delete\n  operationId: cancelOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/orderexecution/orderconfirm\n  method: post\n  operationId: confirmOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/orderexecution/ordergroups\n\
  \  method: post\n  operationId: placeOrderGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/orderexecution/ordergroupconfirm\n  method: post\n  operationId: confirmOrderGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/orderexecution/activationtriggers\n  method: get\n  operationId: getActivationTriggers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/orderexecution/routes\n  method: get\n  operationId: getRoutes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tradestation/refs/heads/main/agentic-access/tradestation-agentic-access.yml
summary_line: 23 operations · 7 acting
tags:
- Brokerage
- Cryptocurrency
- Finance
- Futures
- Market Data
- Options
- Stocks
- Trading
---
