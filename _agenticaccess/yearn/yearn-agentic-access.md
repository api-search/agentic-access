---
acting_count: 0
action_class_counts:
  connected: 9
api_specs:
- filename: docs
  format: yaml
  label: yDaemon REST API
  slug: ydaemon-rest-api
  spec_type: OpenAPI
  url: https://ydaemon.yearn.fi/docs
consequence_counts:
  read: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Yearn Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'Yearn Finance exposes 9 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Yearn Finance
provider_slug: yearn
slug: yearn-agentic-access
source_filename: yearn-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/ydaemon.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 9\n  by_consequence:\n    read: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /{chainID}/vaults/all\n  method: get\n  operationId: getAllVaults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{chainID}/vaults/{address}\n  method: get\n  operationId: getVaultByAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{chainID}/vaults/tvl\n  method: get\n  operationId:\
  \ getVaultsTVL\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{chainID}/vaults/v2\n  method: get\n  operationId: getV2Vaults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{chainID}/vaults/v3\n  method: get\n  operationId: getV3Vaults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{chainID}/vaults/retired\n  method: get\n  operationId: getRetiredVaults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{chainID}/vaults/detected\n  method: get\n  operationId: getDetectedVaults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /info/chains\n  method: get\n  operationId: getSupportedChains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /info/vaults/blacklisted\n  method: get\n  operationId: getBlacklistedVaults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yearn/refs/heads/main/agentic-access/yearn-agentic-access.yml
summary_line: 9 operations
tags:
- DeFi
- Yield Aggregator
- Vaults
- EVM
- Web3
- Blockchain
- Finance
---
