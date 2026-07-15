---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 30
api_specs:
- filename: open-api.json
  format: json
  label: Pendle V2 Core API
  slug: core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/pendle-finance/documentation/master/static/pendle-dev-docs/openapi/open-api.json
- filename: open-api.json
  format: json
  label: Pendle Hosted SDK
  slug: hosted-sdk
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/pendle-finance/documentation/master/static/pendle-dev-docs/openapi/open-api.json
consequence_counts:
  read: 30
  safety-critical: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 4
kind: agentic-access
layout: agentic-access
method: generated
name: Pendle Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/limit-orders/makers/generate-limit-order-data
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/limit-orders/makers/generate-scaled-order-data
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/limit-orders/makers/limit-orders
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v3/sdk/{chainId}/convert
operation_count: 34
overview: 'Pendle exposes 34 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 30 read and 4 safety-critical.


  4 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Pendle
provider_slug: pendle
slug: pendle-agentic-access
source_filename: pendle-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 34\n  by_action_class:\n    connected: 30\n    acting: 4\n  by_consequence:\n    read: 30\n    safety-critical: 4\n  human_in_the_loop_required: 4\noperations:\n- path: /v2/limit-orders\n  method: get\n  operationId: LimitOrdersController_getAllLimitOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/limit-orders/archived\n  method: get\n  operationId: LimitOrdersController_getAllArchivedLimitOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /v1/limit-orders/makers/limit-orders\n  method: get\n  operationId: LimitOrdersController_getMakerLimitOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/limit-orders/makers/limit-orders\n  method: post\n  operationId: LimitOrdersController_createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/limit-orders/makers/generate-limit-order-data\n  method: post\n  operationId: LimitOrdersController_generateLimitOrderData\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n \
  \     max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/limit-orders/makers/generate-scaled-order-data\n  method: post\n  operationId: LimitOrdersController_generateScaledLimitOrderData\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/limit-orders/takers/limit-orders\n  method: get\n  operationId: LimitOrdersController_getTakerLimitOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/limit-orders/book/{chainId}\n  method: get\n  operationId: LimitOrdersController_getLimitOrderBookV2\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/prices/assets\n  method: get\n  operationId: PricesCrossChainController_getAllAssetPricesByAddressesCrossChains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/{chainId}/prices/{address}/ohlcv\n  method: get\n  operationId: PricesController_ohlcv_v4\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/assets/all\n  method: get\n  operationId: AssetsCrossChainController_getPendleAssetsMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/markets/all\n  method: get\n  operationId: MarketsCrossChainController_getAllMarkets\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/markets/points-market\n  method: get\n  operationId: MarketsCrossChainController_getPointsMarkets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/{chainId}/markets/{address}/data\n  method: get\n  operationId: MarketsController_marketData_v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/{chainId}/markets/{address}/historical-data\n  method: get\n  operationId: MarketsController_marketHistoricalData_v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/ve-pendle/data\n  method: get\n  operationId: VePendleController_vePendleExtendedData\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ve-pendle/market-fees-chart\n  method: get\n  operationId: VePendleController_allMarketTotalFees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sdk/{chainId}/markets/{market}/tokens\n  method: get\n  operationId: SdkController_getMarketTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sdk/{chainId}/supported-aggregators\n  method: get\n  operationId: SdkController_getSupportedAggregators\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sdk/{chainId}/markets/{market}/swapping-prices\n  method: get\n\
  \  operationId: SdkController_getMarketSpotSwappingPrice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sdk/{chainId}/limit-order/cancel-single\n  method: get\n  operationId: SdkController_cancelSingleLimitOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sdk/{chainId}/limit-order/cancel-all\n  method: get\n  operationId: SdkController_cancelAllLimitOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sdk/{chainId}/redeem-interests-and-rewards\n  method: get\n  operationId: SdkController_redeemInterestsAndRewards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v2/sdk/{chainId}/convert\n  method: get\n  operationId: SdkController_convert\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/sdk/{chainId}/convert\n  method: post\n  operationId: SdkController_convertV3\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/sdk/{chainId}/swap-pt-cross-chain\n  method: get\n  operationId: SdkController_swapPtCrossChainV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sdk/{chainId}/cross-chain-pt-metadata/{pt}\n  method: get\n  operationId: SdkController_getPtCrossChainMetadata\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/{chainId}/transactions/{address}\n  method: get\n  operationId: TransactionsController_transactionsV5\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/statistics/get-distinct-user-from-token\n  method: get\n  operationId: StatisticsController_getDistinctUserFromToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chains\n  method: get\n  operationId: ChainsController_getSupportedChainIds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/dashboard/positions/database/{user}\n  method: get\n  operationId: DashboardController_getUserPositions\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/dashboard/merkle-claimed-rewards/{user}\n  method: get\n  operationId: DashboardController_getMerkleClaimedRewards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/pnl/transactions\n  method: get\n  operationId: TransactionsController_getTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/pendle-emission\n  method: get\n  operationId: PendleEmissionController_pendleEmission\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pendle/refs/heads/main/agentic-access/pendle-agentic-access.yml
summary_line: 34 operations · 4 acting · 4 human-in-the-loop
tags:
- Web3
- DeFi
- Yield Tokenization
- Crypto
- Principal Tokens
- Yield Tokens
- AMM
- Liquidity Pools
---
