---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 24
api_specs:
- filename: gmx-allowances-api-openapi.yml
  format: yaml
  label: GMX Allowances API
  slug: gmx-allowances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmx/refs/heads/main/openapi/gmx-allowances-api-openapi.yml
- filename: gmx-apy-api-openapi.yml
  format: yaml
  label: GMX APY API
  slug: gmx-apy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmx/refs/heads/main/openapi/gmx-apy-api-openapi.yml
- filename: gmx-balances-api-openapi.yml
  format: yaml
  label: GMX Balances API
  slug: gmx-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmx/refs/heads/main/openapi/gmx-balances-api-openapi.yml
- filename: gmx-buyback-api-openapi.yml
  format: yaml
  label: GMX Buyback API
  slug: gmx-buyback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmx/refs/heads/main/openapi/gmx-buyback-api-openapi.yml
- filename: gmx-gmx-account-api-openapi.yml
  format: yaml
  label: GMX GMX Account API
  slug: gmx-gmx-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmx/refs/heads/main/openapi/gmx-gmx-account-api-openapi.yml
- filename: gmx-jit-api-openapi.yml
  format: yaml
  label: GMX JIT API
  slug: gmx-jit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmx/refs/heads/main/openapi/gmx-jit-api-openapi.yml
- filename: gmx-markets-api-openapi.yml
  format: yaml
  label: GMX Markets API
  slug: gmx-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmx/refs/heads/main/openapi/gmx-markets-api-openapi.yml
- filename: gmx-order-transactions-api-openapi.yml
  format: yaml
  label: GMX Order Transactions API
  slug: gmx-order-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmx/refs/heads/main/openapi/gmx-order-transactions-api-openapi.yml
- filename: gmx-orders-api-openapi.yml
  format: yaml
  label: GMX Orders API
  slug: gmx-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmx/refs/heads/main/openapi/gmx-orders-api-openapi.yml
- filename: gmx-pairs-api-openapi.yml
  format: yaml
  label: GMX Pairs API
  slug: gmx-pairs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmx/refs/heads/main/openapi/gmx-pairs-api-openapi.yml
- filename: gmx-performance-api-openapi.yml
  format: yaml
  label: GMX Performance API
  slug: gmx-performance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmx/refs/heads/main/openapi/gmx-performance-api-openapi.yml
- filename: gmx-positions-api-openapi.yml
  format: yaml
  label: GMX Positions API
  slug: gmx-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmx/refs/heads/main/openapi/gmx-positions-api-openapi.yml
- filename: gmx-prices-api-openapi.yml
  format: yaml
  label: GMX Prices API
  slug: gmx-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmx/refs/heads/main/openapi/gmx-prices-api-openapi.yml
- filename: gmx-rates-api-openapi.yml
  format: yaml
  label: GMX Rates API
  slug: gmx-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmx/refs/heads/main/openapi/gmx-rates-api-openapi.yml
- filename: gmx-staking-api-openapi.yml
  format: yaml
  label: GMX Staking API
  slug: gmx-staking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmx/refs/heads/main/openapi/gmx-staking-api-openapi.yml
- filename: gmx-subaccounts-api-openapi.yml
  format: yaml
  label: GMX Subaccounts API
  slug: gmx-subaccounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmx/refs/heads/main/openapi/gmx-subaccounts-api-openapi.yml
- filename: gmx-tokens-api-openapi.yml
  format: yaml
  label: GMX Tokens API
  slug: gmx-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmx/refs/heads/main/openapi/gmx-tokens-api-openapi.yml
- filename: gmx-trades-api-openapi.yml
  format: yaml
  label: GMX Trades API
  slug: gmx-trades-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gmx/refs/heads/main/openapi/gmx-trades-api-openapi.yml
consequence_counts:
  physical: 11
  read: 24
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Gmx Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /gmx-account/deposit/cross-chain/prepare
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /gmx-account/withdraw/cross-chain/prepare
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /gmx-account/withdraw/cross-chain/status
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /gmx-account/withdraw/cross-chain/submit
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/txns/cancel/prepare
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/txns/collateral/prepare
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/txns/edit/prepare
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/txns/prepare
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/txns/status
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/txns/submit
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /trades/search
operation_count: 37
overview: 'GMX exposes 37 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 24 read, 2 write, and 11 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: GMX
provider_slug: gmx
slug: gmx-agentic-access
source_filename: gmx-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 37\n  by_action_class:\n    connected: 24\n    acting: 13\n  by_consequence:\n    read: 24\n    physical: 11\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /trades\n  method: get\n  operationId: GetTrades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trades/search\n  method: post\n  operationId: SearchTrades\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tokens\n  method: get\n  operationId: GetTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tokens/info\n  method: get\n  operationId: GetTokensInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subaccounts/status\n  method: post\n  operationId: FetchStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subaccounts/approval/prepare\n  method: post\n  operationId: PrepareApproval\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /staking/power\n  method: get\n  operationId: GetStakingPower\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rates\n  method: get\n  operationId: GetRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /prices/ohlcv\n  method: get\n  operationId: GetOhlcv\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /positions\n  method: get\n  operationId: GetPositionsInfo\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /positions/{key}\n  method: get\n  operationId: GetPositionByKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /performance/annualized\n  method: get\n  operationId: GetAnnualized\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /performance/snapshots\n  method: get\n  operationId: GetSnapshots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pairs\n  method: get\n  operationId: GetPairs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders\n  method: get\n  operationId:\
  \ GetOrdersByAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{key}\n  method: get\n  operationId: GetOrderByKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/txns/prepare\n  method: post\n  operationId: Prepare\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/txns/submit\n  method: post\n  operationId: Submit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n\
  \      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/txns/status\n  method: post\n  operationId: Status\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/txns/edit/prepare\n  method: post\n  operationId: EditPrepare\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /orders/txns/cancel/prepare\n  method: post\n  operationId: CancelPrepare\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/txns/collateral/prepare\n  method: post\n  operationId: CollateralPrepare\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /markets\n  method: get\n  operationId: GetMarkets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /markets/tickers\n  method: get\n  operationId: GetMarketsTickers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/info\n  method: get\n  operationId: GetMarketsInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/config\n  method: get\n  operationId: GetMarketsConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/values\n  method: get\n  operationId: GetMarketsValues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jit/liquidity_info\n  method: get\n  operationId: GetLiquidityInfo\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jit/liquidity_history\n  method: get\n  operationId: GetLiquidityHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gmx-account/deposit/cross-chain/prepare\n  method: post\n  operationId: PrepareCrossChainDeposit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gmx-account/withdraw/cross-chain/prepare\n  method: post\n  operationId: PrepareCrossChainWithdraw\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gmx-account/withdraw/cross-chain/submit\n  method: post\n  operationId: SubmitCrossChainWithdraw\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gmx-account/withdraw/cross-chain/status\n  method: post\n  operationId: StatusCrossChainWithdraw\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /buyback/weekly-stats\n  method: get\n  operationId: GetWeeklyStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /balances/wallet\n  method: get\n  operationId: GetWalletBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apy\n  method: get\n  operationId: GetApy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /allowances\n  method: get\n  operationId: GetAllowances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gmx/refs/heads/main/agentic-access/gmx-agentic-access.yml
summary_line: 37 operations · 13 acting
tags:
- DeFi
- Perpetual Exchange
- DEX
- Trading
- Leverage
- Liquidity Pools
- GLP
- GM Tokens
- GLV
- Arbitrum
- Avalanche
- Web3
---
