---
acting_count: 35
action_class_counts:
  acting: 35
  connected: 58
api_specs:
- filename: reservoir-accounts-api-openapi.yml
  format: yaml
  label: Reservoir Accounts API
  slug: reservoir-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-accounts-api-openapi.yml
- filename: reservoir-activity-api-openapi.yml
  format: yaml
  label: Reservoir Activity API
  slug: reservoir-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-activity-api-openapi.yml
- filename: reservoir-attributes-api-openapi.yml
  format: yaml
  label: Reservoir Attributes API
  slug: reservoir-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-attributes-api-openapi.yml
- filename: reservoir-chain-api-openapi.yml
  format: yaml
  label: Reservoir Chain API
  slug: reservoir-chain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-chain-api-openapi.yml
- filename: reservoir-collections-api-openapi.yml
  format: yaml
  label: Reservoir Collections API
  slug: reservoir-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-collections-api-openapi.yml
- filename: reservoir-events-api-openapi.yml
  format: yaml
  label: Reservoir Events API
  slug: reservoir-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-events-api-openapi.yml
- filename: reservoir-manage-orders-api-openapi.yml
  format: yaml
  label: Reservoir Manage Orders API
  slug: reservoir-manage-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-manage-orders-api-openapi.yml
- filename: reservoir-management-api-openapi.yml
  format: yaml
  label: Reservoir Management API
  slug: reservoir-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-management-api-openapi.yml
- filename: reservoir-marketplace-api-openapi.yml
  format: yaml
  label: Reservoir Marketplace API
  slug: reservoir-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-marketplace-api-openapi.yml
- filename: reservoir-misc-api-openapi.yml
  format: yaml
  label: Reservoir Misc API
  slug: reservoir-misc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-misc-api-openapi.yml
- filename: reservoir-orders-api-openapi.yml
  format: yaml
  label: Reservoir Orders API
  slug: reservoir-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-orders-api-openapi.yml
- filename: reservoir-owners-api-openapi.yml
  format: yaml
  label: Reservoir Owners API
  slug: reservoir-owners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-owners-api-openapi.yml
- filename: reservoir-redirects-api-openapi.yml
  format: yaml
  label: Reservoir Redirects API
  slug: reservoir-redirects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-redirects-api-openapi.yml
- filename: reservoir-sales-api-openapi.yml
  format: yaml
  label: Reservoir Sales API
  slug: reservoir-sales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-sales-api-openapi.yml
- filename: reservoir-sources-api-openapi.yml
  format: yaml
  label: Reservoir Sources API
  slug: reservoir-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-sources-api-openapi.yml
- filename: reservoir-stats-api-openapi.yml
  format: yaml
  label: Reservoir Stats API
  slug: reservoir-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-stats-api-openapi.yml
- filename: reservoir-tokens-api-openapi.yml
  format: yaml
  label: Reservoir Tokens API
  slug: reservoir-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-tokens-api-openapi.yml
- filename: reservoir-transfers-api-openapi.yml
  format: yaml
  label: Reservoir Transfers API
  slug: reservoir-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-transfers-api-openapi.yml
- filename: reservoir-x-deprecated-api-openapi.yml
  format: yaml
  label: Reservoir X Deprecated API
  slug: reservoir-x-deprecated-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/openapi/reservoir-x-deprecated-api-openapi.yml
consequence_counts:
  physical: 9
  read: 58
  safety-critical: 5
  write: 21
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 5
kind: agentic-access
layout: agentic-access
method: generated
name: Reservoir Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /collections/disable-metadata/v1
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /collections/{collection}/override/v1
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /collections/{collection}/override/v2
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /tokens/disable-metadata/v1
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /tokens/{token}/override/v1
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /execute/cancel-signature/v1
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /execute/cancel/v3
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /execute/deposit/v1
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /execute/results/v1
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /execute/solve/v1
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /execute/transfer/v1
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /management/orders/simulate/v1
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /order/v4
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/invalidate/v1
operation_count: 93
overview: 'Reservoir exposes 93 API operations that an AI agent could call, of which 35 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 58 read, 21 write, 9 physical, and 5 safety-critical.


  5 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Reservoir
provider_slug: reservoir
slug: reservoir-agentic-access
source_filename: reservoir-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: generated\nsource: openapi/reservoir-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 93\n  by_action_class:\n    connected: 58\n    acting: 35\n  by_consequence:\n    read: 58\n    write: 21\n    safety-critical: 5\n    physical: 9\n  human_in_the_loop_required: 5\noperations:\n- path: /api-keys/{key}/rate-limits\n  method: get\n  operationId: getApikeysKeyRatelimits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chain/stats/v1\n  method: get\n  operationId: getChainStatsV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n    \
  \  max-ttl: 3600\n    audit: none\n- path: /collections-sets/v1\n  method: post\n  operationId: postCollectionssetsV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collections-sets/{collectionsSetId}/owners-distribution/v1\n  method: get\n  operationId: getCollectionssetsCollectionssetidOwnersdistributionV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/activity/v6\n  method: get\n  operationId: getCollectionsActivityV6\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/daily-volumes/v1\n  method: get\n  operationId:\
  \ getCollectionsDailyvolumesV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/disable-metadata/v1\n  method: post\n  operationId: postCollectionsDisablemetadataV1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /collections/nsfw-status/v1\n  method: post\n  operationId: postCollectionsNsfwstatusV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collections/refresh/v2\n\
  \  method: post\n  operationId: postCollectionsRefreshV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collections/search/v1\n  method: get\n  operationId: getCollectionsSearchV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/spam-status/v1\n  method: post\n  operationId: postCollectionsSpamstatusV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collections/trending-mints/v1\n  method: get\n  operationId:\
  \ getCollectionsTrendingmintsV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/trending-mints/v2\n  method: get\n  operationId: getCollectionsTrendingmintsV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/trending/v1\n  method: get\n  operationId: getCollectionsTrendingV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/v7\n  method: get\n  operationId: getCollectionsV7\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collectionId}/bids/v1\n  method: get\n  operationId: getCollectionsCollectionidBidsV1\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collection}/attributes/all/v4\n  method: get\n  operationId: getCollectionsCollectionAttributesAllV4\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collection}/attributes/explore/v6\n  method: get\n  operationId: getCollectionsCollectionAttributesExploreV6\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collection}/marketplace-configurations/v2\n  method: get\n  operationId: getCollectionsCollectionMarketplaceconfigurationsV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collection}/override/v1\n\
  \  method: post\n  operationId: postCollectionsCollectionOverrideV1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /collections/{collection}/override/v2\n  method: post\n  operationId: postCollectionsCollectionOverrideV2\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /collections/{collection}/owners-distribution/v1\n  method: get\n  operationId: getCollectionsCollectionOwnersdistributionV1\n  x-agentic-access:\n    action-class: connected\n   \
  \ consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collection}/top-traders/v1\n  method: get\n  operationId: getCollectionsCollectionToptradersV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts-sets/v1\n  method: post\n  operationId: postContractssetsV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cross-posting-orders/v1\n  method: get\n  operationId: getCrosspostingordersV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/asks/v3\n  method: get\n  operationId:\
  \ getEventsAsksV3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/bids/v3\n  method: get\n  operationId: getEventsBidsV3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/collections/floor-ask/v2\n  method: get\n  operationId: getEventsCollectionsFlooraskV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/collections/top-bid/v2\n  method: get\n  operationId: getEventsCollectionsTopbidV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/tokens/floor-ask/v4\n  method: get\n  operationId: getEventsTokensFlooraskV4\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /execute/auth-signature/v1\n  method: post\n  operationId: postExecuteAuthsignatureV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /execute/bid/v5\n  method: post\n  operationId: postExecuteBidV5\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /execute/buy/v7\n  method: post\n  operationId: postExecuteBuyV7\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /execute/call/v1\n  method: post\n  operationId: postExecuteCallV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /execute/cancel-signature/v1\n  method: post\n  operationId: postExecuteCancelsignatureV1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /execute/cancel/v3\n  method:\
  \ post\n  operationId: postExecuteCancelV3\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /execute/deposit/v1\n  method: post\n  operationId: postExecuteDepositV1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /execute/list/v5\n  method: post\n  operationId: postExecuteListV5\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /execute/mint/v1\n  method: post\n  operationId: postExecuteMintV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /execute/permit-signature/v1\n  method: post\n  operationId: postExecutePermitsignatureV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /execute/pre-signature/v1\n  method: post\n  operationId: postExecutePresignatureV1\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /execute/results/v1\n  method: post\n  operationId: postExecuteResultsV1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /execute/sell/v7\n  method: post\n  operationId: postExecuteSellV7\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /execute/solve/capacity/v1\n  method: post\n  operationId: postExecuteSolveCapacityV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /execute/solve/capacity/v2\n  method: post\n  operationId: postExecuteSolveCapacityV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /execute/solve/v1\n  method: post\n  operationId: postExecuteSolveV1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /execute/status/v1\n  method: post\n  operationId: postExecuteStatusV1\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /execute/transfer/v1\n  method: post\n  operationId: postExecuteTransferV1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /management/cosigners/v1\n  method: post\n  operationId: postManagementCosignersV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /management/mints/simulate/v1\n  method: post\n  operationId: postManagementMintsSimulateV1\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /management/orders/simulate/v1\n  method: post\n  operationId: postManagementOrdersSimulateV1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /order/v4\n  method: post\n  operationId: postOrderV4\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/asks/v5\n  method: get\n  operationId: getOrdersAsksV5\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/bids/v6\n  method: get\n  operationId: getOrdersBidsV6\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/depth/v1\n  method: get\n  operationId: getOrdersDepthV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/invalidate/v1\n  method: post\n  operationId: postOrdersInvalidateV1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/users/{user}/top-bids/v4\n  method: get\n  operationId: getOrdersUsersUserTopbidsV4\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /owners/common-collections/v1\n  method: get\n  operationId: getOwnersCommoncollectionsV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /owners/cross-collections/v1\n  method: get\n  operationId: getOwnersCrosscollectionsV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /owners/v2\n  method: get\n  operationId: getOwnersV2\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /redirect/collections/{collection}/image/v1\n  method: get\n  operationId: getRedirectCollectionsCollectionImageV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /redirect/currency/{address}/icon/v1\n  method: get\n  operationId: getRedirectCurrencyAddressIconV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /redirect/sources/{source}/logo/v2\n  method: get\n  operationId: getRedirectSourcesSourceLogoV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /redirect/sources/{source}/tokens/{token}/link/v2\n  method: get\n  operationId: getRedirectSourcesSourceTokensTokenLinkV2\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /redirect/tokens/{token}/image/v1\n  method: get\n  operationId: getRedirectTokensTokenImageV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sales/v6\n  method: get\n  operationId: getSalesV6\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/collections/v2\n  method: get\n  operationId: getSearchCollectionsV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sources/v1\n  method: get\n  operationId: getSourcesV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /stats/v2\n  method: get\n  operationId: getStatsV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /token-sets/v2\n  method: post\n  operationId: postTokensetsV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tokens/bootstrap/v1\n  method: get\n  operationId: getTokensBootstrapV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tokens/disable-metadata/v1\n  method: post\n  operationId: postTokensDisablemetadataV1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /tokens/flag/changes/v1\n  method: get\n  operationId: getTokensFlagChangesV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tokens/flag/v1\n  method: post\n  operationId: postTokensFlagV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tokens/floor/v1\n  method: get\n  operationId: getTokensFloorV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /tokens/ids/v1\n  method: get\n  operationId: getTokensIdsV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tokens/nsfw-status/v1\n  method: post\n  operationId: postTokensNsfwstatusV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tokens/refresh/v2\n  method: post\n  operationId: postTokensRefreshV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tokens/spam-status/v1\n  method:\
  \ post\n  operationId: postTokensSpamstatusV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tokens/v7\n  method: get\n  operationId: getTokensV7\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tokens/{token}/activity/v5\n  method: get\n  operationId: getTokensTokenActivityV5\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tokens/{token}/asks/v1\n  method: get\n  operationId: getTokensTokenAsksV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /tokens/{token}/bids/v1\n  method: get\n  operationId: getTokensTokenBidsV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tokens/{token}/override/v1\n  method: post\n  operationId: postTokensTokenOverrideV1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /transactions/synced/v2\n  method: get\n  operationId: getTransactionsSyncedV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/{txHash}/synced/v1\n  method: get\n  operationId: getTransactionsTxhashSyncedV1\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transfers/bulk/v2\n  method: get\n  operationId: getTransfersBulkV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transfers/v4\n  method: get\n  operationId: getTransfersV4\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/activity/v6\n  method: get\n  operationId: getUsersActivityV6\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{user}/asks/v1\n  method: get\n  operationId: getUsersUserAsksV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n \
  \   audit: none\n- path: /users/{user}/bids/v1\n  method: get\n  operationId: getUsersUserBidsV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{user}/collections/v4\n  method: get\n  operationId: getUsersUserCollectionsV4\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{user}/tokens/v10\n  method: get\n  operationId: getUsersUserTokensV10\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reservoir/refs/heads/main/agentic-access/reservoir-agentic-access.yml
summary_line: 93 operations · 35 acting · 5 human-in-the-loop
tags:
- NFT
- Blockchain
- Marketplace
- Ethereum
- EVM
- Liquidity
- Order Book
- Web3
- DeFi
- Trading
- Data API
---
