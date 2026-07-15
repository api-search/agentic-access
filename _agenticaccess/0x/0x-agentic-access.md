---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 18
api_specs:
- filename: 0x-api.yaml
  format: yaml
  label: 0x Swap API
  slug: swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/0x/refs/heads/main/openapi/0x-api.yaml
- filename: 0x-api.yaml
  format: yaml
  label: 0x Gasless API
  slug: gasless-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/0x/refs/heads/main/openapi/0x-api.yaml
- filename: 0x-cross-chain.yaml
  format: yaml
  label: 0x Cross-Chain API
  slug: cross-chain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/0x/refs/heads/main/openapi/0x-cross-chain.yaml
- filename: 0x-api.yaml
  format: yaml
  label: 0x Trade Analytics API
  slug: trade-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/0x/refs/heads/main/openapi/0x-api.yaml
- filename: 0x-api.yaml
  format: yaml
  label: 0x Sources API
  slug: sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/0x/refs/heads/main/openapi/0x-api.yaml
consequence_counts:
  physical: 1
  read: 18
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: 0X Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /gasless/submit
operation_count: 19
overview: '0x exposes 19 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: 0x
provider_slug: 0x
slug: 0x-agentic-access
source_filename: 0x-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/0x-api.yaml, openapi/0x-cross-chain.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    connected: 18\n    acting: 1\n  by_consequence:\n    read: 18\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /swap/allowance-holder/price\n  method: get\n  operationId: swap::allowanceHolder::getPrice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /swap/allowance-holder/quote\n  method: get\n  operationId: swap::allowanceHolder::getQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n   \
  \ token:\n      max-ttl: 3600\n    audit: none\n- path: /swap/permit2/price\n  method: get\n  operationId: swap::permit2::getPrice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /swap/permit2/quote\n  method: get\n  operationId: swap::permit2::getQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /swap/chains\n  method: get\n  operationId: swap::chains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gasless/price\n  method: get\n  operationId: gasless::getPrice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gasless/quote\n  method: get\n  operationId: gasless::getQuote\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gasless/submit\n  method: post\n  operationId: gasless::submit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gasless/status/{tradeHash}\n  method: get\n  operationId: gasless::getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gasless/gasless-approval-tokens\n  method: get\n  operationId: gasless::getGaslessApprovalTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /gasless/chains\n  method: get\n  operationId: gasless::chains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sources\n  method: get\n  operationId: sources::getSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trade-analytics/swap\n  method: get\n  operationId: tradeAnalytics::swap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trade-analytics/gasless\n  method: get\n  operationId: tradeAnalytics::gasless\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cross-chain/quotes\n  method: get\n  operationId: crossChain::getQuotes\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cross-chain/status\n  method: get\n  operationId: crossChain::getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cross-chain/sources\n  method: get\n  operationId: crossChain::listSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cross-chain/tx-history-beta\n  method: get\n  operationId: crossChain::getTxHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cross-chain/quotes/stream\n  method: get\n  operationId: crossChain::streamQuotes\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/0x/refs/heads/main/agentic-access/0x-agentic-access.yml
summary_line: 19 operations · 1 acting
tags:
- Cryptocurrency
- DeFi
- DEX Aggregator
- Swap
- Gasless
- Cross-Chain
- Permit2
- Liquidity
- Trade Analytics
- Web3
- Settlement
- Smart Contracts
---
