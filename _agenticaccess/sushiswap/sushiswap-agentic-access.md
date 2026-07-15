---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 9
api_specs:
- filename: blade-v2-openapi.json
  format: json
  label: Sushi Price API
  slug: sushi-price-api
  spec_type: OpenAPI
  url: https://docs.sushi.com/blade-v2-openapi.json
- filename: blade-v2-openapi.json
  format: json
  label: Sushi Quote API
  slug: sushi-quote-api
  spec_type: OpenAPI
  url: https://docs.sushi.com/blade-v2-openapi.json
- filename: blade-v2-openapi.json
  format: json
  label: Sushi Swap API
  slug: sushi-swap-api
  spec_type: OpenAPI
  url: https://docs.sushi.com/blade-v2-openapi.json
consequence_counts:
  physical: 1
  read: 9
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sushiswap Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rfq/v2/deposit
operation_count: 11
overview: 'SushiSwap exposes 11 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 1 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SushiSwap
provider_slug: sushiswap
slug: sushiswap-agentic-access
source_filename: sushiswap-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/blade-v2-openapi.json, openapi/sushi-api-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 9\n    acting: 2\n  by_consequence:\n    read: 9\n    write: 1\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /rfq/v2/pool/{chainId}\n  method: get\n  operationId: getPoolInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rfq/v2/quote/{chainId}\n  method: get\n  operationId: generateQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /rfq/sign\n  method: post\n  operationId: signQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rfq/v2/quote-sign/{chainId}\n  method: get\n  operationId: quoteAndSign\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rfq/v2/deposit\n  method: post\n  operationId: depositAssets\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /quote/v7/{chainId}\n\
  \  method: get\n  operationId: quote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /swap/v7/{chainId}\n  method: get\n  operationId: swap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /price/v1/{chainId}\n  method: get\n  operationId: prices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /price/v1/{chainId}/{tokenAddress}\n  method: get\n  operationId: price\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /token/v1/{chainId}/{tokenAddress}\n  method: get\n  operationId: token\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /liquidity-providers/v7/{chainId}\n  method: get\n  operationId: getLiquidityProviders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sushiswap/refs/heads/main/agentic-access/sushiswap-agentic-access.yml
summary_line: 11 operations · 2 acting
tags:
- DeFi
- Decentralized Exchange
- DEX
- Cryptocurrency
- Web3
- Blockchain
- Multi-Chain
- Liquidity
- Swap
- Token Pricing
---
