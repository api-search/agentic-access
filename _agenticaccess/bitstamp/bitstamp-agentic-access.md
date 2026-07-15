---
acting_count: 0
action_class_counts:
  connected: 7
api_specs:
- filename: openapi.json
  format: json
  label: Bitstamp REST API
  slug: bitstamp-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitstamp/refs/heads/main/openapi/openapi.json
consequence_counts:
  read: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bitstamp Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Bitstamp exposes 7 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bitstamp
provider_slug: bitstamp
slug: bitstamp-agentic-access
source_filename: bitstamp-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 7\n  by_consequence:\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v2/ticker/{currency_pair}/\n  method: get\n  operationId: getticker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/ticker_hour/{currency_pair}/\n  method: get\n  operationId: gethourlyticker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/order_book/{currency_pair}/\n\
  \  method: get\n  operationId: getorderbook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/transactions/{currency_pair}/\n  method: get\n  operationId: gettransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/trading-pairs-info/\n  method: get\n  operationId: gettradingpairsinfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/ohlc/{currency_pair}/\n  method: get\n  operationId: getohlcdata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/currencies/\n  method: get\n  operationId: getcurrencies\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitstamp/refs/heads/main/agentic-access/bitstamp-agentic-access.yml
summary_line: 7 operations
tags:
- Cryptocurrency
- Exchange
- Trading
- Bitcoin
- Ethereum
- Spot Trading
- WebSocket
- Market Data
- Order Management
- Finance
---
