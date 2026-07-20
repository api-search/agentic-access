---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 11
api_specs:
- filename: dflow-openapi-original.json
  format: json
  label: DFlow Trading API (Aggregator)
  slug: dflow-trading-api-aggregator
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dflow/refs/heads/main/openapi/dflow-openapi-original.json
consequence_counts:
  read: 11
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Dflow Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'DFlow exposes 14 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: DFlow
provider_slug: dflow
slug: dflow-agentic-access
source_filename: dflow-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/dflow-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 11\n    acting: 3\n  by_consequence:\n    read: 11\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /health-check\n  method: get\n  operationId: handler_health_check\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /intent\n  method: get\n  operationId: intent_handler\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /order\n  method: get\n  operationId:\
  \ order_handler\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /order-status\n  method: get\n  operationId: order_status_handler\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /prediction-market-init\n  method: get\n  operationId: prediction_market_init_handler\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /priority-fees\n  method: get\n  operationId: priority_fees_handler\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /priority-fees/stream\n  method: get\n  operationId: priority_fee_stream_handler\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /quote\n  method: get\n  operationId: quote_handler\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /submit-intent\n  method: post\n  operationId: submit_intent_handler\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /swap\n  method: post\n  operationId: swap_handler\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /swap-instructions\n\
  \  method: post\n  operationId: swap_instructions_handler\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tokens\n  method: get\n  operationId: tokens_handler\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tokens-with-decimals\n  method: get\n  operationId: tokens_with_decimals_handler\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /venues\n  method: get\n  operationId: venues_handler\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dflow/refs/heads/main/agentic-access/dflow-agentic-access.yml
summary_line: 14 operations · 3 acting
tags:
- Company
- Crypto Web3
- Solana
- Trading API
- DeFi
- DEX Aggregator
- Token Swap
- Blockchain
- MEV Protection
- Prediction Markets
- Agent Ready
---
