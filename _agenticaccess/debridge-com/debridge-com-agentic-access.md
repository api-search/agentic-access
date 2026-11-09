---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 34
api_specs:
- filename: debridge-com-appcontrollerv10-api-openapi.yml
  format: yaml
  label: deBridge App Controller V10 API
  slug: debridge-com-appcontrollerv10-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/debridge-com/openapi/debridge-com-appcontrollerv10-api-openapi.yml
- filename: debridge-com-dln-api-openapi.yml
  format: yaml
  label: deBridge DLN API
  slug: debridge-com-dln-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/debridge-com/openapi/debridge-com-dln-api-openapi.yml
- filename: debridge-com-orders-api-openapi.yml
  format: yaml
  label: deBridge Orders API
  slug: debridge-com-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/debridge-com/openapi/debridge-com-orders-api-openapi.yml
- filename: debridge-com-samechainswap-api-openapi.yml
  format: yaml
  label: deBridge Same Chain Swap API
  slug: debridge-com-samechainswap-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/debridge-com/openapi/debridge-com-samechainswap-api-openapi.yml
- filename: debridge-com-satistics-api-openapi.yml
  format: yaml
  label: deBridge Satistics API
  slug: debridge-com-satistics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/debridge-com/openapi/debridge-com-satistics-api-openapi.yml
- filename: debridge-com-single-chain-swap-api-openapi.yml
  format: yaml
  label: deBridge single chain swap API
  slug: debridge-com-single-chain-swap-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/debridge-com/openapi/debridge-com-single-chain-swap-api-openapi.yml
- filename: debridge-com-tokenmetadata-api-openapi.yml
  format: yaml
  label: deBridge Token Metadata API
  slug: debridge-com-tokenmetadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/debridge-com/openapi/debridge-com-tokenmetadata-api-openapi.yml
- filename: debridge-com-transaction-api-openapi.yml
  format: yaml
  label: deBridge Transaction API
  slug: debridge-com-transaction-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/debridge-com/openapi/debridge-com-transaction-api-openapi.yml
- filename: debridge-com-users-api-openapi.yml
  format: yaml
  label: deBridge Users API
  slug: debridge-com-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/debridge-com/openapi/debridge-com-users-api-openapi.yml
- filename: debridge-com-utils-api-openapi.yml
  format: yaml
  label: deBridge Utils API
  slug: debridge-com-utils-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/debridge-com/openapi/debridge-com-utils-api-openapi.yml
- filename: debridge-com-order-events-api-openapi.yml
  format: yaml
  label: deBridge Order Events API
  slug: debridge-com-order-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/debridge-com/openapi/debridge-com-order-events-api-openapi.yml
- filename: debridge-com-referral-program-api-openapi.yml
  format: yaml
  label: deBridge Referral Program API
  slug: debridge-com-referral-program-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/debridge-com/openapi/debridge-com-referral-program-api-openapi.yml
- filename: debridge-com-terms-and-conditions-api-openapi.yml
  format: yaml
  label: deBridge Terms And Conditions API
  slug: debridge-com-terms-and-conditions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/debridge-com/openapi/debridge-com-terms-and-conditions-api-openapi.yml
consequence_counts:
  physical: 1
  read: 34
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Debridge Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/Orders/getForUnlockAuthorities
operation_count: 38
overview: 'deBridge exposes 38 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 34 read, 3 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: deBridge
provider_slug: debridge-com
slug: debridge-com-agentic-access
source_filename: debridge-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/create-tx.json, openapi/monitoring.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 38\n  by_action_class:\n    connected: 34\n    acting: 4\n  by_consequence:\n    read: 34\n    physical: 1\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /v1.0/dln/order/create-tx\n  method: get\n  operationId: DlnOrderControllerV10_createOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.0/dln/order/{id}\n  method: get\n  operationId: DlnOrderControllerV10_getOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.0/dln/order/{id}/status\n  method: get\n  operationId: DlnOrderControllerV10_getOrderStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.0/dln/tx/{hash}/order-ids\n  method: get\n  operationId: DlnOrderControllerV10_getOrderIdsByTx\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.0/dln/order/{id}/cancel-tx\n  method: get\n  operationId: DlnOrderControllerV10_cancelOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.0/dln/order/{id}/extcall-cancel-tx\n  method: get\n  operationId: DlnOrderControllerV10_extCallCancelOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.0/supported-chains\n  method: get\n  operationId: AppControllerV10_getSupportedChainResponse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.0/supported-chains-info\n  method: get\n  operationId: AppControllerV10_getSupportedChainInfoResponse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.0/token-list\n  method: get\n  operationId: AppControllerV10_getTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.0/chain/transaction\n  method: get\n  operationId: SingleSwapControllerV10_getChainTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n \
  \   subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.0/chain/estimation\n  method: get\n  operationId: SingleSwapControllerV10_getChainEstimation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/OrderEvents/solanaDepositsAndWithdrawals\n  method: get\n  operationId: OrderEvents_GetSolanaDepositsAndWithdrawals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Orders/filteredList\n  method: post\n  operationId: Orders_GetOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Orders/{orderId}\n  method: get\n  operationId: Orders_GetOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Orders/creationTxHash/{creationTxHash}\n  method: get\n  operationId: Orders_GetOrderByCreationTx\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Orders/{orderId}/externalCallProcess\n  method: get\n  operationId: Orders_GetExternalCallProcessedEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Orders/getInitiatorsPendingOrdersCount\n  method: get\n  operationId: Orders_GetInitiatorsPendingOrdersCount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Orders/{orderId}/state\n  method: get\n  operationId: Orders_GetOrderState\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Orders/{orderId}/liteModel\n  method: get\n  operationId: Orders_GetLiteOrderModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Orders/getForUnlockAuthorities\n  method: post\n  operationId: Orders_GetOrdersInfoForUnlockAuthorities\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/ReferralProgram/{referralCode}/summary\n  method: get\n  operationId: ReferralProgram_GetReferralStatistics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/ReferralProgram/{referralCode}/referredUsers\n  method: get\n  operationId: ReferralProgram_GetReferredUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ReferralProgram/referrerCode/{walletAddress}\n  method: get\n  operationId: ReferralProgram_GetReferrerCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/SameChainSwap/{swapId}\n  method: get\n  operationId: SameChainSwap_GetSameChainSwap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/SameChainSwap/{chainId}/tx/{transactionHash}\n  method: get\n  operationId: SameChainSwap_GetSwapByTx\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Satistics/getAllTime\n  method: get\n  operationId: Satistics_GetAllTime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Satistics/getLatestTwentyFourHours\n  method: get\n  operationId: Satistics_GetLatestTwentyFourHours\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Satistics/getDaily\n  method: get\n  operationId: Satistics_GetDailyStatistics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Satistics/{takerAddress}/lockedAssets\n  method: get\n  operationId: Satistics_GetLockedAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n   \
  \ subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/TermsAndConditions/signConditions\n  method: post\n  operationId: TermsAndConditions_SignConditions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/TermsAndConditions/{signatoryAddress}/hasSigned\n  method: get\n  operationId: TermsAndConditions_CheckIfTermsAreSigned\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/TermsAndConditions/current\n  method: get\n  operationId: TermsAndConditions_GetCurrent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/TokenMetadata/popularTokens\n\
  \  method: get\n  operationId: TokenMetadata_GetPopularTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/TokenMetadata/popularTokens/{chainId}\n  method: get\n  operationId: TokenMetadata_GetPopularTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Transaction/{orderCreationTransactionHash}/orderIds\n  method: get\n  operationId: Transaction_GetOrdersFromTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Transaction/{transactionHash}/liteModels\n  method: get\n  operationId: Transaction_GetLiteOrderModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/Users/usersLeaderboard\n  method: post\n  operationId: Users_GetUserLeaderBoard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Users/referralProgramLeaderboard\n  method: post\n  operationId: Users_GetReferralProgramLeaderboard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/debridge-com/agentic-access/debridge-com-agentic-access.yml
summary_line: 38 operations · 4 acting
tags:
- Cross-Chain Bridge
- DeFi Infrastructure
- Crypto Swaps
- Analytics
---
