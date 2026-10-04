---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 41
api_specs:
- filename: solana-accounts-api-openapi.yml
  format: yaml
  label: Solana Accounts API
  slug: solana-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solana/refs/heads/main/openapi/solana-accounts-api-openapi.yml
- filename: solana-blocks-api-openapi.yml
  format: yaml
  label: Solana Blocks API
  slug: solana-blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solana/refs/heads/main/openapi/solana-blocks-api-openapi.yml
- filename: solana-cluster-api-openapi.yml
  format: yaml
  label: Solana Cluster API
  slug: solana-cluster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solana/refs/heads/main/openapi/solana-cluster-api-openapi.yml
- filename: solana-economics-api-openapi.yml
  format: yaml
  label: Solana Economics API
  slug: solana-economics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solana/refs/heads/main/openapi/solana-economics-api-openapi.yml
- filename: solana-tokens-api-openapi.yml
  format: yaml
  label: Solana Tokens API
  slug: solana-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solana/refs/heads/main/openapi/solana-tokens-api-openapi.yml
- filename: solana-transactions-api-openapi.yml
  format: yaml
  label: Solana Transactions API
  slug: solana-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solana/refs/heads/main/openapi/solana-transactions-api-openapi.yml
consequence_counts:
  physical: 1
  read: 41
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Solana Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sendTransaction
operation_count: 52
overview: 'Solana exposes 52 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 41 read, 10 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Solana
provider_slug: solana
slug: solana-agentic-access
source_filename: solana-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/solana-accounts-api-openapi.yml, openapi/solana-blocks-api-openapi.yml, openapi/solana-cluster-api-openapi.yml,\n  openapi/solana-economics-api-openapi.yml, openapi/solana-tokens-api-openapi.yml, openapi/solana-transactions-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 52\n  by_action_class:\n    connected: 41\n    acting: 11\n  by_consequence:\n    read: 41\n    write: 10\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: post\n  operationId: getAccountInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getBalance\n  method:\
  \ post\n  operationId: getBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getLargestAccounts\n  method: post\n  operationId: getLargestAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getMinimumBalanceForRentExemption\n  method: post\n  operationId: getMinimumBalanceForRentExemption\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getMultipleAccounts\n  method: post\n  operationId: getMultipleAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getProgramAccounts\n  method: post\n  operationId: getProgramAccounts\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getBlock\n  method: post\n  operationId: getBlock\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getBlockCommitment\n  method: post\n  operationId: getBlockCommitment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getBlockHeight\n  method: post\n  operationId: getBlockHeight\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getBlockProduction\n  method: post\n  operationId: getBlockProduction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getBlocks\n\
  \  method: post\n  operationId: getBlocks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getBlocksWithLimit\n  method: post\n  operationId: getBlocksWithLimit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getBlockTime\n  method: post\n  operationId: getBlockTime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getFirstAvailableBlock\n  method: post\n  operationId: getFirstAvailableBlock\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getRecentPerformanceSamples\n  method: post\n  operationId: getRecentPerformanceSamples\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /minimumLedgerSlot\n  method: post\n  operationId: minimumLedgerSlot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getClusterNodes\n  method: post\n  operationId: getClusterNodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getEpochInfo\n  method: post\n  operationId: getEpochInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getEpochSchedule\n  method: post\n  operationId: getEpochSchedule\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getGenesisHash\n  method: post\n  operationId: getGenesisHash\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getHealth\n  method: post\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getHighestSnapshotSlot\n  method: post\n  operationId: getHighestSnapshotSlot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getIdentity\n  method: post\n  operationId: getIdentity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getLeaderSchedule\n\
  \  method: post\n  operationId: getLeaderSchedule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getMaxRetransmitSlot\n  method: post\n  operationId: getMaxRetransmitSlot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getMaxShredInsertSlot\n  method: post\n  operationId: getMaxShredInsertSlot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getSlot\n  method: post\n  operationId: getSlot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /getSlotLeader\n  method: post\n  operationId: getSlotLeader\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getSlotLeaders\n  method: post\n  operationId: getSlotLeaders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getVersion\n  method: post\n  operationId: getVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getVoteAccounts\n  method: post\n  operationId: getVoteAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getInflationGovernor\n  method: post\n  operationId: getInflationGovernor\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getInflationRate\n  method: post\n  operationId: getInflationRate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getInflationReward\n  method: post\n  operationId: getInflationReward\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getStakeMinimumDelegation\n  method: post\n  operationId: getStakeMinimumDelegation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getSupply\n  method: post\n  operationId: getSupply\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getTokenAccountBalance\n\
  \  method: post\n  operationId: getTokenAccountBalance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getTokenAccountsByDelegate\n  method: post\n  operationId: getTokenAccountsByDelegate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getTokenAccountsByOwner\n  method: post\n  operationId: getTokenAccountsByOwner\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n  \
  \    triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getTokenLargestAccounts\n  method: post\n  operationId: getTokenLargestAccounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getTokenSupply\n  method: post\n  operationId: getTokenSupply\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sendTransaction\n  method: post\n  operationId: sendTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n     \
  \ max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /simulateTransaction\n  method: post\n  operationId: simulateTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getTransaction\n  method: post\n  operationId: getTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getSignaturesForAddress\n  method: post\n  operationId: getSignaturesForAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /getSignatureStatuses\n  method: post\n  operationId: getSignatureStatuses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getFeeForMessage\n  method: post\n  operationId: getFeeForMessage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getLatestBlockhash\n  method: post\n  operationId: getLatestBlockhash\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /isBlockhashValid\n  method: post\n  operationId: isBlockhashValid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n \
  \     - high-value\n    audit: required\n- path: /getRecentPrioritizationFees\n  method: post\n  operationId: getRecentPrioritizationFees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getTransactionCount\n  method: post\n  operationId: getTransactionCount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /requestAirdrop\n  method: post\n  operationId: requestAirdrop\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solana/refs/heads/main/agentic-access/solana-agentic-access.yml
summary_line: 52 operations · 11 acting
tags:
- Solana
- Blockchain
- Cryptocurrency
- Web3
- DeFi
- Transaction
- Tokens
---
