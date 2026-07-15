---
acting_count: 22
action_class_counts:
  acting: 22
  connected: 61
api_specs:
- filename: opensea-api.json
  format: json
  label: OpenSea NFT API
  slug: nft-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/ProjectOpenSea/api-types/main/opensea-api.json
- filename: opensea-api.json
  format: json
  label: OpenSea Collection API
  slug: collection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/ProjectOpenSea/api-types/main/opensea-api.json
- filename: opensea-api.json
  format: json
  label: OpenSea Listing API
  slug: listing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/ProjectOpenSea/api-types/main/opensea-api.json
- filename: opensea-api.json
  format: json
  label: OpenSea Offer API
  slug: offer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/ProjectOpenSea/api-types/main/opensea-api.json
- filename: opensea-api.json
  format: json
  label: OpenSea Order API
  slug: order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/ProjectOpenSea/api-types/main/opensea-api.json
- filename: opensea-api.json
  format: json
  label: OpenSea Events API
  slug: events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/ProjectOpenSea/api-types/main/opensea-api.json
- filename: opensea-api.json
  format: json
  label: OpenSea Token API
  slug: token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/ProjectOpenSea/api-types/main/opensea-api.json
- filename: opensea-api.json
  format: json
  label: OpenSea Account API
  slug: account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/ProjectOpenSea/api-types/main/opensea-api.json
- filename: opensea-api.json
  format: json
  label: OpenSea Drops API
  slug: drops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/ProjectOpenSea/api-types/main/opensea-api.json
- filename: opensea-api.json
  format: json
  label: OpenSea Search API
  slug: search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/ProjectOpenSea/api-types/main/opensea-api.json
- filename: opensea-api.json
  format: json
  label: OpenSea Swap API
  slug: swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/ProjectOpenSea/api-types/main/opensea-api.json
consequence_counts:
  physical: 8
  read: 61
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Opensea Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/assets/transfer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/drops/deploy
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/listings/cross_chain_fulfillment_data
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/listings/fulfillment_data
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/offers/fulfillment_data
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/orders/chain/{chain}/protocol/{protocol_address}/{order_hash}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/orders/{chain}/{protocol}/listings
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/orders/{chain}/{protocol}/offers
operation_count: 83
overview: 'OpenSea exposes 83 API operations that an AI agent could call, of which 22 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 61 read, 14 write, and 8 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: OpenSea
provider_slug: opensea
slug: opensea-agentic-access
source_filename: opensea-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/opensea-api.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 83\n  by_action_class:\n    acting: 22\n    connected: 61\n  by_consequence:\n    write: 14\n    physical: 8\n    read: 61\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v2/transactions/receipt\n  method: post\n  operationId: get_transaction_receipt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/tools/usage\n  method: post\n  operationId: report_tool_usage\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/tokens/batch\n  method: post\n  operationId: get_tokens_batch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/swap/execute\n  method: post\n  operationId: post_swap_execute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/orders/{chain}/{protocol}/offers\n\
  \  method: post\n  operationId: post_offer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/orders/{chain}/{protocol}/listings\n  method: post\n  operationId: post_listing\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/orders/chain/{chain}/protocol/{protocol_address}/{order_hash}/cancel\n  method: post\n  operationId: cancel_order\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/offers\n  method: post\n  operationId: post_criteria_offer_v2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/offers/fulfillment_data\n  method: post\n  operationId: generate_offer_fulfillment_data_v2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/offers/build\n  method: post\n  operationId: build_offer_v2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/nfts/batch\n  method: post\n  operationId: get_nfts_batch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/listings/sweep\n  method: post\n  operationId: sweep_collection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/listings/fulfillment_data\n  method: post\n  operationId: generate_listing_fulfillment_data_v2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/listings/cross_chain_fulfillment_data\n  method: post\n  operationId: generate_cross_chain_listing_fulfillment_data\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/v2/listings/actions\n  method: post\n  operationId: create_listing_actions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/drops/{slug}/mint\n  method: post\n  operationId: build_drop_mint_transaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/drops/deploy\n  method: post\n  operationId: deploy_drop_contract\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/collections/batch\n  method: post\n  operationId: get_collections_batch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/chain/{chain}/contract/{address}/nfts/{identifier}/validate-metadata\n  method: post\n  operationId: validate_nft_metadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/chain/{chain}/contract/{address}/nfts/{identifier}/refresh\n\
  \  method: post\n  operationId: refresh_nft_metadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/auth/keys\n  method: post\n  operationId: create_instant_api_key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/assets/transfer\n  method: post\n  operationId: transfer_assets\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/traits/{slug}\n  method: get\n  operationId: get_collection_traits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/tools\n  method: get\n  operationId: list_tools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/tools/{registry_chain}/{registry_addr}/{tool_id}\n  method: get\n  operationId: get_tool\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/tools/search\n  method: get\n  operationId: search_tools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/v2/tokens/trending\n  method: get\n  operationId: get_trending_tokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/tokens/top\n  method: get\n  operationId: get_top_tokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/token-groups\n  method: get\n  operationId: get_token_groups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/token-groups/{slug}\n  method: get\n  operationId: get_token_group\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/swap/quote\n  method: get\n  operationId: get_swap_quote\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/search\n  method: get\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/orders/chain/{chain}/protocol/{protocol_address}/{order_hash}\n  method: get\n  operationId: get_order\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/offers/collection/{slug}\n  method: get\n  operationId: get_offers_collection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/offers/collection/{slug}/traits\n  method: get\n  operationId: get_offers_collection_trait\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/offers/collection/{slug}/nfts/{identifier}\n  method: get\n  operationId: get_offers_nft\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/offers/collection/{slug}/nfts/{identifier}/best\n  method: get\n  operationId: get_best_offer_nft\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/offers/collection/{slug}/all\n  method: get\n  operationId: list_offers_collection_all\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/metadata/{chain}/{contractAddress}/{tokenId}\n  method: get\n  operationId: get_nft_metadata\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/listings/collection/{slug}/nfts/{identifier}/best\n  method: get\n  operationId: get_best_listing_nft\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/listings/collection/{slug}/best\n  method: get\n  operationId: get_best_listings_collection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/listings/collection/{slug}/all\n  method: get\n  operationId: list_listings_collection_all\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/events\n  method: get\n  operationId: list_events\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/events/collection/{slug}\n  method: get\n  operationId: list_events_by_collection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/events/chain/{chain}/contract/{address}/nfts/{identifier}\n  method: get\n  operationId: list_events_by_nft\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/events/accounts/{address}\n  method: get\n  operationId: list_events_by_account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/drops\n  method: get\n  operationId: get_drops\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/drops/{slug}\n  method: get\n  operationId: get_drop_by_slug\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/drops/deploy/{chain}/{tx_hash}/receipt\n  method: get\n  operationId: get_deploy_contract_receipt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/collections\n  method: get\n  operationId: list_collections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/collections/{slug}\n  method: get\n  operationId: get_collection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /api/v2/collections/{slug}/stats\n  method: get\n  operationId: get_collection_stats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/collections/{slug}/offer_aggregates\n  method: get\n  operationId: get_collection_offer_aggregates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/collections/{slug}/holders\n  method: get\n  operationId: get_collection_holders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/collections/{slug}/floor_prices\n  method: get\n  operationId: get_collection_floor_prices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/v2/collections/trending\n  method: get\n  operationId: get_trending_collections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/collections/top\n  method: get\n  operationId: get_top_collections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/collection/{slug}/nfts\n  method: get\n  operationId: get_nfts_by_collection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/chains\n  method: get\n  operationId: get_chains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/chain/{chain}/token/{address}\n  method: get\n  operationId: get_token\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/chain/{chain}/token/{address}/price_history\n  method: get\n  operationId: get_token_price_history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/chain/{chain}/token/{address}/ohlcv\n  method: get\n  operationId: get_token_ohlcv\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/chain/{chain}/token/{address}/liquidity-pools\n  method: get\n  operationId: get_token_liquidity_pools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/chain/{chain}/token/{address}/holders\n  method: get\n  operationId:\
  \ get_token_holders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/chain/{chain}/token/{address}/activity\n  method: get\n  operationId: get_token_activity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/chain/{chain}/payment_token/{address}\n  method: get\n  operationId: get_payment_token\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/chain/{chain}/contract/{address}\n  method: get\n  operationId: get_contract\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/chain/{chain}/contract/{address}/nfts\n  method: get\n  operationId: get_nfts_by_contract\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/chain/{chain}/contract/{address}/nfts/{identifier}\n  method: get\n  operationId: get_nft\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/chain/{chain}/contract/{address}/nfts/{identifier}/owners\n  method: get\n  operationId: get_nft_owners\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/chain/{chain}/contract/{address}/nfts/{identifier}/collection\n  method: get\n  operationId: get_nft_collection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/chain/{chain}/contract/{address}/nfts/{identifier}/analytics\n\
  \  method: get\n  operationId: get_nft_analytics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/chain/{chain}/account/{address}/nfts\n  method: get\n  operationId: get_nfts_by_account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/accounts/{address_or_username}\n  method: get\n  operationId: get_account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/accounts/resolve/{identifier}\n  method: get\n  operationId: resolve_account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/account/{address}/tokens\n  method: get\n  operationId: get_token_balances_by_account\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/account/{address}/portfolio\n  method: get\n  operationId: get_portfolio_stats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/account/{address}/portfolio/history\n  method: get\n  operationId: get_portfolio_history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/account/{address}/offers_received\n  method: get\n  operationId: get_profile_offers_received\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/account/{address}/offers\n  method: get\n  operationId: get_profile_offers\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/account/{address}/listings\n  method: get\n  operationId: get_profile_listings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/account/{address}/favorites\n  method: get\n  operationId: get_profile_favorites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/account/{address}/collections\n  method: get\n  operationId: get_profile_collections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opensea/refs/heads/main/agentic-access/opensea-agentic-access.yml
summary_line: 83 operations · 22 acting
tags:
- NFT
- Marketplace
- Web3
- Blockchain
- Trading
- Digital Assets
---
