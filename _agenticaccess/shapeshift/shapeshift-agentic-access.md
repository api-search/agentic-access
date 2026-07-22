---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 18
api_specs:
- filename: shapeshift-ethereum-openapi.json
  format: json
  label: ShapeShift Unchained — Ethereum (EVM) API
  slug: shapeshift-unchained-ethereum-evm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shapeshift/refs/heads/main/openapi/shapeshift-ethereum-openapi.json
- filename: shapeshift-bitcoin-openapi.json
  format: json
  label: ShapeShift Unchained — Bitcoin (UTXO) API
  slug: shapeshift-unchained-bitcoin-utxo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shapeshift/refs/heads/main/openapi/shapeshift-bitcoin-openapi.json
- filename: shapeshift-solana-openapi.json
  format: json
  label: ShapeShift Unchained — Solana API
  slug: shapeshift-unchained-solana-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shapeshift/refs/heads/main/openapi/shapeshift-solana-openapi.json
consequence_counts:
  physical: 3
  read: 18
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Shapeshift Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/send
operation_count: 25
overview: 'Shapeshift exposes 25 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read, 4 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Shapeshift
provider_slug: shapeshift
slug: shapeshift-agentic-access
source_filename: shapeshift-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/shapeshift-bitcoin-openapi.json, openapi/shapeshift-ethereum-openapi.json, openapi/shapeshift-solana-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 25\n  by_action_class:\n    connected: 18\n    acting: 7\n  by_consequence:\n    read: 18\n    physical: 3\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/info\n  method: get\n  operationId: GetInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/account/{pubkey}\n  method: get\n  operationId: GetAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/account/{pubkey}/txs\n  method: get\n  operationId: GetTxHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/account/{pubkey}/utxos\n  method: get\n  operationId: GetUtxos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tx/{txid}\n  method: get\n  operationId: GetTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tx/{txid}/raw\n  method: get\n  operationId: GetRawTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/send\n  method: post\n\
  \  operationId: SendTx\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/fees\n  method: get\n  operationId: GetNetworkFees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/info\n  method: get\n  operationId: GetInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/account/{pubkey}\n  method: get\n  operationId: GetAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/v1/account/{pubkey}/txs\n  method: get\n  operationId: GetTxHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tx/{txid}\n  method: get\n  operationId: GetTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/send\n  method: post\n  operationId: SendTx\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/jsonrpc\n  method: post\n  operationId: DoRpcRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/gas/estimate\n  method: post\n  operationId: EstimateGas\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/gas/fees\n  method: get\n  operationId: GetGasFees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/info\n  method: get\n  operationId: GetInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/account/{pubkey}\n  method:\
  \ get\n  operationId: GetAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/account/{pubkey}/txs\n  method: get\n  operationId: GetTxHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tx/{txid}\n  method: get\n  operationId: GetTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/send\n  method: post\n  operationId: SendTx\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/v1/fees/priority\n  method: get\n  operationId: GetPriorityFees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/fees/estimate\n  method: post\n  operationId: EstimateFees\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/jsonrpc\n  method: post\n  operationId: DoRpcRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/token/{id}\n  method: get\n  operationId:\
  \ GetToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shapeshift/refs/heads/main/agentic-access/shapeshift-agentic-access.yml
summary_line: 25 operations · 7 acting
tags:
- Company
- Cryptocurrency
- Blockchain
- Bitcoin
- Ethereum
- Web3
- DeFi
- Wallet
- Trading
- Multichain
- API
---
