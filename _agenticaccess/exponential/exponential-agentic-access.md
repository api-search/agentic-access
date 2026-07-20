---
acting_count: 0
action_class_counts:
  connected: 12
api_specs:
- filename: exponential-protocol-openapi.yml
  format: yaml
  label: YO Protocol API
  slug: yo-protocol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exponential/refs/heads/main/openapi/exponential-protocol-openapi.yml
- filename: exponential-risk-graph-openapi.yml
  format: yaml
  label: YO Risk Graph API
  slug: yo-risk-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exponential/refs/heads/main/openapi/exponential-risk-graph-openapi.yml
consequence_counts:
  read: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Exponential Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Exponential exposes 12 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Exponential
provider_slug: exponential
slug: exponential-agentic-access
source_filename: exponential-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/exponential-protocol-openapi.yml, openapi/exponential-risk-graph-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 12\n  by_consequence:\n    read: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/vault/{network}/{vaultAddress}\n  method: get\n  operationId: VaultController_getVault_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/vault/pending-redeems/{network}/{vaultAddress}\n  method: get\n  operationId: VaultController_getTotalPendingRedeems_v1\n  x-agentic-access:\n    action-class: connected\n   \
  \ consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/vault/yield/timeseries/{network}/{vaultAddress}\n  method: get\n  operationId: VaultController_getYieldTimeseries_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/vault/tvl/timeseries/{network}/{vaultAddress}\n  method: get\n  operationId: VaultController_getTvlTimeseries_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/history/user/{network}/{vaultAddress}/{userAddress}\n  method: get\n  operationId: HistoryController_getAggregatedHistory_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/vault/pending-redeems/{network}/{vaultAddress}/{userAddress}\n\
  \  method: get\n  operationId: VaultController_getPendingRedeemsForUser_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/performance/user/{network}/{vaultAddress}/{userAddress}\n  method: get\n  operationId: PerformanceController_getUserPerformance_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/public/vault/{chain}/{vaultAddress}/exposure\n  method: get\n  operationId: getVaultExposure\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agent/schema\n  method: get\n  operationId: agentSchema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agent/search\n\
  \  method: get\n  operationId: agentSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agent/node/{nodeId}\n  method: get\n  operationId: agentNode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agent/dependencies\n  method: get\n  operationId: agentDependencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exponential/refs/heads/main/agentic-access/exponential-agentic-access.yml
summary_line: 12 operations
tags:
- Company
- DeFi
- Decentralized Finance
- Yield
- Yield Optimizer
- Vaults
- ERC-4626
- Cross-chain
- Blockchain
- Crypto
- Risk
- Risk Ratings
- Agents
- x402
- Web3
---
