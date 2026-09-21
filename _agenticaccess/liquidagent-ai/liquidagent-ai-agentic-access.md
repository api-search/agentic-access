---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 8
api_specs:
- filename: liquidagent-ai-openapi.yml
  format: yaml
  label: Liquid Agent Tokenized Stock Index and Gas Sponsor API
  slug: liquid-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liquidagent-ai/refs/heads/main/openapi/liquidagent-ai-openapi.yml
consequence_counts:
  physical: 3
  read: 8
  safety-critical: 1
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Liquidagent Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/create-vault
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/buy
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/gas
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/send
operation_count: 17
overview: 'Liquid Agent exposes 17 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 5 write, 3 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Liquid Agent
provider_slug: liquidagent-ai
slug: liquidagent-ai-agentic-access
source_filename: liquidagent-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: generated\nsource: openapi/liquidagent-ai-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    connected: 8\n    acting: 9\n  by_consequence:\n    read: 8\n    safety-critical: 1\n    write: 5\n    physical: 3\n  human_in_the_loop_required: 1\noperations:\n- path: /v1/guide\n  method: get\n  operationId: get_v1_guide\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/basket\n  method: get\n  operationId: get_v1_basket\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/vault/{address}\n  method: get\n  operationId: get_v1_vault_address\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/balance/{agent}\n  method: get\n  operationId: get_v1_balance_agent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/quote\n  method: get\n  operationId: get_v1_quote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/create-vault\n  method: post\n  operationId: post_v1_create-vault\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n     \
  \ human-in-the-loop: required\n    audit: required\n- path: /v1/set-weights\n  method: post\n  operationId: post_v1_set-weights\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/buy\n  method: post\n  operationId: post_v1_buy\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/redeem\n  method: post\n  operationId: post_v1_redeem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/rebalance\n  method: post\n  operationId: post_v1_rebalance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/send\n  method: post\n  operationId: post_v1_send\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/signals\n  method: get\n  operationId: getV1Signals\n  x-agentic-access:\n    action-class: connected\n \
  \   consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/publish\n  method: post\n  operationId: postV1Publish\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/gas/solana\n  method: get\n  operationId: getV1GasSolana\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/gas/solana\n  method: post\n  operationId: postV1GasSolana\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/gas\n  method: get\n  operationId: getV1Gas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/gas\n  method: post\n  operationId: postV1Gas\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liquidagent-ai/refs/heads/main/agentic-access/liquidagent-ai-agentic-access.yml
summary_line: 17 operations · 9 acting · 1 human-in-the-loop
tags:
- Tokenized Stocks
- DeFi
- Investing
- Agentic Commerce
- x402
- Stablecoins
- Account Abstraction
- Gas Sponsorship
- Base
- Solana
- AI Agents
- agent-native
- A2A
- Portfolio-Management
- Market Data
---
