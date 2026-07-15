---
acting_count: 0
action_class_counts:
  connected: 48
api_specs:
- filename: openapi.yml
  format: yaml
  label: BarnBridge SMART Yield API
  slug: barnbridge-smart-yield-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barnbridge/refs/heads/main/openapi.yml
- filename: openapi.yml
  format: yaml
  label: BarnBridge Governance API
  slug: barnbridge-governance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barnbridge/refs/heads/main/openapi/openapi.yml
- filename: openapi.yml
  format: yaml
  label: BarnBridge SMART Alpha API
  slug: barnbridge-smart-alpha-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barnbridge/refs/heads/main/openapi/openapi.yml
- filename: openapi.yml
  format: yaml
  label: BarnBridge SMART Exposure API
  slug: barnbridge-smart-exposure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barnbridge/refs/heads/main/openapi/openapi.yml
- filename: openapi.yml
  format: yaml
  label: BarnBridge Yield Farming API
  slug: barnbridge-yield-farming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barnbridge/refs/heads/main/openapi/openapi.yml
consequence_counts:
  read: 48
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Barnbridge Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 48
overview: 'BarnBridge exposes 48 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 48 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BarnBridge
provider_slug: barnbridge
slug: barnbridge-agentic-access
source_filename: barnbridge-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 48\n  by_action_class:\n    connected: 48\n  by_consequence:\n    read: 48\n  human_in_the_loop_required: 0\noperations:\n- path: /api/smartyield/pools\n  method: get\n  operationId: listSmartYieldPools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/smartyield/pools/{address}\n  method: get\n  operationId: getSmartYieldPool\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/smartyield/pools/{address}/apy\n\
  \  method: get\n  operationId: getSmartYieldPoolAPYTrend\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/smartyield/pools/{address}/liquidity\n  method: get\n  operationId: getSmartYieldPoolLiquidity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/smartyield/pools/{address}/transactions\n  method: get\n  operationId: listSmartYieldPoolTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/smartyield/pools/{address}/senior-bonds\n  method: get\n  operationId: listSmartYieldSeniorBonds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/smartyield/pools/{address}/junior-bonds\n\
  \  method: get\n  operationId: listSmartYieldJuniorBonds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/smartyield/rewards/pools\n  method: get\n  operationId: listSmartYieldRewardPools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/smartyield/rewards/pools/{poolAddress}/transactions\n  method: get\n  operationId: listSmartYieldRewardPoolTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/smartyield/rewards/v2/pools\n  method: get\n  operationId: listSmartYieldRewardPoolsV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/smartyield/rewards/v2/pools/{poolAddress}/transactions\n\
  \  method: get\n  operationId: listSmartYieldRewardPoolTransactionsV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/smartyield/users/{address}/history\n  method: get\n  operationId: getSmartYieldUserHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/smartyield/users/{address}/redeems/senior\n  method: get\n  operationId: getSmartYieldUserSeniorRedeems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/smartyield/users/{address}/junior-past-positions\n  method: get\n  operationId: getSmartYieldUserJuniorPastPositions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/smartyield/users/{address}/portfolio-value\n  method: get\n  operationId: getSmartYieldUserPortfolioValue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/smartyield/users/{address}/portfolio-value/junior\n  method: get\n  operationId: getSmartYieldUserJuniorPortfolioValue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/smartyield/users/{address}/portfolio-value/senior\n  method: get\n  operationId: getSmartYieldUserSeniorPortfolioValue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/smartalpha/pools\n  method: get\n  operationId: listSmartAlphaPools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/smartalpha/pools/{poolAddress}/tokens-price-chart\n  method: get\n  operationId: getSmartAlphaTokensPriceChart\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/smartalpha/pools/{poolAddress}/pool-performance-chart\n  method: get\n  operationId: getSmartAlphaPoolPerformanceChart\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/smartalpha/pools/{poolAddress}/previous-epochs\n  method: get\n  operationId: listSmartAlphaPreviousEpochs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/smartalpha/users/{address}/portfolio-value\n  method: get\n  operationId: getSmartAlphaUserPortfolioValue\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/smartalpha/users/{address}/queue-positions\n  method: get\n  operationId: getSmartAlphaUserQueuePositions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/smartalpha/transactions\n  method: get\n  operationId: listSmartAlphaTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/smartalpha/rewards/pools\n  method: get\n  operationId: listSmartAlphaRewardPools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/smartalpha/rewards/pools/{poolAddress}/transactions\n  method: get\n  operationId: listSmartAlphaRewardPoolTransactions\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/smartexposure/pools\n  method: get\n  operationId: listSmartExposurePools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/smartexposure/tranches\n  method: get\n  operationId: listSmartExposureTranches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/smartexposure/tranches/{eTokenAddress}\n  method: get\n  operationId: getSmartExposureTranche\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/smartexposure/tranches/{eTokenAddress}/etoken-price\n  method: get\n  operationId: getSmartExposureETokenPriceChart\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/smartexposure/tranches/{eTokenAddress}/price-trend\n  method: get\n  operationId: getSmartExposurePriceTrend\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/smartexposure/tranches/{eTokenAddress}/liquidity\n  method: get\n  operationId: getSmartExposureTrancheLiquidity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/smartexposure/tranches/{eTokenAddress}/ratio-deviation\n  method: get\n  operationId: getSmartExposureRatioDeviation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/smartexposure/transactions\n\
  \  method: get\n  operationId: listSmartExposureTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/smartexposure/users/{userAddress}/portfolio-value\n  method: get\n  operationId: getSmartExposureUserPortfolioValue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/governance/proposals\n  method: get\n  operationId: listGovernanceProposals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/governance/proposals/{proposalID}\n  method: get\n  operationId: getGovernanceProposal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/governance/proposals/{proposalID}/votes\n\
  \  method: get\n  operationId: listGovernanceProposalVotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/governance/proposals/{proposalID}/events\n  method: get\n  operationId: listGovernanceProposalEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/governance/overview\n  method: get\n  operationId: getGovernanceOverview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/governance/voters\n  method: get\n  operationId: listGovernanceVoters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/governance/abrogation-proposals\n  method: get\n  operationId:\
  \ listAbrogationProposals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/governance/abrogation-proposals/{proposalID}\n  method: get\n  operationId: getAbrogationProposal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/governance/abrogation-proposals/{proposalID}/votes\n  method: get\n  operationId: listAbrogationProposalVotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/governance/treasury/transactions\n  method: get\n  operationId: listTreasuryTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/governance/treasury/tokens\n  method:\
  \ get\n  operationId: listTreasuryTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/yieldfarming/staking-actions/list\n  method: get\n  operationId: listYieldFarmingStakingActions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/yieldfarming/staking-actions/chart\n  method: get\n  operationId: getYieldFarmingStakingActionsChart\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/barnbridge/refs/heads/main/agentic-access/barnbridge-agentic-access.yml
summary_line: 48 operations
tags:
- DeFi
- Risk Tokenization
- Yield
- Blockchain
- Ethereum
- SMART Yield
- Structured Products
- Tranches
---
