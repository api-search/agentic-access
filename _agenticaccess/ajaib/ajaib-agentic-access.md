---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 8
api_specs:
- filename: ajaib-market-info-api-openapi.yml
  format: yaml
  label: Ajaib Market Info API
  slug: ajaib-market-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ajaib/refs/heads/main/openapi/ajaib-market-info-api-openapi.yml
- filename: ajaib-spot-trading-api-openapi.yml
  format: yaml
  label: Ajaib Spot Trading API
  slug: ajaib-spot-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ajaib/refs/heads/main/openapi/ajaib-spot-trading-api-openapi.yml
- filename: ajaib-wallet-api-openapi.yml
  format: yaml
  label: Ajaib Wallet API
  slug: ajaib-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ajaib/refs/heads/main/openapi/ajaib-wallet-api-openapi.yml
consequence_counts:
  physical: 6
  read: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ajaib Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /coin/internal/v1/order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /coin/internal/v1/order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /coin/internal/v1/order/batch
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /coin/internal/v1/order/batch
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /coin/internal/v1/order/open
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /coin/internal/v1/order/self-trading
operation_count: 14
overview: 'Ajaib exposes 14 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 6 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Ajaib
provider_slug: ajaib
slug: ajaib-agentic-access
source_filename: ajaib-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: generated\nsource: openapi/ajaib-coin-exchange-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 8\n    acting: 6\n  by_consequence:\n    read: 8\n    physical: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /coin/internal/v1/public/time\n  method: get\n  operationId: getServerTime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coin/internal/v1/public/exchange-info\n  method: get\n  operationId: getExchangeInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /coin/internal/v1/depth\n  method: get\n  operationId: getDepth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coin/internal/v1/price\n  method: get\n  operationId: getPrice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coin/internal/v1/portfolio\n  method: get\n  operationId: getPortfolio\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coin/internal/v1/trades\n  method: get\n  operationId: getTrades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coin/internal/v1/order\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coin/internal/v1/order\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coin/internal/v1/order\n  method: delete\n  operationId: cancelOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coin/internal/v1/order/open\n  method: get\n  operationId: getOpenOrders\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coin/internal/v1/order/open\n  method: delete\n  operationId: cancelAllOpenOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coin/internal/v1/order/self-trading\n  method: post\n  operationId: createSelfTradingOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /coin/internal/v1/order/batch\n  method: post\n  operationId: createBatchOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coin/internal/v1/order/batch\n  method: delete\n  operationId: cancelBatchOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ajaib/refs/heads/main/agentic-access/ajaib-agentic-access.yml
summary_line: 14 operations · 6 acting
tags:
- Company
- Financial Services
- Investing
- Brokerage
- Trading
- Cryptocurrency
- Crypto Exchange
- Stocks
- Mutual Funds
- Fintech
- Indonesia
- Wealth Management
---
