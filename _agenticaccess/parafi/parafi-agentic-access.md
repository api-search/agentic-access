---
acting_count: 0
action_class_counts:
  connected: 23
api_specs:
- filename: parafi-openapi.json
  format: json
  label: ParaFi Tech API
  slug: parafi-tech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parafi/refs/heads/main/openapi/parafi-openapi.json
consequence_counts:
  read: 23
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Parafi Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 23
overview: 'Parafi exposes 23 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 23 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Parafi
provider_slug: parafi
slug: parafi-agentic-access
source_filename: parafi-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/parafi-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 23\n  by_consequence:\n    read: 23\n  human_in_the_loop_required: 0\noperations:\n- path: /api/market/prices\n  method: get\n  operationId: getMarketPrices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/solana/validator-apy\n  method: get\n  operationId: getSolanaValidatorApy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/solana/network-validators\n  method:\
  \ get\n  operationId: getSolanaNetworkValidators\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/solana/supply\n  method: get\n  operationId: getSolanaSupply\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/solana/simple-rewards/epoch/{epochNumber}\n  method: get\n  operationId: getSolanaSimpleRewardsByEpoch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/avalanche/validators\n  method: get\n  operationId: getAvalancheValidators\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/avalanche/supply\n  method: get\n  operationId: getAvalancheSupply\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/solana/network-apy\n  method: get\n  operationId: getSolanaNetworkApy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/solana/validator-active-stake\n  method: get\n  operationId: getSolanaValidatorActiveStake\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/solana/validator-stake\n  method: get\n  operationId: getSolanaValidatorStake\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/solana/validator-delegators\n  method: get\n  operationId: getSolanaValidatorDelegators\n  x-agentic-access:\n    action-class: connected\n  \
  \  consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/solana/rewards/staker/{address}\n  method: get\n  operationId: getSolanaStakerRewards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/solana/rewards/validator/{voteAccount}\n  method: get\n  operationId: getSolanaValidatorRewards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/solana/rewards/epoch/{epochNumber}\n  method: get\n  operationId: getSolanaEpochRewards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/solana/mev-rewards\n  method: get\n  operationId: getSolanaMevRewards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/solana/compute-units\n  method: get\n  operationId: getSolanaComputeUnits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/solana/compute-units/history\n  method: get\n  operationId: getSolanaComputeUnitsHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/solana/leader-slots\n  method: get\n  operationId: getSolanaLeaderSlots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/solana/sidecar-stats\n  method: get\n  operationId: getSolanaSidecarStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/solana/network-stats/history\n  method: get\n  operationId: getSolanaNetworkStatsHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/solana/delegators\n  method: get\n  operationId: getSolanaDelegators\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ethereum/network-stats\n  method: get\n  operationId: getEthereumNetworkStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ethereum/sidecar-stats\n  method: get\n  operationId: getEthereumSidecarStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parafi/refs/heads/main/agentic-access/parafi-agentic-access.yml
summary_line: 23 operations
tags:
- Company
- Fintech
- Blockchain
- Digital Assets
- Staking
- Validators
- Solana
- Ethereum
- Avalanche
- DeFi
- Market Data
---
