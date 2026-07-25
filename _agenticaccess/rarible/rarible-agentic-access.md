---
acting_count: 27
action_class_counts:
  acting: 27
  connected: 65
api_specs:
- filename: rarible-charts-api-openapi.yml
  format: yaml
  label: Rarible Charts API
  slug: rarible-charts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rarible/refs/heads/main/openapi/rarible-charts-api-openapi.yml
- filename: rarible-collection-leader-board-api-openapi.yml
  format: yaml
  label: Rarible Collection Leader Board API
  slug: rarible-collection-leader-board-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rarible/refs/heads/main/openapi/rarible-collection-leader-board-api-openapi.yml
- filename: rarible-collection-statistics-api-openapi.yml
  format: yaml
  label: Rarible Collection Statistics API
  slug: rarible-collection-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rarible/refs/heads/main/openapi/rarible-collection-statistics-api-openapi.yml
- filename: rarible-currencies-and-rates-api-openapi.yml
  format: yaml
  label: Rarible Currencies and rates API
  slug: rarible-currencies-and-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rarible/refs/heads/main/openapi/rarible-currencies-and-rates-api-openapi.yml
- filename: rarible-domain-lookup-api-openapi.yml
  format: yaml
  label: Rarible Domain lookup API
  slug: rarible-domain-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rarible/refs/heads/main/openapi/rarible-domain-lookup-api-openapi.yml
- filename: rarible-encode-operations-api-openapi.yml
  format: yaml
  label: Rarible Encode operations API
  slug: rarible-encode-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rarible/refs/heads/main/openapi/rarible-encode-operations-api-openapi.yml
- filename: rarible-indexer-blocks-api-openapi.yml
  format: yaml
  label: Rarible Indexer blocks API
  slug: rarible-indexer-blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rarible/refs/heads/main/openapi/rarible-indexer-blocks-api-openapi.yml
- filename: rarible-nft-activities-api-openapi.yml
  format: yaml
  label: Rarible NFT Activities API
  slug: rarible-nft-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rarible/refs/heads/main/openapi/rarible-nft-activities-api-openapi.yml
- filename: rarible-nft-collections-api-openapi.yml
  format: yaml
  label: Rarible NFT Collections API
  slug: rarible-nft-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rarible/refs/heads/main/openapi/rarible-nft-collections-api-openapi.yml
- filename: rarible-nft-data-and-historical-statistics-api-openapi.yml
  format: yaml
  label: Rarible NFT Data and Historical Statistics API
  slug: rarible-nft-data-and-historical-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rarible/refs/heads/main/openapi/rarible-nft-data-and-historical-statistics-api-openapi.yml
- filename: rarible-nft-items-api-openapi.yml
  format: yaml
  label: Rarible NFT Items API
  slug: rarible-nft-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rarible/refs/heads/main/openapi/rarible-nft-items-api-openapi.yml
- filename: rarible-nft-ownerships-api-openapi.yml
  format: yaml
  label: Rarible NFT Ownerships API
  slug: rarible-nft-ownerships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rarible/refs/heads/main/openapi/rarible-nft-ownerships-api-openapi.yml
- filename: rarible-nft-sales-api-openapi.yml
  format: yaml
  label: Rarible NFT Sales API
  slug: rarible-nft-sales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rarible/refs/heads/main/openapi/rarible-nft-sales-api-openapi.yml
- filename: rarible-points-api-openapi.yml
  format: yaml
  label: Rarible Points API
  slug: rarible-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rarible/refs/heads/main/openapi/rarible-points-api-openapi.yml
- filename: rarible-reconciliation-api-openapi.yml
  format: yaml
  label: Rarible Reconciliation API
  slug: rarible-reconciliation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rarible/refs/heads/main/openapi/rarible-reconciliation-api-openapi.yml
- filename: rarible-search-api-api-openapi.yml
  format: yaml
  label: Rarible Search API API
  slug: rarible-search-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rarible/refs/heads/main/openapi/rarible-search-api-api-openapi.yml
- filename: rarible-signature-operations-api-openapi.yml
  format: yaml
  label: Rarible Signature operations API
  slug: rarible-signature-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rarible/refs/heads/main/openapi/rarible-signature-operations-api-openapi.yml
- filename: rarible-user-balances-api-openapi.yml
  format: yaml
  label: Rarible User balances API
  slug: rarible-user-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rarible/refs/heads/main/openapi/rarible-user-balances-api-openapi.yml
consequence_counts:
  physical: 9
  read: 65
  safety-critical: 3
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Rarible Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v0.1/collections/{collection}/refreshMeta
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v0.1/collections/{collection}/resetMeta
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v0.1/items/{itemId}/resetMeta
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v0.1/encode/order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v0.1/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v0.1/orders/byIds
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v0.1/orders/{id}/prepareCancelTx
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v0.1/orders/{id}/prepareTx
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v0.1/orders/{id}/report
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v0.1/ownerships/byIds
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v0.1/ownerships/search
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v0.1/signature/validate
operation_count: 92
overview: 'Rarible exposes 92 API operations that an AI agent could call, of which 27 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 65 read, 15 write, 9 physical, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Rarible
provider_slug: rarible
slug: rarible-agentic-access
source_filename: rarible-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 92\n  by_action_class:\n    connected: 65\n    acting: 27\n  by_consequence:\n    read: 65\n    write: 15\n    safety-critical: 3\n    physical: 9\n  human_in_the_loop_required: 3\noperations:\n- path: /v0.1/items/{itemId}\n  method: get\n  operationId: getItemById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/items/byIds\n  method: post\n  operationId: getItemByIds\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.1/items/{itemId}/royalties\n  method: get\n  operationId: getItemRoyaltiesById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/items/{itemId}/resetMeta\n  method: delete\n  operationId: resetItemMeta\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v0.1/items/byOwner\n  method: get\n  operationId: getItemsByOwner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v0.1/items/byCreator\n  method: get\n  operationId: getItemsByCreator\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/items/byCollection\n  method: get\n  operationId: getItemsByCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/items/byOwnerWithOwnership\n  method: get\n  operationId: getItemsByOwnerWithOwnership\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/items/all\n  method: get\n  operationId: getAllItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/items/traits\n  method: get\n  operationId: queryTraits\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/items/traits/search\n  method: get\n  operationId: searchTraits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/items/traits/rarity\n  method: post\n  operationId: queryTraitsWithRarity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.1/items/search\n  method: post\n  operationId: searchItems\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v0.1/items/search/duplicates\n  method: post\n  operationId: searchDuplicatedItems\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.1/items/lazy/{itemId}\n  method: get\n  operationId: getLazyItemById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/items/lazy/mint\n  method: post\n  operationId: mintLazyItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v0.1/items/lazy/burn\n  method: post\n  operationId: burnLazyItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.1/ownerships/{ownershipId}\n  method: get\n  operationId: getOwnershipById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/ownerships/byIds\n  method: post\n  operationId: getOwnershipsByIds\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v0.1/ownerships/byCollection\n  method: get\n  operationId: getOwnershipsByCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/ownerships/byItem\n  method: get\n  operationId: getOwnershipsByItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/ownerships/search\n  method: post\n  operationId: searchOwnerships\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.1/ownerships/collections\n  method: get\n  operationId: getCollectionsWithOwnedItems\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/orders/{id}\n  method: get\n  operationId: getOrderById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/orders/{id}/prepareTx\n  method: post\n  operationId: prepareOrderTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.1/orders/{id}/prepareCancelTx\n  method: post\n  operationId: prepareOrderCancelTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.1/orders/{id}/report\n  method: post\n  operationId: reportOrderById\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.1/orders\n  method: post\n  operationId: upsertOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v0.1/orders/{id}/validate\n  method: get\n  operationId: getValidatedOrderById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/orders/byIds\n  method: post\n  operationId: getOrdersByIds\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.1/orders/all\n  method: get\n  operationId: getOrdersAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/orders/sync\n  method: get\n  operationId: getAllSync\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/orders/sell/byMaker\n  method: get\n  operationId: getSellOrdersByMaker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/orders/sell/byItem\n  method: get\n  operationId: getSellOrdersByItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/orders/sell\n  method: get\n  operationId: getSellOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/orders/bids/byMaker\n  method: get\n  operationId: getOrderBidsByMaker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v0.1/orders/bids/byItem\n  method: get\n  operationId: getOrderBidsByItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/orders/floorBids/byCollection\n  method: get\n  operationId: getOrderFloorBidsByCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/orders/settings/fees\n  method: get\n  operationId: getOrderFees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/orders/history/bestActiveAtTime\n  method: get\n  operationId: getBestActiveOrdersAtTime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/orders/history/closestActiveAtTime/byOrder\n\
  \  method: get\n  operationId: getClosestActiveOrdersAtTimeByOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/orders/history/closestActiveAtTime/byPrice\n  method: get\n  operationId: getClosestActiveOrdersAtTimeByPrice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/activities/byUser\n  method: get\n  operationId: getActivitiesByUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/activities/byUsers\n  method: post\n  operationId: getActivitiesByUsers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.1/activities/byItem\n  method: get\n  operationId: getActivitiesByItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/activities/byCollection\n  method: get\n  operationId: getActivitiesByCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/activities/sync\n  method: get\n  operationId: getAllActivitiesSync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/activities/all\n  method: get\n  operationId: getAllActivities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v0.1/collections/{id}/charts/sales\n  method: get\n  operationId: getSalesChart\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/activities/search\n  method: post\n  operationId: searchActivities\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.1/activities/search/count\n  method: post\n  operationId: searchActivitiesCount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.1/collections/{collection}\n\
  \  method: get\n  operationId: getCollectionById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/collections/{collection}/generateTokenId\n  method: get\n  operationId: generateTokenId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/collections/{collection}/refreshMeta\n  method: delete\n  operationId: refreshCollectionItemsMeta\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v0.1/collections/{collection}/resetMeta\n  method: delete\n  operationId: resetCollectionMeta\n  x-agentic-access:\n  \
  \  action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v0.1/collections/byOwner\n  method: get\n  operationId: getCollectionsByOwner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/collections/all\n  method: get\n  operationId: getAllCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/collections/search\n  method: post\n  operationId: searchCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n \
  \     human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.1/data/rankings/{entity}/volume\n  method: get\n  operationId: getUserRankingByVolume\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/data/rankings/collections/volume\n  method: get\n  operationId: getCollectionRankingByVolume\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2.0/data/leaderboard/collections\n  method: get\n  operationId: getCollectionLeaderboard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2.0/data/leaderboard/collections/byOwner\n  method: get\n  operationId: getCollectionLeaderboardByOwner\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2.0/data/collections/{id}/statistics/global\n  method: get\n  operationId: getGlobalCollectionStatistics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2.0/data/collections/statistics/global/byIds\n  method: post\n  operationId: getGlobalCollectionStatisticsByIds\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2.0/data/collections/statistics/aggregated\n  method: post\n  operationId: getCollectionsAggregatedStatistics\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2.0/data/collections/{id}/statistics/period\n  method: get\n  operationId: getPeriodCollectionStatistics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2.0/data/collections/statistics/period/byIds\n  method: post\n  operationId: getPeriodCollectionStatisticsByIds\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2.0/data/collections/{id}/owners\n  method: get\n  operationId: getOwners\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2.0/data/collections/{id}/bidsByPrice\n  method: get\n  operationId: getBidsByPrice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2.0/data/collections/{id}/charts/floorPrice\n  method: get\n  operationId: getFloorPriceChart\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2.0/data/collections/{id}/charts/volume\n  method: get\n  operationId: getVolumeChart\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/data/collections/{collection}/transactions\n  method: get\n  operationId: getTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n \
  \   token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/data/collections/{collection}/stats\n  method: get\n  operationId: getCollectionStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/data/collections/{collection}/statistics\n  method: get\n  operationId: getCollectionStatistics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/data/collections/{collection}/sellers\n  method: get\n  operationId: getSellers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/data/collections/{collection}/gmv\n  method: get\n  operationId: getGmv\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v0.1/data/collections/{collection}/floorPrice\n  method: get\n  operationId: getFloorPrice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/data/collections/{collection}/buyers\n  method: get\n  operationId: getBuyers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/data/collections/{collection}/listed\n  method: get\n  operationId: getListed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/domains/{domain}/resolution\n  method: post\n  operationId: resolve\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n   \
  \   human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.1/signature/validate\n  method: post\n  operationId: validate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.1/signature/input\n  method: post\n  operationId: getInput\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.1/encode/order\n  method: post\n  operationId: encode\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.1/currencies/{currencyId}/rates/usd\n  method: get\n  operationId: getUsdRate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/currencies/all\n  method: get\n  operationId: getAllCurrencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/balances/{currencyId}/{owner}\n  method: get\n  operationId: getBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/points/rewards\n  method: get\n \
  \ operationId: getPointsRewards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/points/rewards/{address}\n  method: get\n  operationId: getPointsRewardsByAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/points/claim/signature\n  method: get\n  operationId: getClaimSignature\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/reconciliation/items\n  method: get\n  operationId: getReconciliationItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/reconciliation/collections\n  method: get\n  operationId: getReconciliationCollections\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/blocks/latestIndexed\n  method: get\n  operationId: getLatestIndexedBlock\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rarible/refs/heads/main/agentic-access/rarible-agentic-access.yml
summary_line: 92 operations · 27 acting · 3 human-in-the-loop
tags:
- NFT
- Non-Fungible Tokens
- Marketplace
- Aggregator
- Multichain
- Ethereum
- Polygon
- Arbitrum
- Flow
- Web3
- Blockchain
- Collections
- Order Book
- Trading
- Indexer
---
