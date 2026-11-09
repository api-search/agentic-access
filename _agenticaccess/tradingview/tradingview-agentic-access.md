---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 29
api_specs:
- filename: tradingview-account-api-openapi.yml
  format: yaml
  label: TradingView Account API
  slug: tradingview-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tradingview/openapi/tradingview-account-api-openapi.yml
- filename: tradingview-authorization-api-openapi.yml
  format: yaml
  label: TradingView Authorization API
  slug: tradingview-authorization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tradingview/openapi/tradingview-authorization-api-openapi.yml
- filename: tradingview-broker-configuration-api-openapi.yml
  format: yaml
  label: TradingView Broker Configuration API
  slug: tradingview-broker-configuration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tradingview/openapi/tradingview-broker-configuration-api-openapi.yml
- filename: tradingview-data-integration-api-openapi.yml
  format: yaml
  label: TradingView Data Integration API
  slug: tradingview-data-integration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tradingview/openapi/tradingview-data-integration-api-openapi.yml
- filename: tradingview-data-permissions-api-openapi.yml
  format: yaml
  label: TradingView Data Permissions API
  slug: tradingview-data-permissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tradingview/openapi/tradingview-data-permissions-api-openapi.yml
- filename: tradingview-market-data-api-openapi.yml
  format: yaml
  label: TradingView Market Data API
  slug: tradingview-market-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tradingview/openapi/tradingview-market-data-api-openapi.yml
- filename: tradingview-trading-api-openapi.yml
  format: yaml
  label: TradingView Trading API
  slug: tradingview-trading-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tradingview/openapi/tradingview-trading-api-openapi.yml
consequence_counts:
  physical: 6
  read: 29
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tradingview Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/{accountId}/orderInfo
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/{accountId}/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/{accountId}/orders/cancelAll
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /accounts/{accountId}/orders/{orderId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /accounts/{accountId}/orders/{orderId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/{accountId}/previewOrder
operation_count: 47
overview: 'TradingView exposes 47 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 29 read, 12 write, and 6 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: TradingView
provider_slug: tradingview
slug: tradingview-agentic-access
source_filename: tradingview-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/tradingview-broker-rest-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 47\n  by_action_class:\n    acting: 18\n    connected: 29\n  by_consequence:\n    write: 12\n    read: 29\n    physical: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /authorize\n  method: post\n  operationId: authorize\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /logout\n  method: post\n  operationId: logout\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /config\n  method: get\n  operationId: getConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mapping\n  method: get\n  operationId: getMapping\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts\n  method: get\n  operationId: getAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /userInfo\n  method: get\n  operationId: getUserInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /promotionReport\n  method: post\n  operationId: postPromotionReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/instruments\n  method: get\n  operationId: getInstruments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/state\n  method: get\n  operationId: getState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/stream/state\n  method: get\n  operationId: streamState\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/orders\n  method: get\n  operationId: getOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/orders\n  method: post\n  operationId: placeOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/orders/cancelAll\n  method: post\n  operationId: cancelAllOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/stream/orders\n  method: get\n  operationId: streamOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/positions\n  method: get\n  operationId: getPositions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/stream/positions\n  method: get\n  operationId: streamPositions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/netPositions\n  method: get\n  operationId: getNetPositions\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/stream/netPositions\n  method: get\n  operationId: streamNetPositions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/individualPositions\n  method: get\n  operationId: getIndividualPositions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/stream/individualPositions\n  method: get\n  operationId: streamIndividualPositions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/balances\n  method: get\n  operationId: getBalances\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/executions\n  method: get\n  operationId: getExecutions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/ordersHistory\n  method: get\n  operationId: getOrdersHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/getLeverage\n  method: post\n  operationId: getLeverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/setLeverage\n  method: post\n  operationId: setLeverage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/previewLeverage\n  method: post\n  operationId: previewLeverage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/stream/notifications\n  method: get\n  operationId: streamNotifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/orders/{orderId}\n  method: put\n  operationId: modifyOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/orders/{orderId}\n  method: delete\n  operationId: cancelOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/previewOrder\n  method: post\n  operationId: previewOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/previewClosePosition\n  method: post\n  operationId: previewClosePosition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/orderInfo\n  method: post\n  operationId: orderInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/positions/{positionId}\n  method: put\n  operationId: modifyPosition\n  x-agentic-access:\n    action-class: acting\n  \
  \  consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/positions/{positionId}\n  method: delete\n  operationId: closePosition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/netPositions/{netPositionId}\n  method: delete\n  operationId: closeNetPosition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /accounts/{accountId}/individualPositions/{individualPositionId}\n  method: put\n  operationId: modifyIndividualPosition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/individualPositions/{individualPositionId}\n  method: delete\n  operationId: closeIndividualPosition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/trackLatency\n  method: post\n  operationId: trackLatency\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /quotes\n  method: get\n  operationId: getQuotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stream/quotes\n  method: get\n  operationId: streamQuotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /depth\n  method: get\n  operationId: getDepth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stream/depth\n  method: get\n  operationId: streamDepth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /groups\n  method: get\n  operationId: getGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /permissions\n  method: get\n  operationId: getPermissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /symbol_info\n  method: get\n  operationId: getSymbolInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /history\n  method: get\n  operationId: getHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /streaming\n  method: get\n  operationId: streaming\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/tradingview/agentic-access/tradingview-agentic-access.yml
summary_line: 47 operations · 18 acting
tags:
- Company
- Consumer
- Charts
- Charting Library
- Financial Data
- Market Data
- Widgets
- Trading
- Fintech
- Embeddable Components
---
