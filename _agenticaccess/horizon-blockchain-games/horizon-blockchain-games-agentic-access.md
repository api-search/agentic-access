---
acting_count: 302
action_class_counts:
  acting: 302
api_specs:
- filename: horizon-blockchain-games-indexer-openapi-original.json
  format: json
  label: Sequence Indexer API
  slug: sequence-indexer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/horizon-blockchain-games/refs/heads/main/openapi/horizon-blockchain-games-indexer-openapi-original.json
- filename: horizon-blockchain-games-metadata-openapi-original.json
  format: json
  label: Sequence Metadata API
  slug: sequence-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/horizon-blockchain-games/refs/heads/main/openapi/horizon-blockchain-games-metadata-openapi-original.json
- filename: horizon-blockchain-games-marketplace-openapi-original.json
  format: json
  label: Sequence Marketplace API
  slug: sequence-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/horizon-blockchain-games/refs/heads/main/openapi/horizon-blockchain-games-marketplace-openapi-original.json
- filename: horizon-blockchain-games-transactions-openapi-original.json
  format: json
  label: Sequence Transactions (Relayer) API
  slug: sequence-transactions-relayer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/horizon-blockchain-games/refs/heads/main/openapi/horizon-blockchain-games-transactions-openapi-original.json
- filename: horizon-blockchain-games-analytics-openapi-original.json
  format: json
  label: Sequence Analytics API
  slug: sequence-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/horizon-blockchain-games/refs/heads/main/openapi/horizon-blockchain-games-analytics-openapi-original.json
- filename: horizon-blockchain-games-builder-openapi-original.json
  format: json
  label: Sequence Builder API
  slug: sequence-builder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/horizon-blockchain-games/refs/heads/main/openapi/horizon-blockchain-games-builder-openapi-original.json
- filename: horizon-blockchain-games-infrastructure-openapi-original.json
  format: json
  label: Sequence API (Infrastructure)
  slug: sequence-api-infrastructure
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/horizon-blockchain-games/refs/heads/main/openapi/horizon-blockchain-games-infrastructure-openapi-original.json
consequence_counts:
  physical: 18
  safety-critical: 1
  write: 283
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Horizon Blockchain Games Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /rpc/Analytics/TrailsTopTransactions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rpc/Analytics/AverageShopPurchasePrice
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rpc/Analytics/GetOrderbookCollections
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rpc/Analytics/TotalMarketplaceItemsPurchased
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rpc/Analytics/TotalMarketplaceTradedCollections
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rpc/Analytics/TotalShopItemsPurchased
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rpc/Analytics/TotalShopPurchasers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rpc/Analytics/TrailsDailyPaymentCompletionPercentage
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rpc/Analytics/TrailsMonthlyPaymentCompletionPercentage
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rpc/Analytics/TrailsPaymentCompletionPercentage
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rpc/Indexer/GetOrderbookOrders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rpc/Indexer/GetTopOrders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rpc/Marketplace/CheckoutOptionsMarketplace
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rpc/Marketplace/CheckoutOptionsSalesContract
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rpc/Marketplace/GenerateBuyTransaction
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rpc/Marketplace/GetFloorOrder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rpc/Marketplace/GetOrders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rpc/Marketplace/ListCollectibles
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rpc/Relayer/ListGasSponsors
operation_count: 302
overview: 'Horizon Blockchain Games exposes 302 API operations that an AI agent could call, of which 302 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 283 write, 18 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Horizon Blockchain Games
provider_slug: horizon-blockchain-games
slug: horizon-blockchain-games-agentic-access
source_filename: horizon-blockchain-games-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/horizon-blockchain-games-analytics-openapi-original.json, openapi/horizon-blockchain-games-builder-openapi-original.json,\n  openapi/horizon-blockchain-games-indexer-openapi-original.json, openapi/horizon-blockchain-games-infrastructure-openapi-original.json,\n  openapi/horizon-blockchain-games-marketplace-openapi-original.json, openapi/horizon-blockchain-games-metadata-openapi-original.json,\n  openapi/horizon-blockchain-games-transactions-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 302\n  by_action_class:\n    acting: 302\n  by_consequence:\n    write: 283\n    physical: 18\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /rpc/Analytics/TotalCompute\n\
  \  method: post\n  operationId: Analytics-TotalCompute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/ComputeByService\n  method: post\n  operationId: Analytics-ComputeByService\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/DailyComputeByType\n  method: post\n  operationId: Analytics-DailyComputeByType\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/DailyComputeByService\n  method: post\n  operationId: Analytics-DailyComputeByService\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/GetOrderbookCollections\n  method: post\n  operationId: Analytics-GetOrderbookCollections\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/CreditsPerDailyActiveUser\n  method: post\n  operationId:\
  \ Analytics-CreditsPerDailyActiveUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/CreditsPerMonthlyActiveUser\n  method: post\n  operationId: Analytics-CreditsPerMonthlyActiveUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/WalletsTotal\n  method: post\n  operationId: Analytics-WalletsTotal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/WalletsDaily\n  method: post\n  operationId: Analytics-WalletsDaily\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/WalletsMonthly\n  method: post\n  operationId: Analytics-WalletsMonthly\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/WalletsByCountry\n  method: post\n  operationId: Analytics-WalletsByCountry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/WalletsByDevice\n  method: post\n  operationId: Analytics-WalletsByDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/WalletsByBrowser\n  method: post\n  operationId: Analytics-WalletsByBrowser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/WalletsByOS\n  method: post\n\
  \  operationId: Analytics-WalletsByOS\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/WalletsByType\n  method: post\n  operationId: Analytics-WalletsByType\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/WalletsTxnSentTotal\n  method: post\n  operationId: Analytics-WalletsTxnSentTotal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n     \
  \ triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/WalletsTxnSentDaily\n  method: post\n  operationId: Analytics-WalletsTxnSentDaily\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/WalletsTxnSentMonthly\n  method: post\n  operationId: Analytics-WalletsTxnSentMonthly\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/WalletsByOrigin\n  method: post\n  operationId: Analytics-WalletsByOrigin\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/ConnectionsByOrigin\n  method: post\n  operationId: Analytics-ConnectionsByOrigin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/MarketTxnEventTotal\n  method: post\n  operationId: Analytics-MarketTxnEventTotal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/MarketTxnEventDaily\n\
  \  method: post\n  operationId: Analytics-MarketTxnEventDaily\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/MarketTxnEventMonthly\n  method: post\n  operationId: Analytics-MarketTxnEventMonthly\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/MarketWalletsTotal\n  method: post\n  operationId: Analytics-MarketWalletsTotal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n     \
  \ human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/MarketWalletsDaily\n  method: post\n  operationId: Analytics-MarketWalletsDaily\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/MarketWalletsMonthly\n  method: post\n  operationId: Analytics-MarketWalletsMonthly\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/TotalWalletTxnConversionRate\n  method: post\n  operationId: Analytics-TotalWalletTxnConversionRate\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/DailyWalletTxnConversionRate\n  method: post\n  operationId: Analytics-DailyWalletTxnConversionRate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/MonthlyWalletTxnConversionRate\n  method: post\n  operationId: Analytics-MonthlyWalletTxnConversionRate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/DailyNewWallets\n  method: post\n  operationId: Analytics-DailyNewWallets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/MonthlyNewWallets\n  method: post\n  operationId: Analytics-MonthlyNewWallets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/TotalNewWallets\n  method: post\n  operationId: Analytics-TotalNewWallets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/AverageDAU\n  method: post\n  operationId: Analytics-AverageDAU\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/RollingStickiness\n  method: post\n  operationId: Analytics-RollingStickiness\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/AverageStickiness\n  method:\
  \ post\n  operationId: Analytics-AverageStickiness\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/D1RetentionByCohort\n  method: post\n  operationId: Analytics-D1RetentionByCohort\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/D3RetentionByCohort\n  method: post\n  operationId: Analytics-D3RetentionByCohort\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/D7RetentionByCohort\n  method: post\n  operationId: Analytics-D7RetentionByCohort\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/D14RetentionByCohort\n  method: post\n  operationId: Analytics-D14RetentionByCohort\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/D28RetentionByCohort\n  method: post\n  operationId: Analytics-D28RetentionByCohort\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/AverageD1Retention\n  method: post\n  operationId: Analytics-AverageD1Retention\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/AverageD3Retention\n  method: post\n  operationId: Analytics-AverageD3Retention\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /rpc/Analytics/AverageD7Retention\n  method: post\n  operationId: Analytics-AverageD7Retention\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/AverageD14Retention\n  method: post\n  operationId: Analytics-AverageD14Retention\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/AverageD28Retention\n  method: post\n  operationId: Analytics-AverageD28Retention\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n   \
  \   max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/MonthlyActiveWalletsBySegment\n  method: post\n  operationId: Analytics-MonthlyActiveWalletsBySegment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/MonthlyTransactingWalletsBySegment\n  method: post\n  operationId: Analytics-MonthlyTransactingWalletsBySegment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/WeeklyActiveWallets\n\
  \  method: post\n  operationId: Analytics-WeeklyActiveWallets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/TotalViews\n  method: post\n  operationId: Analytics-TotalViews\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/DailyViews\n  method: post\n  operationId: Analytics-DailyViews\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n     \
  \ triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/ViewsByCountry\n  method: post\n  operationId: Analytics-ViewsByCountry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/ViewsByDevice\n  method: post\n  operationId: Analytics-ViewsByDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/ViewsByOS\n  method: post\n  operationId: Analytics-ViewsByOS\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n   \
  \ audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/DailyUniqueVisitors\n  method: post\n  operationId: Analytics-DailyUniqueVisitors\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/MonthlyUniqueVisitors\n  method: post\n  operationId: Analytics-MonthlyUniqueVisitors\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/ActiveSessions\n  method:\
  \ post\n  operationId: Analytics-ActiveSessions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/UserEvents\n  method: post\n  operationId: Analytics-UserEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/EcosystemTotalWallets\n  method: post\n  operationId: Analytics-EcosystemTotalWallets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/EcosystemTotalProjects\n  method: post\n  operationId: Analytics-EcosystemTotalProjects\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/EcosystemTotalProjectsCreated\n  method: post\n  operationId: Analytics-EcosystemTotalProjectsCreated\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/EcosystemTotalActiveProjects\n  method: post\n  operationId: Analytics-EcosystemTotalActiveProjects\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/EcosystemTotalDevelopers\n  method: post\n  operationId: Analytics-EcosystemTotalDevelopers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/EcosystemActiveDevelopers\n  method: post\n  operationId: Analytics-EcosystemActiveDevelopers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /rpc/Analytics/EcosystemDailyActiveWallets\n  method: post\n  operationId: Analytics-EcosystemDailyActiveWallets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/EcosystemMonthlyActiveWallets\n  method: post\n  operationId: Analytics-EcosystemMonthlyActiveWallets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/EcosystemDailyNewProjects\n  method: post\n  operationId: Analytics-EcosystemDailyNewProjects\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/EcosystemMonthlyNewProjects\n  method: post\n  operationId: Analytics-EcosystemMonthlyNewProjects\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/EcosystemTotalContracts\n  method: post\n  operationId: Analytics-EcosystemTotalContracts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /rpc/Analytics/EcosystemMonthlyContracts\n  method: post\n  operationId: Analytics-EcosystemMonthlyContracts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/EcosystemTopProjectsByActiveWallets\n  method: post\n  operationId: Analytics-EcosystemTopProjectsByActiveWallets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/EcosystemTopProjectsByNewWallets\n  method: post\n  operationId: Analytics-EcosystemTopProjectsByNewWallets\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/EcosystemWalletsCreated\n  method: post\n  operationId: Analytics-EcosystemWalletsCreated\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/EcosystemMonthlyActiveEcoWallets\n  method: post\n  operationId: Analytics-EcosystemMonthlyActiveEcoWallets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /rpc/Analytics/EcosystemDailyNewWallets\n  method: post\n  operationId: Analytics-EcosystemDailyNewWallets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/EcosystemMonthlyNewWallets\n  method: post\n  operationId: Analytics-EcosystemMonthlyNewWallets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/EcosystemTopProjectsByDeveloperActivity\n  method: post\n  operationId: Analytics-EcosystemTopProjectsByDeveloperActivity\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/EcosystemTopProjectsByNewDevelopers\n  method: post\n  operationId: Analytics-EcosystemTopProjectsByNewDevelopers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/EcosystemTotalMarketplaces\n  method: post\n  operationId: Analytics-EcosystemTotalMarketplaces\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/EcosystemMonthlyMarketplaces\n  method: post\n  operationId: Analytics-EcosystemMonthlyMarketplaces\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/EcosystemActiveMarketplaces\n  method: post\n  operationId: Analytics-EcosystemActiveMarketplaces\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/EcosystemWalletsByCountry\n  method: post\n  operationId: Analytics-EcosystemWalletsByCountry\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/EcosystemWalletsByDevice\n  method: post\n  operationId: Analytics-EcosystemWalletsByDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/EcosystemWalletsByOS\n  method: post\n  operationId: Analytics-EcosystemWalletsByOS\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n     \
  \ - high-value\n    audit: required\n- path: /rpc/Analytics/EcosystemWalletsByBrowser\n  method: post\n  operationId: Analytics-EcosystemWalletsByBrowser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/EcosystemWalletsByType\n  method: post\n  operationId: Analytics-EcosystemWalletsByType\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/Analytics/EcosystemWalletsByLoginMethod\n  method: post\n  operationId: Analytics-EcosystemWalletsByLoginMethod\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    toke\n\n# --- truncated at 32 KB (118 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/horizon-blockchain-games/refs/heads/main/agentic-access/horizon-blockchain-games-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/horizon-blockchain-games/refs/heads/main/agentic-access/horizon-blockchain-games-agentic-access.yml
summary_line: 302 operations · 302 acting · 1 human-in-the-loop
tags:
- Company
- Consumer
- Blockchain
- Web3
- Gaming
- NFT
- Wallet
- Cryptocurrency
- Smart Contracts
- Marketplace
- Developer Tools
- Ethereum
---
