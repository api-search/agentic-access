---
acting_count: 0
action_class_counts:
  connected: 20
api_specs:
- filename: stryke-api.yaml
  format: yaml
  label: Dopex CLAMM Options Trading API
  slug: clamm-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dopex/refs/heads/main/openapi/stryke-api.yaml
consequence_counts:
  read: 20
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Dopex Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 20
overview: 'Dopex exposes 20 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Dopex
provider_slug: dopex
slug: dopex-agentic-access
source_filename: dopex-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/stryke-api.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    connected: 20\n  by_consequence:\n    read: 20\n  human_in_the_loop_required: 0\noperations:\n- path: /clamm/purchase/quote\n  method: get\n  operationId: PurchaseController_getQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clamm/purchase/positions\n  method: get\n  operationId: PurchaseController_getPurchasePositions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clamm/purchase/history\n\
  \  method: get\n  operationId: PurchaseController_getHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clamm/deposit/prepare\n  method: get\n  operationId: DepositController_prepareDeposit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clamm/deposit/history\n  method: get\n  operationId: DepositController_getHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clamm/deposit/positions\n  method: get\n  operationId: DepositController_getPositions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clamm/withdraw/history\n  method: get\n  operationId: WithdrawController_getHistory\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clamm/exercise/prepare\n  method: get\n  operationId: ExerciseController_getExerciseTx\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clamm/exercise/history\n  method: get\n  operationId: ExerciseController_getHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clamm/strikes-chain\n  method: get\n  operationId: StrikesChainController_getStrikesChain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clamm/option-markets\n  method: get\n  operationId: OptionMarketsController_getOptionMarkets\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.1/clamm/option-markets\n  method: get\n  operationId: OptionMarketsController_getOptionMarketsV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clamm/stats/fees\n  method: get\n  operationId: StatsController_getFees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clamm/stats/volume\n  method: get\n  operationId: StatsController_getVolume\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clamm/stats/dau\n  method: get\n  operationId: StatsController_getDau\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clamm/stats/open-interest\n  method: get\n  operationId: StatsController_getOpenInterest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clamm/stats/tvl\n  method: get\n  operationId: StatsController_getTvl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clamm/stats/tvl/{pool}\n  method: get\n  operationId: StatsController_getTvlForPool\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clamm/stats/delta\n  method: get\n  operationId: StatsController_getPnlDelta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /xsyk/vest-positions/{account}\n  method: get\n  operationId: VestPositionsController_getUserData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dopex/refs/heads/main/agentic-access/dopex-agentic-access.yml
summary_line: 20 operations
tags:
- DeFi
- Decentralized Options
- SSOV
- Options Exchange
- Arbitrum
- DPX
- rDPX
- Staking
- Implied Volatility
- Black-Scholes
- Options Pricing
- CLAMM
- Cryptocurrency
- Web3
- EVM
---
