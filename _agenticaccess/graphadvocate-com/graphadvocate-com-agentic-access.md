---
acting_count: 23
action_class_counts:
  acting: 23
api_specs:
- filename: graphadvocate-com-openapi.yml
  format: yaml
  label: Graph Advocate API
  slug: graph-advocate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/graphadvocate-com/refs/heads/main/openapi/graphadvocate-com-openapi.yml
consequence_counts:
  physical: 6
  safety-critical: 4
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 4
kind: agentic-access
layout: agentic-access
method: generated
name: Graphadvocate Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /hyperliquid/score
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /polymarket/leaders
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /polymarket/pnl-quick
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /polymarket/screen
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /hyperliquid/pnl
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /hyperliquid/screen
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /kalshi-polymarket/spread
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /polymarket/pnl
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /uniswap/pretrade
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /uniswap/traders
operation_count: 23
overview: 'PaulieB14 exposes 23 API operations that an AI agent could call, of which 23 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 write, 6 physical, and 4 safety-critical.


  4 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: PaulieB14
provider_slug: graphadvocate-com
slug: graphadvocate-com-agentic-access
source_filename: graphadvocate-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: generated\nsource: openapi/graphadvocate-com-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    acting: 23\n  by_consequence:\n    write: 13\n    physical: 6\n    safety-critical: 4\n  human_in_the_loop_required: 4\noperations:\n- path: /route\n  method: post\n  operationId: routeQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/score\n  method: post\n  operationId: agentScore\n  x-agentic-access:\n    action-class: acting\n   \
  \ consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ask\n  method: post\n  operationId: askSettlements\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hyperliquid/fills\n  method: post\n  operationId: hyperliquidFills\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hyperliquid/pnl\n  method: post\n  operationId: hyperliquidPnl\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hyperliquid/risk\n  method: post\n  operationId: hyperliquidRisk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hyperliquid/score\n  method: post\n  operationId: hyperliquidScore\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /hyperliquid/screen\n  method: post\n  operationId: hyperliquidScreen\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hyperliquid/vault\n  method: post\n  operationId: hyperliquidVault\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /kalshi-polymarket/spread\n  method: post\n  operationId: kalshiPolymarketSpread\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /kalshi/consensus-trend\n  method: post\n  operationId: kalshiConsensusTrend\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /kalshi/sports-live-edge\n  method: post\n  operationId: kalshiSportsLiveEdge\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /onchain-x402/address\n  method:\
  \ post\n  operationId: onchainX402Address\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /polymarket/pnl\n  method: post\n  operationId: polymarketPnl\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /polymarket/pnl-quick\n  method: post\n  operationId: polymarketPnlQuick\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /polymarket/risk\n  method: post\n  operationId: polymarketRisk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /polymarket/screen\n  method: post\n  operationId: polymarketScreen\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /polymarket/leaders\n  method: post\n  operationId: polymarketLeaders\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /predmarket/spread\n  method: post\n  operationId: predmarketSpread\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /narrative/divergence\n  method: post\n  operationId: narrativeDivergence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /uniswap/basis\n  method: post\n  operationId:\
  \ uniswapBasis\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /uniswap/pretrade\n  method: post\n  operationId: uniswapPretrade\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /uniswap/traders\n  method: post\n  operationId: uniswapTraders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/graphadvocate-com/refs/heads/main/agentic-access/graphadvocate-com-agentic-access.yml
summary_line: 23 operations · 23 acting · 4 human-in-the-loop
tags:
- Blockchain
- On-Chain Data
- The Graph
- Subgraph
- GraphQL
- MCP
- A2A
- x402
- Agentic Commerce
- AI Agents
- DeFi
- Prediction Markets
- Trader Intelligence
- Web3
---
