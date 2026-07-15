---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 26
api_specs:
- filename: pocket-network-path-gateway-api-openapi.yml
  format: yaml
  label: Pocket Network PATH Gateway API
  slug: pocket-network-path-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pocket-network/refs/heads/main/openapi/pocket-network-path-gateway-api-openapi.yml
- filename: pocket-network-shannon-rpc-api-openapi.yml
  format: yaml
  label: Pocket Network Shannon RPC API
  slug: pocket-network-shannon-rpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pocket-network/refs/heads/main/openapi/pocket-network-shannon-rpc-api-openapi.yml
- filename: pocket-network-cometbft-rpc-api-openapi.yml
  format: yaml
  label: Pocket Network CometBFT RPC API
  slug: pocket-network-cometbft-rpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pocket-network/refs/heads/main/openapi/pocket-network-cometbft-rpc-api-openapi.yml
consequence_counts:
  physical: 2
  read: 26
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Pocket Network Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/{appId}
operation_count: 29
overview: 'Pocket Network exposes 29 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 26 read, 1 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Pocket Network
provider_slug: pocket-network
slug: pocket-network-agentic-access
source_filename: pocket-network-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/pocket-network-cometbft-rpc-api-openapi.yml, openapi/pocket-network-path-gateway-api-openapi.yml,\n  openapi/pocket-network-shannon-rpc-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 29\n  by_action_class:\n    connected: 26\n    acting: 3\n  by_consequence:\n    read: 26\n    physical: 2\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /status\n  method: get\n  operationId: getCometbftStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /net_info\n  method: get\n  operationId: getCometbftNetInfo\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /block\n  method: get\n  operationId: getCometbftBlock\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /block_results\n  method: get\n  operationId: getCometbftBlockResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /commit\n  method: get\n  operationId: getCometbftCommit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tx\n  method: get\n  operationId: getCometbftTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /unconfirmed_txs\n  method: get\n \
  \ operationId: getCometbftUnconfirmedTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broadcast_tx_sync\n  method: get\n  operationId: broadcastCometbftTxSync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/{appId}\n  method: post\n  operationId: sendAuthenticatedRelay\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1\n  method: post\n  operationId: sendPublicRelay\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /healthz\n  method: get\n  operationId: getPathLiveness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /readyz\n  method: get\n  operationId: getPathReadiness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/base/tendermint/v1beta1/blocks/latest\n  method: get\n  operationId: getLatestShannonBlock\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/base/tendermint/v1beta1/blocks/{height}\n  method: get\n  operationId: getShannonBlockByHeight\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/tx/v1beta1/txs/{hash}\n  method: get\n  operationId: getShannonTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/tx/v1beta1/txs\n  method: post\n  operationId: broadcastShannonTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cosmos/bank/v1beta1/balances/{address}\n  method: get\n  operationId: getShannonBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /cosmos/bank/v1beta1/supply\n  method: get\n  operationId: getShannonTotalSupply\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/staking/v1beta1/validators\n  method: get\n  operationId: listShannonValidators\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pocket/application/v1/application\n  method: get\n  operationId: listShannonApplications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pocket/application/v1/application/{address}\n  method: get\n  operationId: getShannonApplication\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pocket/supplier/v1/supplier\n\
  \  method: get\n  operationId: listShannonSuppliers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pocket/supplier/v1/supplier/{address}\n  method: get\n  operationId: getShannonSupplier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pocket/gateway/v1/gateway\n  method: get\n  operationId: listShannonGateways\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pocket/service/v1/service\n  method: get\n  operationId: listShannonServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pocket/service/v1/service/{serviceId}\n  method: get\n  operationId: getShannonService\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pocket/session/v1/get_session\n  method: get\n  operationId: getShannonSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pocket/proof/v1/params\n  method: get\n  operationId: getShannonProofParameters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pocket/tokenomics/v1/params\n  method: get\n  operationId: getShannonTokenomicsParameters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pocket-network/refs/heads/main/agentic-access/pocket-network-agentic-access.yml
summary_line: 29 operations · 3 acting
tags:
- Web3
- Blockchain
- RPC
- Decentralized Infrastructure
- Pocket Network
- Grove
- PATH
- Shannon
- Cosmos
- POKT
---
