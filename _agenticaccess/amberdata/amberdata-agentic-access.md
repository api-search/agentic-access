---
acting_count: 0
action_class_counts:
  connected: 24
api_specs:
- filename: amberdata-openapi.yml
  format: yaml
  label: Amberdata Spot Market Data API
  slug: spot-market-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amberdata/refs/heads/main/openapi/amberdata-openapi.yml
- filename: amberdata-openapi.yml
  format: yaml
  label: Amberdata Derivatives API
  slug: derivatives
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amberdata/refs/heads/main/openapi/amberdata-openapi.yml
- filename: amberdata-openapi.yml
  format: yaml
  label: Amberdata DeFi API
  slug: defi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amberdata/refs/heads/main/openapi/amberdata-openapi.yml
- filename: amberdata-openapi.yml
  format: yaml
  label: Amberdata On-Chain API
  slug: on-chain
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amberdata/refs/heads/main/openapi/amberdata-openapi.yml
- filename: amberdata-asyncapi.yml
  format: yaml
  label: Amberdata WebSocket Streaming API
  slug: websocket-streaming
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/amberdata/refs/heads/main/asyncapi/amberdata-asyncapi.yml
consequence_counts:
  read: 24
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Amberdata Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 24
overview: 'Amberdata exposes 24 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 24 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amberdata
provider_slug: amberdata
slug: amberdata-agentic-access
source_filename: amberdata-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/amberdata-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 24\n  by_action_class:\n    connected: 24\n  by_consequence:\n    read: 24\n  human_in_the_loop_required: 0\noperations:\n- path: /markets/spot/exchanges/reference\n  method: get\n  operationId: getSpotExchangesReference\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/spot/prices/{pair}/latest\n  method: get\n  operationId: getSpotPriceLatest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/spot/ohlcv/{pair}/historical\n\
  \  method: get\n  operationId: getSpotOhlcvHistorical\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/spot/tickers/{pair}\n  method: get\n  operationId: getSpotTickers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/spot/trades/{pair}\n  method: get\n  operationId: getSpotTrades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/spot/order-book-snapshots/{pair}\n  method: get\n  operationId: getSpotOrderBookSnapshots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/futures/exchanges/reference\n  method: get\n  operationId: getFuturesExchangesReference\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/futures/tickers/{instrument}\n  method: get\n  operationId: getFuturesTickers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/futures/funding-rates/{instrument}\n  method: get\n  operationId: getFuturesFundingRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/futures/open-interest/{instrument}\n  method: get\n  operationId: getFuturesOpenInterest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/futures/liquidations/{instrument}\n  method: get\n  operationId: getFuturesLiquidations\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/options/exchanges/reference\n  method: get\n  operationId: getOptionsExchangesReference\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/options/trades/{instrument}\n  method: get\n  operationId: getOptionsTrades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/options/order-book-snapshots/{instrument}\n  method: get\n  operationId: getOptionsOrderBookSnapshots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /defi/dex/trades/{pair}\n  method: get\n  operationId: getDefiDexTrades\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /defi/lending/protocols\n  method: get\n  operationId: getDefiLendingProtocols\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /blockchains/{blockchainId}/blocks\n  method: get\n  operationId: getBlocks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /blockchains/{blockchainId}/transactions\n  method: get\n  operationId: getTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /blockchains/{blockchainId}/transactions/{hash}\n  method: get\n  operationId: getTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /blockchains/{blockchainId}/addresses/{address}/balances\n  method: get\n  operationId: getAddressBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /blockchains/{blockchainId}/addresses/{address}/transactions\n  method: get\n  operationId: getAddressTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /blockchains/{blockchainId}/tokens/{address}/information\n  method: get\n  operationId: getTokenInformation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /blockchains/{blockchainId}/tokens/{address}/transfers\n  method: get\n  operationId: getTokenTransfers\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /blockchains/{blockchainId}/tokens/{address}/holders\n  method: get\n  operationId: getTokenHolders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amberdata/refs/heads/main/agentic-access/amberdata-agentic-access.yml
summary_line: 24 operations
tags:
- Crypto
- Blockchain
- Market Data
- Digital Assets
- Derivatives
- DeFi
- On-Chain
---
