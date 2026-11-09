---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 75
api_specs:
- filename: dripmetrics-ai-aerodrome-api-openapi.yml
  format: yaml
  label: DripMetrics AI Aerodrome API
  slug: dripmetrics-ai-aerodrome-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dripmetrics-ai/openapi/dripmetrics-ai-aerodrome-api-openapi.yml
- filename: dripmetrics-ai-btc-options-api-openapi.yml
  format: yaml
  label: DripMetrics AI BTC options API
  slug: dripmetrics-ai-btc-options-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dripmetrics-ai/openapi/dripmetrics-ai-btc-options-api-openapi.yml
- filename: dripmetrics-ai-discovery-api-openapi.yml
  format: yaml
  label: DripMetrics AI Discovery API
  slug: dripmetrics-ai-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dripmetrics-ai/openapi/dripmetrics-ai-discovery-api-openapi.yml
- filename: dripmetrics-ai-exchange-metrics-api-openapi.yml
  format: yaml
  label: DripMetrics AI Exchange metrics API
  slug: dripmetrics-ai-exchange-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dripmetrics-ai/openapi/dripmetrics-ai-exchange-metrics-api-openapi.yml
- filename: dripmetrics-ai-hyperliquid-api-openapi.yml
  format: yaml
  label: DripMetrics AI Hyperliquid API
  slug: dripmetrics-ai-hyperliquid-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dripmetrics-ai/openapi/dripmetrics-ai-hyperliquid-api-openapi.yml
- filename: dripmetrics-ai-hyperliquid-book-api-openapi.yml
  format: yaml
  label: DripMetrics AI Hyperliquid book API
  slug: dripmetrics-ai-hyperliquid-book-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dripmetrics-ai/openapi/dripmetrics-ai-hyperliquid-book-api-openapi.yml
- filename: dripmetrics-ai-kraken-xstocks-api-openapi.yml
  format: yaml
  label: DripMetrics AI Kraken xStocks API
  slug: dripmetrics-ai-kraken-xstocks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dripmetrics-ai/openapi/dripmetrics-ai-kraken-xstocks-api-openapi.yml
- filename: dripmetrics-ai-market-summary-api-openapi.yml
  format: yaml
  label: DripMetrics AI Market summary API
  slug: dripmetrics-ai-market-summary-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dripmetrics-ai/openapi/dripmetrics-ai-market-summary-api-openapi.yml
- filename: dripmetrics-ai-on-chain-api-openapi.yml
  format: yaml
  label: DripMetrics AI On Chain API
  slug: dripmetrics-ai-on-chain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dripmetrics-ai/openapi/dripmetrics-ai-on-chain-api-openapi.yml
- filename: dripmetrics-ai-orderbook-api-openapi.yml
  format: yaml
  label: DripMetrics AI Orderbook API
  slug: dripmetrics-ai-orderbook-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dripmetrics-ai/openapi/dripmetrics-ai-orderbook-api-openapi.yml
- filename: dripmetrics-ai-polymarket-api-openapi.yml
  format: yaml
  label: DripMetrics AI Polymarket API
  slug: dripmetrics-ai-polymarket-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dripmetrics-ai/openapi/dripmetrics-ai-polymarket-api-openapi.yml
- filename: dripmetrics-ai-portfolio-risk-api-openapi.yml
  format: yaml
  label: DripMetrics AI Portfolio risk API
  slug: dripmetrics-ai-portfolio-risk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dripmetrics-ai/openapi/dripmetrics-ai-portfolio-risk-api-openapi.yml
consequence_counts:
  read: 75
  safety-critical: 1
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Dripmetrics Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /options/spread-greeks
operation_count: 77
overview: 'DripMetrics AI exposes 77 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 75 read, 1 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: DripMetrics AI
provider_slug: dripmetrics-ai
slug: dripmetrics-ai-agentic-access
source_filename: dripmetrics-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: generated\nsource: openapi/dripmetrics-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 77\n  by_action_class:\n    connected: 75\n    acting: 2\n  by_consequence:\n    read: 75\n    safety-critical: 1\n    write: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /\n  method: get\n  operationId: getRoot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog\n  method: get\n  operationId:\
  \ getCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi.json\n  method: get\n  operationId: getOpenApiJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/vpin\n  method: get\n  operationId: getMetricVpin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/kyle-lambda\n  method: get\n  operationId: getMetricKyleLambda\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/beta\n  method: get\n  operationId: getMetricBeta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /metrics/order-flow-hhi\n  method: get\n  operationId: getMetricOrderFlowHhi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/historical-volatility\n  method: get\n  operationId: getMetricHistoricalVolatility\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/cvd\n  method: get\n  operationId: getMetricCvd\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/buy-sell-volume-imbalance\n  method: get\n  operationId: getMetricBuySellVolumeImbalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/signed-dollar-volume\n\
  \  method: get\n  operationId: getMetricSignedDollarVolume\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/trade-intensity\n  method: get\n  operationId: getMetricTradeIntensity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/average-trade-size\n  method: get\n  operationId: getMetricAverageTradeSize\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/large-trade-share\n  method: get\n  operationId: getMetricLargeTradeShare\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/realized-vol\n  method: get\n  operationId: getMetricRealizedVol\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/amihud-illiquidity\n  method: get\n  operationId: getMetricAmihudIlliquidity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/vwap\n  method: get\n  operationId: getMetricVwap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/vwap-deviation\n  method: get\n  operationId: getMetricVwapDeviation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/momentum\n  method: get\n  operationId: getMetricMomentum\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/reversal\n  method: get\n  operationId: getMetricReversal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/drawdown\n  method: get\n  operationId: getMetricDrawdown\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/downside-semivolatility\n  method: get\n  operationId: getMetricDownsideSemivolatility\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/rolling-correlation\n  method: get\n  operationId: getMetricRollingCorrelation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/vol-of-vol\n\
  \  method: get\n  operationId: getMetricVolOfVol\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/roll-spread\n  method: get\n  operationId: getMetricRollSpread\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hyperliquid/historical-volatility\n  method: get\n  operationId: getHyperliquidHistoricalVolatility\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hyperliquid/realized-vol\n  method: get\n  operationId: getHyperliquidRealizedVol\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hyperliquid/momentum\n  method: get\n  operationId: getHyperliquidMomentum\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hyperliquid/reversal\n  method: get\n  operationId: getHyperliquidReversal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hyperliquid/drawdown\n  method: get\n  operationId: getHyperliquidDrawdown\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hyperliquid/downside-semivolatility\n  method: get\n  operationId: getHyperliquidDownsideSemivolatility\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hyperliquid/vol-of-vol\n  method: get\n  operationId: getHyperliquidVolOfVol\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hyperliquid/beta\n  method: get\n  operationId: getHyperliquidBeta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hyperliquid/participant-concentration\n  method: get\n  operationId: getHyperliquidParticipantConcentration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hyperliquid-book/coverage\n  method: get\n  operationId: getHyperliquidBookCoverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hyperliquid-book/bbo\n  method: get\n  operationId: getHyperliquidBookBbo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /hyperliquid-book/depth\n  method: get\n  operationId: getHyperliquidBookDepth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hyperliquid-book/execution-impact\n  method: get\n  operationId: getHyperliquidBookExecutionImpact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /polymarket/vpin\n  method: get\n  operationId: getPolymarketVpin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /polymarket/kyle-lambda\n  method: get\n  operationId: getPolymarketKyleLambda\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /polymarket/flow-imbalance\n  method: get\n  operationId: getPolymarketFlowImbalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /polymarket/two-sidedness\n  method: get\n  operationId: getPolymarketTwoSidedness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /polymarket/wallet-concentration\n  method: get\n  operationId: getPolymarketWalletConcentration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /polymarket/wallet-novelty\n  method: get\n  operationId: getPolymarketWalletNovelty\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /polymarket/probability-shock\n\
  \  method: get\n  operationId: getPolymarketProbabilityShock\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /polymarket/leakage-score\n  method: get\n  operationId: getPolymarketLeakageScore\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/onchain/stablecoin-flow\n  method: get\n  operationId: getOnchainStablecoinFlow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/onchain/tvl-momentum\n  method: get\n  operationId: getOnchainTvlMomentum\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/onchain/protocol-fee-yield\n  method: get\n  operationId:\
  \ getOnchainProtocolFeeYield\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/onchain/dex-efficiency\n  method: get\n  operationId: getOnchainDexEfficiency\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /options/vrp\n  method: get\n  operationId: getOptionsVrp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /options/expected-move\n  method: get\n  operationId: getOptionsExpectedMove\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /options/crash-premium\n  method: get\n  operationId: getOptionsCrashPremium\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /options/gex\n  method: get\n  operationId: getOptionsGex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /options/spread-greeks\n  method: post\n  operationId: postOptionsSpreadGreeks\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /orderbook/spread\n  method: get\n  operationId: getOrderbookSpread\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orderbook/micro-price\n  method: get\n  operationId: getOrderbookMicroPrice\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orderbook/imbalance\n  method: get\n  operationId: getOrderbookImbalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orderbook/depth-at-distance\n  method: get\n  operationId: getOrderbookDepthAtDistance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orderbook/concentration\n  method: get\n  operationId: getOrderbookConcentration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orderbook/execution-impact\n  method: get\n  operationId: getOrderbookExecutionImpact\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orderbook/snapshot\n  method: get\n  operationId: getOrderbookSnapshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /kraken/spread\n  method: get\n  operationId: getKrakenSpread\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /kraken/micro-price\n  method: get\n  operationId: getKrakenMicroPrice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /kraken/imbalance\n  method: get\n  operationId: getKrakenImbalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /kraken/depth-at-distance\n\
  \  method: get\n  operationId: getKrakenDepthAtDistance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /kraken/concentration\n  method: get\n  operationId: getKrakenConcentration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /kraken/execution-impact\n  method: get\n  operationId: getKrakenExecutionImpact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /aerodrome/coverage\n  method: get\n  operationId: getAerodromeCoverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /aerodrome/trade-activity\n  method: get\n  operationId: getAerodromeTradeActivity\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /aerodrome/active-pairs\n  method: get\n  operationId: getAerodromeActivePairs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /aerodrome/flow-imbalance\n  method: get\n  operationId: getAerodromeFlowImbalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /aerodrome/order-flow-concentration\n  method: get\n  operationId: getAerodromeOrderFlowConcentration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /aerodrome/amm-flow-impact\n  method: get\n  operationId: getAerodromeAmmFlowImpact\n  x-agentic-access:\n    action-class: connected\n \
  \   consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/portfolio/var\n  method: post\n  operationId: postPortfolioVar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /market/summary\n  method: get\n  operationId: getMarketSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/dripmetrics-ai/agentic-access/dripmetrics-ai-agentic-access.yml
summary_line: 77 operations · 2 acting · 1 human-in-the-loop
tags:
- Company
- Market Data
- Analytics
- Artificial Intelligence
- Cryptocurrency
---
