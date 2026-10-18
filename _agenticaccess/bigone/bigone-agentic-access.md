---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 37
api_specs:
- filename: bigone-account-api-openapi.yml
  format: yaml
  label: BigONE Account API
  slug: bigone-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigone/refs/heads/main/openapi/bigone-account-api-openapi.yml
- filename: bigone-asset-api-openapi.yml
  format: yaml
  label: BigONE Asset API
  slug: bigone-asset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigone/refs/heads/main/openapi/bigone-asset-api-openapi.yml
- filename: bigone-assets-api-openapi.yml
  format: yaml
  label: BigONE Assets API
  slug: bigone-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigone/refs/heads/main/openapi/bigone-assets-api-openapi.yml
- filename: bigone-deposit-api-openapi.yml
  format: yaml
  label: BigONE Deposit API
  slug: bigone-deposit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigone/refs/heads/main/openapi/bigone-deposit-api-openapi.yml
- filename: bigone-funding-account-api-openapi.yml
  format: yaml
  label: BigONE Funding Account API
  slug: bigone-funding-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigone/refs/heads/main/openapi/bigone-funding-account-api-openapi.yml
- filename: bigone-market-data-api-openapi.yml
  format: yaml
  label: BigONE Market Data API
  slug: bigone-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigone/refs/heads/main/openapi/bigone-market-data-api-openapi.yml
- filename: bigone-order-api-openapi.yml
  format: yaml
  label: BigONE Order API
  slug: bigone-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigone/refs/heads/main/openapi/bigone-order-api-openapi.yml
- filename: bigone-ping-api-openapi.yml
  format: yaml
  label: BigONE Ping API
  slug: bigone-ping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigone/refs/heads/main/openapi/bigone-ping-api-openapi.yml
- filename: bigone-position-api-openapi.yml
  format: yaml
  label: BigONE Position API
  slug: bigone-position-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigone/refs/heads/main/openapi/bigone-position-api-openapi.yml
- filename: bigone-quote-api-openapi.yml
  format: yaml
  label: BigONE Quote API
  slug: bigone-quote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigone/refs/heads/main/openapi/bigone-quote-api-openapi.yml
- filename: bigone-ranges-api-openapi.yml
  format: yaml
  label: BigONE Ranges API
  slug: bigone-ranges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigone/refs/heads/main/openapi/bigone-ranges-api-openapi.yml
- filename: bigone-trade-api-openapi.yml
  format: yaml
  label: BigONE Trade API
  slug: bigone-trade-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigone/refs/heads/main/openapi/bigone-trade-api-openapi.yml
- filename: bigone-trades-api-openapi.yml
  format: yaml
  label: BigONE Trades API
  slug: bigone-trades-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigone/refs/heads/main/openapi/bigone-trades-api-openapi.yml
- filename: bigone-transfer-api-openapi.yml
  format: yaml
  label: BigONE Transfer API
  slug: bigone-transfer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigone/refs/heads/main/openapi/bigone-transfer-api-openapi.yml
- filename: bigone-withdrawal-api-openapi.yml
  format: yaml
  label: BigONE Withdrawal API
  slug: bigone-withdrawal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigone/refs/heads/main/openapi/bigone-withdrawal-api-openapi.yml
consequence_counts:
  physical: 11
  read: 37
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bigone Agentic Access
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
  path: /orders/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /viewer/order/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /viewer/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /viewer/orders/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /viewer/orders/multi
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /viewer/orders/{id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /viewer/trade
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /viewer/transfer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /viewer/withdrawals
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /viewer/withdrawals/{guid}/cancel
operation_count: 50
overview: 'BigONE exposes 50 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 37 read, 2 write, and 11 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BigONE
provider_slug: bigone
slug: bigone-agentic-access
source_filename: bigone-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: generated\nsource: openapi/bigone-contract-openapi.yml, openapi/bigone-convert-openapi.yml, openapi/bigone-server-openapi.yml,\n  openapi/bigone-spot-openapi.yml, openapi/bigone-wallet-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 50\n  by_action_class:\n    connected: 37\n    acting: 13\n  by_consequence:\n    read: 37\n    write: 2\n    physical: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /instruments\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /depth@{symbol}/snapshot\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /positions/{symbol}/margin\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /positions/{symbol}/risk-limit\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/opening\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{id}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/count\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/opening/count\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trades\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trades/count\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets\n  method: get\n  operationId: getConvertAssets\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /range\n  method: get\n  operationId: getConvertRange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /viewer/quote\n  method: get\n  operationId: getConvertQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /viewer/trade\n  method: post\n  operationId: createConvertTrade\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viewer/trade\n  method: get\n  operationId:\
  \ getConvertTradeDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /viewer/trades\n  method: get\n  operationId: getConvertTrades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ping\n  method: get\n  operationId: getPing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset_pairs\n  method: get\n  operationId: getAssetPairs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset_pairs/{asset_pair_name}/ticker\n  method: get\n  operationId: getTicker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /asset_pairs/tickers\n  method: get\n  operationId: getTickers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset_pairs/{asset_pair_name}/depth\n  method: get\n  operationId: getDepth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset_pairs/{asset_pair_name}/trades\n  method: get\n  operationId: getMarketTrades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset_pairs/{asset_pair_name}/candles\n  method: get\n  operationId: getCandles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /viewer/accounts\n  method:\
  \ get\n  operationId: getAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /viewer/accounts/{asset_symbol}\n  method: get\n  operationId: getAccountBySymbol\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /viewer/orders\n  method: get\n  operationId: getOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /viewer/orders\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /viewer/orders/{id}\n  method: get\n  operationId: getOrderById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /viewer/order\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /viewer/orders/multi\n  method: post\n  operationId: createMultiOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viewer/orders/{id}/cancel\n  method: post\n  operationId: cancelOrderByIdPath\n  x-agentic-access:\n    action-class: acting\n  \
  \  consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viewer/order/cancel\n  method: post\n  operationId: cancelOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viewer/orders/cancel\n  method: post\n  operationId: cancelAllOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viewer/trades\n  method: get\n  operationId: getUserTrades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /viewer/trading_fees\n  method: get\n  operationId: getTradingFees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets\n  method: get\n  operationId: getAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /viewer/fund/accounts\n  method: get\n  operationId: getFundingAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - view account balance information\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /viewer/fund/accounts/{asset_symbol}\n  method: get\n  operationId: getFundingAccountBySymbol\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - view account balance information\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /viewer/transfer\n  method: get\n  operationId: getTransfer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - view account balance information\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /viewer/transfer\n  method: post\n  operationId: createTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - view account balance information\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /viewer/deposits\n  method: get\n  operationId: getDeposits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - view deposit history\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /viewer/assets/{asset_symbol}/address\n  method: get\n  operationId: getDepositAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - view deposit address\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /viewer/withdrawals\n  method: get\n  operationId: getWithdrawal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - view withdrawal history\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /viewer/withdrawals\n  method: post\n  operationId: createWithdrawal\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    scope:\n    - execute withdrawals\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viewer/withdrawals/{guid}\n  method: get\n  operationId: getWithdrawalByGuid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - view withdrawal history\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /viewer/withdrawals/{guid}/cancel\n  method: post\n  operationId: cancelWithdrawalByGuid\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - execute withdrawals\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bigone/refs/heads/main/agentic-access/bigone-agentic-access.yml
summary_line: 50 operations · 13 acting
tags:
- Company
- Cryptocurrency
- Exchange
- Trading
- Derivatives
- Wallets
- Market Data
---
