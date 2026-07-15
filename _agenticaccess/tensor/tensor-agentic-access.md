---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 45
api_specs:
- filename: tensor-api-openapi.yml
  format: yaml
  label: Tensor API
  slug: tensor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensor/refs/heads/main/openapi/tensor-api-openapi.yml
- filename: tensor-tx-api-openapi.yml
  format: yaml
  label: Tensor Transaction API
  slug: tensor-tx-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensor/refs/heads/main/openapi/tensor-tx-api-openapi.yml
- filename: tensor-websocket-api-asyncapi.yml
  format: yaml
  label: Tensor WebSocket API
  slug: tensor-websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensor/refs/heads/main/asyncapi/tensor-websocket-api-asyncapi.yml
consequence_counts:
  read: 45
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tensor Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 47
overview: 'Tensor exposes 47 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 45 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Tensor
provider_slug: tensor
slug: tensor-agentic-access
source_filename: tensor-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/tensor-api-openapi.yml, openapi/tensor-tx-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 47\n  by_action_class:\n    connected: 45\n    acting: 2\n  by_consequence:\n    read: 45\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/collections/find\n  method: get\n  operationId: findCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/collections/verified\n  method: get\n  operationId: listVerifiedCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/v1/collections/{slug}/traits\n  method: get\n  operationId: getCollectionTraits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/collections/search\n  method: get\n  operationId: searchCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/collections/by-nfts\n  method: get\n  operationId: getCollectionsByNfts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/mints/info\n  method: get\n  operationId: getMintsInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/collections/{slug}/mints\n  method:\
  \ get\n  operationId: getNftsByCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/collections/{slug}/mint-list\n  method: get\n  operationId: getMintList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/listings\n  method: get\n  operationId: listActiveListings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/collections/{slug}/activity\n  method: get\n  operationId: getCollectionActivity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/bids/collection\n  method: get\n  operationId: getCollectionBids\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/bids/single-nft\n  method: get\n  operationId: getSingleNftBids\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/bids/trait\n  method: get\n  operationId: getTraitBids\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/pools/tswap\n  method: get\n  operationId: getTswapPools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/pools/tamm\n  method: get\n  operationId: getTammPools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/v1/user/listings\n  method: get\n  operationId: getUserListings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/user/bids/collection\n  method: get\n  operationId: getUserCollectionBids\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/user/bids/nft\n  method: get\n  operationId: getUserNftBids\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/user/bids/trait\n  method: get\n  operationId: getUserTraitBids\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/user/escrow\n  method: get\n  operationId: getUserEscrowAccounts\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/user/inventory/{slug}\n  method: get\n  operationId: getUserInventoryForCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/user/portfolio\n  method: get\n  operationId: getUserPortfolio\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/user/pools/tswap\n  method: get\n  operationId: getUserTswapPools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/user/pools/tamm\n  method: get\n  operationId: getUserTammPools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/user/transactions\n  method: get\n  operationId: getUserTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/mints/refresh-metadata\n  method: post\n  operationId: refreshMintMetadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/mints/refresh-rarities\n  method: post\n  operationId: refreshMintRarities\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/v1/mint-proof\n  method: get\n  operationId: getMintProof\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/bids/trait-attributes\n  method: get\n  operationId: getTraitBidAttributes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/whitelist/{address}\n  method: get\n  operationId: getWhitelistInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/priority-fees\n  method: get\n  operationId: getPriorityFees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tx/list\n  method: get\n  operationId: buildListTx\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tx/edit-listing\n  method: get\n  operationId: buildEditListingTx\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tx/delist\n  method: get\n  operationId: buildDelistTx\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tx/buy\n  method: get\n  operationId: buildBuyTx\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tx/place-collection-bid\n  method: get\n  operationId: buildPlaceCollectionBidTx\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tx/place-single-nft-bid\n  method: get\n  operationId: buildPlaceSingleNftBidTx\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tx/place-trait-bid\n  method: get\n  operationId: buildPlaceTraitBidTx\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tx/accept-bid\n  method: get\n  operationId: buildAcceptBidTx\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tx/cancel-bid\n  method: get\n  operationId: buildCancelBidTx\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tx/pool/create\n\
  \  method: get\n  operationId: buildCreatePoolTx\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tx/pool/edit\n  method: get\n  operationId: buildEditPoolTx\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tx/pool/close\n  method: get\n  operationId: buildClosePoolTx\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tx/pool/deposit\n  method: get\n  operationId: buildPoolDepositTx\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tx/pool/withdraw\n  method: get\n  operationId: buildPoolWithdrawTx\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tx/escrow/deposit\n  method: get\n  operationId: buildEscrowDepositTx\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tx/escrow/withdraw\n  method: get\n  operationId: buildEscrowWithdrawTx\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tensor/refs/heads/main/agentic-access/tensor-agentic-access.yml
summary_line: 47 operations · 2 acting
tags:
- NFT
- Marketplace
- Solana
- Blockchain
- Web3
- Cryptocurrency
- Trading
- DAO
- DeFi
- AMM
---
