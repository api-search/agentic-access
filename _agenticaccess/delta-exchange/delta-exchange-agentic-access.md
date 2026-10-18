---
acting_count: 20
action_class_counts:
  acting: 20
  connected: 30
api_specs:
- filename: delta-exchange-account-api-openapi.yml
  format: yaml
  label: Delta Exchange Account API
  slug: delta-exchange-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delta-exchange/refs/heads/main/openapi/delta-exchange-account-api-openapi.yml
- filename: delta-exchange-assets-api-openapi.yml
  format: yaml
  label: Delta Exchange Assets API
  slug: delta-exchange-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delta-exchange/refs/heads/main/openapi/delta-exchange-assets-api-openapi.yml
- filename: delta-exchange-heartbeat-management-api-openapi.yml
  format: yaml
  label: Delta Exchange Heartbeat Management API
  slug: delta-exchange-heartbeat-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delta-exchange/refs/heads/main/openapi/delta-exchange-heartbeat-management-api-openapi.yml
- filename: delta-exchange-historical-ohlc-candles-sparklines-api-openapi.yml
  format: yaml
  label: Delta Exchange Historical OHLC Candles/Sparklines API
  slug: delta-exchange-historical-ohlc-candles-sparklines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delta-exchange/refs/heads/main/openapi/delta-exchange-historical-ohlc-candles-sparklines-api-openapi.yml
- filename: delta-exchange-indices-api-openapi.yml
  format: yaml
  label: Delta Exchange Indices API
  slug: delta-exchange-indices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delta-exchange/refs/heads/main/openapi/delta-exchange-indices-api-openapi.yml
- filename: delta-exchange-mmp-api-openapi.yml
  format: yaml
  label: Delta Exchange MMP API
  slug: delta-exchange-mmp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delta-exchange/refs/heads/main/openapi/delta-exchange-mmp-api-openapi.yml
- filename: delta-exchange-orderbook-api-openapi.yml
  format: yaml
  label: Delta Exchange Orderbook API
  slug: delta-exchange-orderbook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delta-exchange/refs/heads/main/openapi/delta-exchange-orderbook-api-openapi.yml
- filename: delta-exchange-orders-api-openapi.yml
  format: yaml
  label: Delta Exchange Orders API
  slug: delta-exchange-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delta-exchange/refs/heads/main/openapi/delta-exchange-orders-api-openapi.yml
- filename: delta-exchange-positions-api-openapi.yml
  format: yaml
  label: Delta Exchange Positions API
  slug: delta-exchange-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delta-exchange/refs/heads/main/openapi/delta-exchange-positions-api-openapi.yml
- filename: delta-exchange-products-api-openapi.yml
  format: yaml
  label: Delta Exchange Products API
  slug: delta-exchange-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delta-exchange/refs/heads/main/openapi/delta-exchange-products-api-openapi.yml
- filename: delta-exchange-settlement-prices-api-openapi.yml
  format: yaml
  label: Delta Exchange Settlement Prices API
  slug: delta-exchange-settlement-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delta-exchange/refs/heads/main/openapi/delta-exchange-settlement-prices-api-openapi.yml
- filename: delta-exchange-stats-api-openapi.yml
  format: yaml
  label: Delta Exchange Stats API
  slug: delta-exchange-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delta-exchange/refs/heads/main/openapi/delta-exchange-stats-api-openapi.yml
- filename: delta-exchange-tradehistory-api-openapi.yml
  format: yaml
  label: Delta Exchange Trade History API
  slug: delta-exchange-tradehistory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delta-exchange/refs/heads/main/openapi/delta-exchange-tradehistory-api-openapi.yml
- filename: delta-exchange-trades-api-openapi.yml
  format: yaml
  label: Delta Exchange Trades API
  slug: delta-exchange-trades-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delta-exchange/refs/heads/main/openapi/delta-exchange-trades-api-openapi.yml
- filename: delta-exchange-wallet-api-openapi.yml
  format: yaml
  label: Delta Exchange Wallet API
  slug: delta-exchange-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delta-exchange/refs/heads/main/openapi/delta-exchange-wallet-api-openapi.yml
consequence_counts:
  physical: 12
  read: 30
  safety-critical: 1
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Delta Exchange Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /users/reset_mmp
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /heartbeat
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
  method: POST
  path: /orders/batch
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /orders/batch
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /orders/batch
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/bracket
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /orders/bracket
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /products/{product_id}/orders/leverage
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /wallets/sub_account_balance_transfer
operation_count: 50
overview: 'Delta Exchange exposes 50 API operations that an AI agent could call, of which 20 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 30 read, 7 write, 12 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Delta Exchange
provider_slug: delta-exchange
slug: delta-exchange-agentic-access
source_filename: delta-exchange-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: generated\nsource: openapi/delta-exchange-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 50\n  by_action_class:\n    connected: 30\n    acting: 20\n  by_consequence:\n    read: 30\n    physical: 12\n    write: 7\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /assets\n  method: get\n  operationId: getAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /indices\n  method: get\n  operationId: getIndices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products\n\
  \  method: get\n  operationId: getProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/{symbol}\n  method: get\n  operationId: getProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tickers\n  method: get\n  operationId: getTickers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tickers/{symbol}\n  method: get\n  operationId: getTicker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tickers?contract_types=call_options,put_options&underlying_asset_symbols={underlying_asset_symbols}&expiry_date={expiry_date}\n  method: get\n  operationId: getOptionChain\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders\n  method: post\n  operationId: placeOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders\n  method: delete\n  operationId: cancelOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders\n  method: put\n  operationId: editOrder\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders\n  method: get\n  operationId: getOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/bracket\n  method: post\n  operationId: bracketOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/bracket\n  method: put\n  operationId: bracketOrder\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/all\n  method: delete\n  operationId: cancelAllOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/batch\n  method: post\n  operationId: batchCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/batch\n  method: put\n  operationId: batchEdit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/batch\n  method: delete\n  operationId: batchDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /heartbeat/create\n  method: post\n  operationId: createHeartbeat\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /heartbeat\n  method: post\n  operationId: sendHeartbeat\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /heartbeat\n  method: get\n  operationId: getHeartbeats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{order_id}\n  method: get\n  operationId: getOrderById\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/client_order_id/{client_oid}\n  method: get\n  operationId: getOrderByCOI\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/{product_id}/orders/leverage\n  method: post\n  operationId: changeOrderLeverage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /products/{product_id}/orders/leverage\n  method: get\n  operationId: getOrderLeverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /orders/history\n  method: get\n  operationId: getOrderHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fills\n  method: get\n  operationId: getUserfills\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fills/history/download/csv\n  method: get\n  operationId: downloadFillsHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /positions/margined\n  method: get\n  operationId: getMarginedPositions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /positions\n  method: get\n  operationId: getPositions\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /positions/auto_topup\n  method: put\n  operationId: changeAutoTopup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /positions/change_margin\n  method: post\n  operationId: changePositionMargin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /positions/close_all\n  method: post\n  operationId: closeAllPosition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /l2orderbook/{symbol}\n  method: get\n  operationId: getL2Orderbook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trades/{symbol}\n  method: get\n  operationId: getTrades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wallet/balances\n  method: get\n  operationId: getBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wallet/transactions\n  method: get\n  operationId: getTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /wallet/transactions/download\n  method: get\n  operationId: downloadTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wallets/sub_account_balance_transfer\n  method: post\n  operationId: assetTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wallets/sub_accounts_transfer_history\n  method: get\n  operationId: SubaccountTransferHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/?states=expired\n  method: get\n  operationId:\
  \ getProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /history/candles\n  method: get\n  operationId: getCandles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /history/sparklines\n  method: get\n  operationId: getSparklines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats\n  method: get\n  operationId: getStat\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/update_mmp\n  method: put\n  operationId: updateMMP\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/reset_mmp\n  method: put\n  operationId: resetMMP\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /users/trading_preferences\n  method: get\n  operationId: getTradingPreferences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/trading_preferences\n  method: put\n  operationId: updateTradingPreferences\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sub_accounts\n  method: get\n  operationId: getSubaccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/margin_mode\n  method: put\n  operationId: changeMarginMode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rate_limits/quota\n  method: get\n  operationId: currentRateLimitQuota\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/delta-exchange/refs/heads/main/agentic-access/delta-exchange-agentic-access.yml
summary_line: 50 operations · 20 acting · 1 human-in-the-loop
tags:
- Company
- Cryptocurrency
- Crypto Exchanges
- Derivatives
- Trading
- Options
- Futures
- Market Data
---
