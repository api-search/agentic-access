---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 21
api_specs:
- filename: symbiotic-relay-openapi.json
  format: json
  label: Symbiotic Relay API
  slug: symbiotic-relay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symbiotic/refs/heads/main/openapi/symbiotic-relay-openapi.json
consequence_counts:
  read: 21
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Symbiotic Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 22
overview: 'Symbiotic exposes 22 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Symbiotic
provider_slug: symbiotic
slug: symbiotic-agentic-access
source_filename: symbiotic-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/symbiotic-relay-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 21\n    acting: 1\n  by_consequence:\n    read: 21\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/aggregation/proof/{requestId}\n  method: get\n  operationId: SymbioticAPIService_GetAggregationProof\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/aggregation/proofs/epoch/{epoch}\n  method: get\n  operationId: SymbioticAPIService_GetAggregationProofsByEpoch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/aggregation/status/{requestId}\n  method: get\n  operationId: SymbioticAPIService_GetAggregationStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/committed/all\n  method: get\n  operationId: SymbioticAPIService_GetLastAllCommitted\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/committed/chain/{settlementChainId}\n  method: get\n  operationId: SymbioticAPIService_GetLastCommitted\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/epoch/current\n  method: get\n  operationId: SymbioticAPIService_GetCurrentEpoch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n \
  \   subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sign\n  method: post\n  operationId: SymbioticAPIService_SignMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/signature-request-ids/epoch/{epoch}\n  method: get\n  operationId: SymbioticAPIService_GetSignatureRequestIDsByEpoch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/signature-request/{requestId}\n  method: get\n  operationId: SymbioticAPIService_GetSignatureRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/signature-requests/epoch/{epoch}\n\
  \  method: get\n  operationId: SymbioticAPIService_GetSignatureRequestsByEpoch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/signatures/epoch/{epoch}\n  method: get\n  operationId: SymbioticAPIService_GetSignaturesByEpoch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/signatures/{requestId}\n  method: get\n  operationId: SymbioticAPIService_GetSignatures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stream/proofs\n  method: get\n  operationId: SymbioticAPIService_ListenProofs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stream/signatures\n  method:\
  \ get\n  operationId: SymbioticAPIService_ListenSignatures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stream/validator-set\n  method: get\n  operationId: SymbioticAPIService_ListenValidatorSet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/validator-set\n  method: get\n  operationId: SymbioticAPIService_GetValidatorSet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/validator-set/custom-schedule/node-status\n  method: get\n  operationId: SymbioticAPIService_GetCustomScheduleNodeStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/validator-set/header\n\
  \  method: get\n  operationId: SymbioticAPIService_GetValidatorSetHeader\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/validator-set/metadata\n  method: get\n  operationId: SymbioticAPIService_GetValidatorSetMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/validator/address/{address}\n  method: get\n  operationId: SymbioticAPIService_GetValidatorByAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/validator/key/{keyTag}/{onChainKey}\n  method: get\n  operationId: SymbioticAPIService_GetValidatorByKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/validator/local\n  method: get\n  operationId: SymbioticAPIService_GetLocalValidator\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/symbiotic/refs/heads/main/agentic-access/symbiotic-agentic-access.yml
summary_line: 22 operations · 1 acting
tags:
- Company
- Crypto Defi
- Restaking
- Shared Security
- Staking
- Blockchain
- Web3
- Smart Contracts
- Ethereum
- DeFi
---
