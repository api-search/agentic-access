---
acting_count: 0
action_class_counts:
  connected: 5
api_specs:
- filename: waodao-artchain-api-openapi.yml
  format: yaml
  label: WAODAO Art Chain API
  slug: waodao-artchain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/waodao/refs/heads/main/openapi/waodao-artchain-api-openapi.yml
- filename: waodao-liquidity-pools-api-openapi.yml
  format: yaml
  label: WAODAO Liquidity Pools API
  slug: waodao-liquidity-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/waodao/refs/heads/main/openapi/waodao-liquidity-pools-api-openapi.yml
- filename: waodao-schema-api-openapi.yml
  format: yaml
  label: WAODAO Schema API
  slug: waodao-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/waodao/refs/heads/main/openapi/waodao-schema-api-openapi.yml
- filename: waodao-token-metadata-api-openapi.yml
  format: yaml
  label: WAODAO Token Metadata API
  slug: waodao-token-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/waodao/refs/heads/main/openapi/waodao-token-metadata-api-openapi.yml
consequence_counts:
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Waodao Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'WAODAO exposes 5 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: WAODAO
provider_slug: waodao
slug: waodao-agentic-access
source_filename: waodao-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: generated\nsource: openapi/waodao-agent-api-openapi-3.0.json, openapi/waodao-agent-api-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI.\n  A governance starting point for exposing this API to AI agents — review and bind audience per deployment.\n  See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 5\n  by_consequence:\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/waodao/index\n  method: get\n  operationId: listArtChainDays\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/waodao/latest\n  method: get\n  operationId: getLatestArtChainDay\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/v1/waodao/token/{day}\n  method: get\n  operationId: getArtChainDay\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/waodao/schema\n  method: get\n  operationId: getAgentApiSchema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/waodao/pools\n  method: get\n  operationId: listWaoLiquidityPools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\nnote: 'Deduplicated: the OpenAPI 3.1 contract and the 3.0.2 compatibility contract describe the same five\n  operations, so each operation is listed once.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/waodao/refs/heads/main/agentic-access/waodao-agentic-access.yml
summary_line: 5 operations
tags:
- AI Agents
- ArtChain
- Human and AI
- NFT Metadata
- On-chain Culture
- Liquidity Pools
- Web3
- OpenAPI
- Ethereum
- Solana
- agent-native
- Digital Art
---
