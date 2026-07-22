---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 7
api_specs:
- filename: robinhood-crypto-trading-openapi.yml
  format: yaml
  label: Robinhood Crypto Trading API
  slug: robinhood-crypto-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/robinhood/refs/heads/main/openapi/robinhood-crypto-trading-openapi.yml
consequence_counts:
  physical: 2
  read: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Robinhood Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/crypto/trading/orders/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/crypto/trading/orders/{id}/cancel/
operation_count: 9
overview: 'Robinhood exposes 9 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Robinhood
provider_slug: robinhood
slug: robinhood-agentic-access
source_filename: robinhood-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/robinhood-crypto-trading-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 7\n    acting: 2\n  by_consequence:\n    read: 7\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/crypto/trading/accounts/\n  method: get\n  operationId: getCryptoTradingAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/crypto/marketdata/best_bid_ask/\n  method: get\n  operationId: getBestBidAsk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/v1/crypto/marketdata/estimated_price/\n  method: get\n  operationId: getEstimatedPrice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/crypto/trading/trading_pairs/\n  method: get\n  operationId: getTradingPairs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/crypto/trading/holdings/\n  method: get\n  operationId: getHoldings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/crypto/trading/orders/\n  method: get\n  operationId: getOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/crypto/trading/orders/\n\
  \  method: post\n  operationId: placeOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/crypto/trading/orders/{id}/\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/crypto/trading/orders/{id}/cancel/\n  method: post\n  operationId: cancelOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n     \
  \ - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/robinhood/refs/heads/main/agentic-access/robinhood-agentic-access.yml
summary_line: 9 operations · 2 acting
tags:
- Company
- Fintech
- Cryptocurrency
- Trading
- Brokerage
- Investing
- Financial Services
- Crypto
---
