---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 11
api_specs:
- filename: monero-blockchain-api-openapi.yml
  format: yaml
  label: Monero Blockchain API
  slug: monero-blockchain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monero/refs/heads/main/openapi/monero-blockchain-api-openapi.yml
- filename: monero-json-rpc-api-openapi.yml
  format: yaml
  label: Monero JSON-RPC API
  slug: monero-json-rpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monero/refs/heads/main/openapi/monero-json-rpc-api-openapi.yml
- filename: monero-mining-api-openapi.yml
  format: yaml
  label: Monero Mining API
  slug: monero-mining-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monero/refs/heads/main/openapi/monero-mining-api-openapi.yml
- filename: monero-network-api-openapi.yml
  format: yaml
  label: Monero Network API
  slug: monero-network-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monero/refs/heads/main/openapi/monero-network-api-openapi.yml
- filename: monero-node-info-api-openapi.yml
  format: yaml
  label: Monero Node Info API
  slug: monero-node-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monero/refs/heads/main/openapi/monero-node-info-api-openapi.yml
- filename: monero-outputs-api-openapi.yml
  format: yaml
  label: Monero Outputs API
  slug: monero-outputs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monero/refs/heads/main/openapi/monero-outputs-api-openapi.yml
- filename: monero-transaction-pool-api-openapi.yml
  format: yaml
  label: Monero Transaction Pool API
  slug: monero-transaction-pool-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monero/refs/heads/main/openapi/monero-transaction-pool-api-openapi.yml
- filename: monero-transactions-api-openapi.yml
  format: yaml
  label: Monero Transactions API
  slug: monero-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monero/refs/heads/main/openapi/monero-transactions-api-openapi.yml
consequence_counts:
  physical: 1
  read: 11
  safety-critical: 1
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Monero Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /stop_mining
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /send_raw_transaction
operation_count: 16
overview: 'Monero exposes 16 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 3 write, 1 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Monero
provider_slug: monero
slug: monero-agentic-access
source_filename: monero-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/monero-blockchain-api-openapi.yml, openapi/monero-json-rpc-api-openapi.yml,\n  openapi/monero-mining-api-openapi.yml, openapi/monero-network-api-openapi.yml, openapi/monero-node-info-api-openapi.yml,\n  openapi/monero-outputs-api-openapi.yml, openapi/monero-transaction-pool-api-openapi.yml, openapi/monero-transactions-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 11\n    acting: 5\n  by_consequence:\n    read: 11\n    write: 3\n    safety-critical: 1\n    physical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /get_alt_blocks_hashes\n  method: post\n  operationId: getAltBlocksHashes\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /json_rpc\n  method: post\n  operationId: jsonRpc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /start_mining\n  method: post\n  operationId: startMining\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stop_mining\n  method: post\n  operationId: stopMining\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /mining_status\n  method: post\n  operationId: miningStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get_net_stats\n  method: post\n  operationId: getNetStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get_limit\n  method: post\n  operationId: getLimit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get_peer_list\n  method: post\n  operationId: getPeerList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n \
  \   audit: none\n- path: /get_public_nodes\n  method: post\n  operationId: getPublicNodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get_height\n  method: post\n  operationId: getHeight\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get_outs\n  method: post\n  operationId: getOuts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get_transaction_pool\n  method: post\n  operationId: getTransactionPool\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get_transaction_pool_stats\n  method: post\n  operationId: getTransactionPoolStats\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get_transactions\n  method: post\n  operationId: getTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /is_key_image_spent\n  method: post\n  operationId: isKeyImageSpent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /send_raw_transaction\n  method: post\n  operationId: sendRawTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monero/refs/heads/main/agentic-access/monero-agentic-access.yml
summary_line: 16 operations · 5 acting · 1 human-in-the-loop
tags:
- Cryptocurrency
- Privacy
- Blockchain
- JSON-RPC
- Wallets
- Mining
- Transaction
---
