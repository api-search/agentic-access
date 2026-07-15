---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 20
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Transpose Block API
  slug: transpose-block-api
  spec_type: OpenAPI
  url: https://docs.transpose.io/
- filename: openapi.yaml
  format: yaml
  label: Transpose Token API
  slug: transpose-token-api
  spec_type: OpenAPI
  url: https://docs.transpose.io/verified-endpoints/token-api/overview/
- filename: openapi.yaml
  format: yaml
  label: Transpose NFT API
  slug: transpose-nft-api
  spec_type: OpenAPI
  url: https://docs.transpose.io/
- filename: openapi.yaml
  format: yaml
  label: Transpose ENS API
  slug: transpose-ens-api
  spec_type: OpenAPI
  url: https://docs.transpose.io/
- filename: openapi.yaml
  format: yaml
  label: Transpose Token Prices API
  slug: transpose-token-prices-api
  spec_type: OpenAPI
  url: https://docs.transpose.io/verified-endpoints/token-prices-api/overview/
- filename: openapi.yaml
  format: yaml
  label: Transpose SQL Analytics API
  slug: transpose-sql-analytics-api
  spec_type: OpenAPI
  url: https://docs.transpose.io/
consequence_counts:
  read: 20
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Transpose Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 21
overview: 'Transpose exposes 21 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Transpose
provider_slug: transpose
slug: transpose-agentic-access
source_filename: transpose-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    connected: 20\n    acting: 1\n  by_consequence:\n    read: 20\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /block/accounts\n  method: get\n  operationId: getAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /block/blocks\n  method: get\n  operationId: getBlocks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /block/transactions\n  method: get\n  operationId:\
  \ getTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /block/logs\n  method: get\n  operationId: getLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /block/traces\n  method: get\n  operationId: getTraces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /token/tokens\n  method: get\n  operationId: getTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /token/transfers\n  method: get\n  operationId: getTokenTransfers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /token/swaps\n  method: get\n  operationId: getTokenSwaps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /token/native-token-transfers\n  method: get\n  operationId: getNativeTokenTransfers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /token/owners\n  method: get\n  operationId: getTokenOwners\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nft/collections\n  method: get\n  operationId: getNftCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nft/nfts\n  method: get\n  operationId: getNfts\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nft/transfers\n  method: get\n  operationId: getNftTransfers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nft/sales\n  method: get\n  operationId: getNftSales\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nft/owners\n  method: get\n  operationId: getNftOwners\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ens/records\n  method: get\n  operationId: getEnsRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ens/transfers\n  method: get\n  operationId:\
  \ getEnsTransfers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /prices/token-price\n  method: get\n  operationId: getTokenPrice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /prices/token-price-history\n  method: get\n  operationId: getTokenPriceHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /prices/ohlc-price-history\n  method: get\n  operationId: getOhlcPriceHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sql\n  method: post\n  operationId: executeSqlQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transpose/refs/heads/main/agentic-access/transpose-agentic-access.yml
summary_line: 21 operations · 1 acting
tags:
- Blockchain
- NFT
- Cryptocurrency
- Web3
- Ethereum
- Token Transfers
- Smart Contracts
- Historical Data
- DeFi
- DEX
---
