---
acting_count: 0
action_class_counts:
  connected: 36
api_specs:
- filename: blockvision-monad-api-openapi.yml
  format: yaml
  label: BlockVision Monad API
  slug: blockvision-monad-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockvision/refs/heads/main/openapi/blockvision-monad-api-openapi.yml
- filename: blockvision-sui-api-openapi.yml
  format: yaml
  label: BlockVision Sui API
  slug: blockvision-sui-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockvision/refs/heads/main/openapi/blockvision-sui-api-openapi.yml
consequence_counts:
  read: 36
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Blockvision Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 36
overview: 'BlockVision exposes 36 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 36 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BlockVision
provider_slug: blockvision
slug: blockvision-agentic-access
source_filename: blockvision-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: generated\nsource: openapi/blockvision-v2-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 36\n  by_action_class:\n    connected: 36\n  by_consequence:\n    read: 36\n  human_in_the_loop_required: 0\noperations:\n- path: /monad/account/activities\n  method: get\n  operationId: retrieve-monad-account-activity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monad/account/defiPortfolio\n  method: get\n  operationId: get_monadaccountdefiPortfolio\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /monad/account/internal/transactions\n  method: get\n  operationId: retrieve-account-internal-transactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monad/account/nfts\n  method: get\n  operationId: retrieve-monad-account-nfts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monad/account/tokens\n  method: get\n  operationId: retrieve-monad-account-tokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monad/account/transactions\n  method: get\n  operationId: retrieve-monad-account-transactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monad/collection/activities\n\
  \  method: get\n  operationId: retrieve-nft-activities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monad/collection/holders\n  method: get\n  operationId: retrieve-nft-holders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monad/contract/detail\n  method: get\n  operationId: get_monadcontractdetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monad/contract/source/code\n  method: get\n  operationId: retrieve-contract-source-code\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monad/native/holders\n  method: get\n  operationId: retrieve-monad-holders\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monad/token/activities\n  method: get\n  operationId: retrieve-token-activities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monad/token/detail\n  method: get\n  operationId: retrieve-token-detail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monad/token/gating\n  method: get\n  operationId: retrieve-token-gating-api\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monad/token/holders\n  method: get\n  operationId: retrieve-token-holders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /monad/token/market/data\n  method: get\n  operationId: get_monadtokenmarketdata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monad/token/ohlcv\n  method: get\n  operationId: get_monadtokenohlcv\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monad/token/pools\n  method: get\n  operationId: get_monadtokenpools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monad/token/price/list\n  method: get\n  operationId: get_monadtokenpricelist\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monad/token/trades\n\
  \  method: get\n  operationId: get_monadtokentrades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monad/verified/contracts\n  method: get\n  operationId: get_monadverifiedcontracts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sui/account/activities\n  method: get\n  operationId: retrieve-account-activity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sui/account/coins\n  method: get\n  operationId: retrieve-account-coins\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sui/account/defiPortfolio\n  method: get\n  operationId: retrieve-account-defi-portfolio\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sui/account/nfts\n  method: get\n  operationId: retrieve-account-nfts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sui/coin/detail\n  method: get\n  operationId: retrieve-coin-detail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sui/coin/dex/pools\n  method: get\n  operationId: get_coindexpools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sui/coin/holders\n  method: get\n  operationId: retrieve-coin-holders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n   \
  \ token:\n      max-ttl: 3600\n    audit: none\n- path: /sui/coin/market/pro\n  method: get\n  operationId: get_suicoinmarketdata2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sui/coin/ohlcv\n  method: get\n  operationId: get_new-endpoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sui/coin/price/list\n  method: get\n  operationId: get_coinpricelist\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sui/coin/trades\n  method: get\n  operationId: get_cointrades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sui/nft/activities\n  method: get\n  operationId: sui-retrieve-nft-activity\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sui/nft/collection/holder\n  method: get\n  operationId: retrieve-collection-holders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sui/nft/collectionDetail\n  method: get\n  operationId: retrieve-collection-details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sui/nft/list\n  method: get\n  operationId: retrieve-collection-nft-list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blockvision/refs/heads/main/agentic-access/blockvision-agentic-access.yml
summary_line: 36 operations
tags:
- Company
- Blockchain
- Web3
- Data Infrastructure
- Sui
- Monad
- NFT
- DeFi
- RPC Node
- Indexing
- Cryptocurrency
- Smart Contracts
---
