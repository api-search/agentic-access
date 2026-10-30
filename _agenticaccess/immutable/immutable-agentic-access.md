---
acting_count: 19
action_class_counts:
  acting: 19
  connected: 44
api_specs:
- filename: immutable-activities-api-openapi.yml
  format: yaml
  label: Immutable Activities API
  slug: immutable-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immutable/refs/heads/main/openapi/immutable-activities-api-openapi.yml
- filename: immutable-chains-api-openapi.yml
  format: yaml
  label: Immutable Chains API
  slug: immutable-chains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immutable/refs/heads/main/openapi/immutable-chains-api-openapi.yml
- filename: immutable-collections-api-openapi.yml
  format: yaml
  label: Immutable Collections API
  slug: immutable-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immutable/refs/heads/main/openapi/immutable-collections-api-openapi.yml
- filename: immutable-crafting-api-openapi.yml
  format: yaml
  label: Immutable Crafting API
  slug: immutable-crafting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immutable/refs/heads/main/openapi/immutable-crafting-api-openapi.yml
- filename: immutable-data-api-openapi.yml
  format: yaml
  label: Immutable Data API
  slug: immutable-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immutable/refs/heads/main/openapi/immutable-data-api-openapi.yml
- filename: immutable-ingest-api-openapi.yml
  format: yaml
  label: Immutable Ingest API
  slug: immutable-ingest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immutable/refs/heads/main/openapi/immutable-ingest-api-openapi.yml
- filename: immutable-metadata-api-openapi.yml
  format: yaml
  label: Immutable Metadata API
  slug: immutable-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immutable/refs/heads/main/openapi/immutable-metadata-api-openapi.yml
- filename: immutable-metadata-search-api-openapi.yml
  format: yaml
  label: Immutable Metadata Search API
  slug: immutable-metadata-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immutable/refs/heads/main/openapi/immutable-metadata-search-api-openapi.yml
- filename: immutable-nft-owners-api-openapi.yml
  format: yaml
  label: Immutable nft owners API
  slug: immutable-nft-owners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immutable/refs/heads/main/openapi/immutable-nft-owners-api-openapi.yml
- filename: immutable-orders-api-openapi.yml
  format: yaml
  label: Immutable Orders API
  slug: immutable-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immutable/refs/heads/main/openapi/immutable-orders-api-openapi.yml
- filename: immutable-passport-api-openapi.yml
  format: yaml
  label: Immutable Passport API
  slug: immutable-passport-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immutable/refs/heads/main/openapi/immutable-passport-api-openapi.yml
- filename: immutable-passport-profile-api-openapi.yml
  format: yaml
  label: Immutable passport profile API
  slug: immutable-passport-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immutable/refs/heads/main/openapi/immutable-passport-profile-api-openapi.yml
- filename: immutable-pricing-api-openapi.yml
  format: yaml
  label: Immutable Pricing API
  slug: immutable-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immutable/refs/heads/main/openapi/immutable-pricing-api-openapi.yml
- filename: immutable-tokens-api-openapi.yml
  format: yaml
  label: Immutable Tokens API
  slug: immutable-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immutable/refs/heads/main/openapi/immutable-tokens-api-openapi.yml
- filename: immutable-tracking-consent-api-openapi.yml
  format: yaml
  label: Immutable Tracking Consent API
  slug: immutable-tracking-consent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immutable/refs/heads/main/openapi/immutable-tracking-consent-api-openapi.yml
- filename: immutable-nfts-api-openapi.yml
  format: yaml
  label: Immutable Nfts API
  slug: immutable-nfts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immutable/refs/heads/main/openapi/immutable-nfts-api-openapi.yml
consequence_counts:
  physical: 7
  read: 44
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Immutable Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /passport-profile/v1/phone-otp
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/chains/{chain_name}/orders/bids
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/chains/{chain_name}/orders/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/chains/{chain_name}/orders/collection-bids
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/chains/{chain_name}/orders/listings
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/chains/{chain_name}/orders/metadata-bids
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/chains/{chain_name}/orders/trait-bids
operation_count: 63
overview: 'Immutable exposes 63 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 44 read, 12 write, and 7 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Immutable
provider_slug: immutable
slug: immutable-agentic-access
source_filename: immutable-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: generated\nsource: openapi/immutable-activities-api-openapi.yml, openapi/immutable-chains-api-openapi.yml,\n  openapi/immutable-collections-api-openapi.yml, openapi/immutable-crafting-api-openapi.yml,\n  openapi/immutable-data-api-openapi.yml, openapi/immutable-ingest-api-openapi.yml, openapi/immutable-metadata-api-openapi.yml,\n  openapi/immutable-metadata-search-api-openapi.yml, openapi/immutable-nft-owners-api-openapi.yml,\n  openapi/immutable-nfts-api-openapi.yml, openapi/immutable-orders-api-openapi.yml, openapi/immutable-passport-api-openapi.yml,\n  openapi/immutable-passport-profile-api-openapi.yml, openapi/immutable-pricing-api-openapi.yml,\n  openapi/immutable-tokens-api-openapi.yml, openapi/immutable-tracking-consent-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience\
  \ per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 63\n  by_action_class:\n    connected: 44\n    acting: 19\n  by_consequence:\n    read: 44\n    write: 12\n    physical: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/chains/{chain_name}/activity-history\n  method: get\n  operationId: ListActivityHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chains/{chain_name}/activities\n  method: get\n  operationId: ListActivities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chains/{chain_name}/activities/{activity_id}\n  method: get\n  operationId: GetActivity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chains\n\
  \  method: get\n  operationId: ListChains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chains/{chain_name}/collections\n  method: get\n  operationId: ListCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chains/{chain_name}/collections/{contract_address}\n  method: get\n  operationId: GetCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chains/{chain_name}/collections/{contract_address}/refresh-metadata\n  method: post\n  operationId: RefreshCollectionMetadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - refresh:metadata\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chains/{chain_name}/accounts/{account_address}/collections\n  method: get\n  operationId: ListCollectionsByNFTOwner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/internal/chains/{chain_name}/environment/{environment}/collections/{contract_address}/refresh-metadata\n  method: post\n  operationId: RefreshCollectionMetadataInternal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chains/{chain_name}/crafting/sign\n  method: post\n  operationId: SignCraftingPayload\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    scope:\n    - create:collections\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/audience/data\n  method: delete\n  operationId: DeleteAudienceData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/audience/messages\n  method: post\n  operationId: IngestMessages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chains/{chain_name}/collections/{contract_address}/metadata/{metadata_id}\n\
  \  method: get\n  operationId: GetMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chains/{chain_name}/collections/{contract_address}/metadata\n  method: get\n  operationId: ListMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chains/{chain_name}/metadata\n  method: get\n  operationId: ListMetadataForChain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chains/{chain_name}/collections/{contract_address}/metadata/refresh-metadata\n  method: post\n  operationId: RefreshMetadataByID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - refresh:metadata\n    audience: null\n    token:\n  \
  \    max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chains/{chain_name}/collections/{contract_address}/nfts/refresh-metadata\n  method: post\n  operationId: RefreshNFTMetadataByTokenID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - refresh:metadata\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chains/{chain_name}/stacks\n  method: get\n  operationId: ListStacks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chains/{chain_name}/search/filters/{contract_address}\n  method: get\n  operationId: ListFilters\n  x-agentic-access:\n    action-class: connected\n  \
  \  consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chains/{chain_name}/search/nfts\n  method: get\n  operationId: SearchNFTs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chains/{chain_name}/search/stacks\n  method: get\n  operationId: SearchStacks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chains/{chain_name}/collections/{contract_address}/nfts/{token_id}/owners\n  method: get\n  operationId: ListNFTOwners\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chains/{chain_name}/nft-owners\n  method: get\n  operationId: ListAllNFTOwners\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chains/{chain_name}/collections/{contract_address}/owners\n  method: get\n  operationId: ListOwnersByContractAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chains/{chain_name}/collections/{contract_address}/nfts/{token_id}\n  method: get\n  operationId: GetNFT\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chains/{chain_name}/collections/{contract_address}/nfts\n  method: get\n  operationId: ListNFTs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chains/{chain_name}/accounts/{account_address}/nfts\n  method: get\n  operationId: ListNFTsByAccountAddress\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chains/{chain_name}/nfts\n  method: get\n  operationId: ListAllNFTs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chains/{chain_name}/collections/{contract_address}/nfts/mint-requests\n  method: post\n  operationId: CreateMintRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:mint-request\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chains/{chain_name}/collections/{contract_address}/nfts/mint-requests\n  method: get\n  operationId: ListMintRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    scope:\n    - write:mint-request\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chains/{chain_name}/collections/{contract_address}/nfts/mint-requests/{reference_id}\n  method: get\n  operationId: GetMintRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - write:mint-request\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chains/{chain_name}/orders/cancel\n  method: post\n  operationId: CancelOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chains/{chain_name}/orders/listings\n  method: get\n  operationId: ListListings\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chains/{chain_name}/orders/listings\n  method: post\n  operationId: CreateListing\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chains/{chain_name}/orders/bids\n  method: get\n  operationId: ListBids\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chains/{chain_name}/orders/bids\n  method: post\n  operationId: CreateBid\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chains/{chain_name}/orders/collection-bids\n  method: get\n  operationId: ListCollectionBids\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chains/{chain_name}/orders/collection-bids\n  method: post\n  operationId: CreateCollectionBid\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chains/{chain_name}/orders/trait-bids\n  method: get\n  operationId: ListTraitBids\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chains/{chain_name}/orders/trait-bids\n  method: post\n  operationId: CreateTraitBid\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chains/{chain_name}/orders/metadata-bids\n  method: get\n  operationId: ListMetadataBids\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chains/{chain_name}/orders/metadata-bids\n  method: post\n  operationId: CreateMetadataBid\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chains/{chain_name}/orders/trait-bids/{trait_bid_id}\n  method: get\n  operationId: GetTraitBid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chains/{chain_name}/orders/metadata-bids/{metadata_bid_id}\n  method: get\n  operationId: GetMetadataBid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chains/{chain_name}/orders/listings/{listing_id}\n  method: get\n  operationId: GetListing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chains/{chain_name}/orders/bids/{bid_id}\n\
  \  method: get\n  operationId: GetBid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chains/{chain_name}/orders/collection-bids/{collection_bid_id}\n  method: get\n  operationId: GetCollectionBid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chains/{chain_name}/orders/fulfillment-data\n  method: post\n  operationId: fulfillment_data\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chains/{chain_name}/trades\n  method: get\n  operationId: ListTrades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chains/{chain_name}/trades/{trade_id}\n  method: get\n\
  \  operationId: GetTrade\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chains/{chain_name}/passport/users/{user_id}/linked-addresses\n  method: get\n  operationId: getLinkedAddresses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - openid\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /passport-profile/v1/phone-otp/verify\n  method: post\n  operationId: verify-phone-otp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - openid\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /passport-profile/v1/profile\n  method: get\n  operationId: get-profile-by-authenticated-wallet\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    scope:\n    - openid\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /passport-profile/v1/username\n  method: post\n  operationId: update-username\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - openid\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /passport-profile/v1/phone-otp\n  method: post\n  operationId: send-phone-otp\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - openid\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /passport-profile/v2/linked-wallets\n\
  \  method: post\n  operationId: link-wallet-v2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - openid\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /passport-profile/v1/user/info\n  method: get\n  operationId: getUserInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - openid\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chains/{chain_name}/quotes/{contract_address}/stacks\n  method: get\n  operationId: QuotesForStacks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chains/{chain_name}/quotes/{contract_address}/nfts\n  method: get\n  operationId: QuotesForNFTs\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chains/{chain_name}/tokens\n  method: get\n  operationId: ListERC20Tokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chains/{chain_name}/tokens/{contract_address}\n  method: get\n  operationId: GetERC20Token\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/audience/tracking-consent\n  method: get\n  operationId: GetTrackingConsent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/audience/tracking-consent\n  method: put\n  operationId: UpdateTrackingConsent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/immutable/refs/heads/main/agentic-access/immutable-agentic-access.yml
summary_line: 63 operations · 19 acting
tags:
- Company
- Gaming
- Blockchain
- NFT
- Web3
- Wallets
- Marketplace
- Analytics
- Attribution
- Customer Data Platform
- Authentication
- Developer Platform
- A2A
---
