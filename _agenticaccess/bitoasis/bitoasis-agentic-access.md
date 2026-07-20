---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 17
api_specs:
- filename: bitoasis-exchange-openapi.yml
  format: yaml
  label: BitOasis Exchange API
  slug: bitoasis-exchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitoasis/refs/heads/main/openapi/bitoasis-exchange-openapi.yml
consequence_counts:
  physical: 6
  read: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bitoasis Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /exchange/cancel-order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /exchange/coin-deposit
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /exchange/coin-withdrawal
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /exchange/fiat-withdrawal
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /exchange/fiat-withdrawal/{withdrawal_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /exchange/order
operation_count: 23
overview: 'BitOasis exposes 23 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read and 6 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BitOasis
provider_slug: bitoasis
slug: bitoasis-agentic-access
source_filename: bitoasis-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/bitoasis-exchange-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 17\n    acting: 6\n  by_consequence:\n    read: 17\n    physical: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /exchange/markets\n  method: get\n  operationId: getMarkets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exchange/ticker/{pair}\n  method: get\n  operationId: getTicker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exchange/order-book/{pair}\n\
  \  method: get\n  operationId: getOrderBook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exchange/trades/{pair}\n  method: get\n  operationId: getTrades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exchange/balances\n  method: get\n  operationId: getBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exchange/banks\n  method: get\n  operationId: getBanks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exchange/orders/{pair}\n  method: get\n  operationId: getOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /exchange/order/{order_id}\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exchange/order\n  method: post\n  operationId: placeOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /exchange/cancel-order\n  method: post\n  operationId: cancelOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /exchange/coin-deposits/{currency}\n  method: get\n  operationId: getCoinDeposits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exchange/coin-deposit/{deposit_id}\n  method: get\n  operationId: getCoinDeposit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exchange/coin-deposit\n  method: post\n  operationId: newCoinDepositAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /exchange/coin-withdrawals/{currency}\n\
  \  method: get\n  operationId: getCoinWithdrawals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exchange/coin-withdrawal/{withdrawal_id}\n  method: get\n  operationId: getCoinWithdrawal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exchange/coin-withdrawal\n  method: post\n  operationId: newCoinWithdrawal\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /exchange/coin-withdrawal-fees\n  method: get\n  operationId: getCoinWithdrawalFees\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exchange/fiat-deposits\n  method: get\n  operationId: getFiatDeposits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exchange/fiat-deposit/{deposit_id}\n  method: get\n  operationId: getFiatDeposit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exchange/fiat-withdrawals\n  method: get\n  operationId: getFiatWithdrawals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exchange/fiat-withdrawal/{withdrawal_id}\n  method: get\n  operationId: getFiatWithdrawal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /exchange/fiat-withdrawal/{withdrawal_id}\n  method: delete\n  operationId: cancelFiatWithdrawal\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /exchange/fiat-withdrawal\n  method: post\n  operationId: newFiatWithdrawal\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitoasis/refs/heads/main/agentic-access/bitoasis-agentic-access.yml
summary_line: 23 operations · 6 acting
tags:
- Company
- Crypto
- Cryptocurrency
- Exchange
- Trading
- Digital Assets
- Bitcoin
- MENA
- Fintech
- MCP
---
