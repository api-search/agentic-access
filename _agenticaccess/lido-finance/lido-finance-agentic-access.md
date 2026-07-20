---
acting_count: 0
action_class_counts:
  connected: 18
api_specs:
- filename: lido-finance-eth-api-openapi-original.json
  format: json
  label: Lido Ethereum API
  slug: lido-ethereum-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lido-finance/refs/heads/main/openapi/lido-finance-eth-api-openapi-original.json
- filename: lido-finance-withdrawal-queue-openapi-original.json
  format: json
  label: Lido Withdrawals API
  slug: lido-withdrawals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lido-finance/refs/heads/main/openapi/lido-finance-withdrawal-queue-openapi-original.json
- filename: lido-finance-reward-history-openapi-original.json
  format: json
  label: Lido Reward History Backend API
  slug: lido-reward-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lido-finance/refs/heads/main/openapi/lido-finance-reward-history-openapi-original.json
consequence_counts:
  read: 18
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Lido Finance Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 18
overview: 'Lido Finance exposes 18 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Lido Finance
provider_slug: lido-finance
slug: lido-finance-agentic-access
source_filename: lido-finance-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/lido-finance-eth-api-openapi-original.json, openapi/lido-finance-reward-history-openapi-original.json,\n  openapi/lido-finance-withdrawal-queue-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    connected: 18\n  by_consequence:\n    read: 18\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/protocol/eth/apr\n  method: get\n  operationId: ProtocolController_findAPRforEth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/protocol/eth/price\n  method: get\n  operationId: ProtocolController_findEthPrice\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/protocol/eth/apr/last\n  method: get\n  operationId: ProtocolController_findLastAPRforEth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/protocol/steth/apr\n  method: get\n  operationId: ProtocolController_findAPRforSTETH\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/protocol/steth/price\n  method: get\n  operationId: ProtocolController_findStEthPrice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/protocol/steth/stats\n  method: get\n  operationId: ProtocolController_findStethStats\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/protocol/steth/apr/last\n  method: get\n  operationId: ProtocolController_findLastAPRforSTETH\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/protocol/steth/apr/sma\n  method: get\n  operationId: ProtocolController_findSmaAPRforSTETH\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/swap/one-inch\n  method: get\n  operationId: SwapController_findOneInchRate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/swap/jumper\n  method: get\n  operationId: SwapController_findJumperRate\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: RewardsController_rewards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/request-time\n  method: get\n  operationId: RequestTimeController_requestTimeV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/request-time\n  method: get\n  operationId: RequestTimeController_requestsTime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/request-time/calculate\n  method: get\n  operationId: RequestTimeController_calculateTime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/nft/{tokenId}\n  method: get\n  operationId: NFTController_nftMetaV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/nft/{tokenId}/image\n  method: get\n  operationId: NFTController_nftImageV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/estimate-gas\n  method: get\n  operationId: EstimateController_requestTimeV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/validators-info\n  method: get\n  operationId: ValidatorsController_validatorsV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lido-finance/refs/heads/main/agentic-access/lido-finance-agentic-access.yml
summary_line: 18 operations
tags:
- Company
- Blockchain
- Ethereum
- Liquid Staking
- DeFi
- Cryptocurrency
- Staking
- Web3
- Financial Services
- GraphQL
---
