---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 17
api_specs:
- filename: gte-openapi-original.yml
  format: yaml
  label: GTE API
  slug: gte-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gte/refs/heads/main/openapi/gte-openapi-original.yml
consequence_counts:
  physical: 1
  read: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Gte Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /exchange
operation_count: 18
overview: 'GTE exposes 18 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: GTE
provider_slug: gte
slug: gte-agentic-access
source_filename: gte-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/gte-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    connected: 17\n    acting: 1\n  by_consequence:\n    read: 17\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /health\n  method: get\n  operationId: GetServerHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /info\n  method: get\n  operationId: GetGTEInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tokens\n  method: get\n  operationId: GetTokens\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tokens/search\n  method: get\n  operationId: SearchTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tokens/{token_address}\n  method: get\n  operationId: GetTokenByAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets\n  method: get\n  operationId: GetMarkets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/search\n  method: get\n  operationId: SearchMarkets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /markets/{market_address}\n  method: get\n  operationId: GetMarketByAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/{market_address}/candles\n  method: get\n  operationId: GetMarketCandles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/{market_address}/trades\n  method: get\n  operationId: GetMarketTrades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/{market_address}/book\n  method: get\n  operationId: GetMarketBook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{user_address}/lppositions\n  method: get\n\
  \  operationId: GetUserLpPositions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{user_address}/portfolio\n  method: get\n  operationId: GetUserPortfolio\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{user_address}/trades\n  method: get\n  operationId: GetUserTrades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{user_address}/open_orders\n  method: get\n  operationId: GetOpenOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{user_address}/filled_orders\n  method: get\n  operationId: GetFilledOrders\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{user_address}/order_history\n  method: get\n  operationId: GetOrderHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exchange\n  method: post\n  operationId: Exchange\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gte/refs/heads/main/agentic-access/gte-agentic-access.yml
summary_line: 18 operations · 1 acting
tags:
- Company
- Crypto Defi
- Decentralized Exchange
- Trading
- Market Data
- Order Book
- Perpetuals
- MegaETH
- Blockchain
---
