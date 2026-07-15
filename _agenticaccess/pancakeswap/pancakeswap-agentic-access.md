---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 9
api_specs:
- filename: openapi.yml
  format: yaml
  label: PancakeSwap Info API v2
  slug: pancakeswap-info-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pancakeswap/refs/heads/main/openapi/openapi.yml
- filename: profile-openapi.yml
  format: yaml
  label: PancakeSwap Profile API
  slug: pancakeswap-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pancakeswap/refs/heads/main/openapi/profile-openapi.yml
consequence_counts:
  read: 9
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Pancakeswap Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'PancakeSwap exposes 10 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: PancakeSwap
provider_slug: pancakeswap
slug: pancakeswap-agentic-access
source_filename: pancakeswap-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openapi.yml, openapi/profile-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 9\n    acting: 1\n  by_consequence:\n    read: 9\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/summary\n  method: get\n  operationId: getSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/tokens\n  method: get\n  operationId: getTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/tokens/{address}\n  method:\
  \ get\n  operationId: getToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/pairs\n  method: get\n  operationId: getPairs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /version\n  method: get\n  operationId: getVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{address}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/register\n  method: post\n  operationId: registerUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n   \
  \   max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/valid/{username}\n  method: get\n  operationId: validateUsername\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leaderboard/global\n  method: get\n  operationId: getGlobalLeaderboard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leaderboard/team/{id}\n  method: get\n  operationId: getTeamLeaderboard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pancakeswap/refs/heads/main/agentic-access/pancakeswap-agentic-access.yml
summary_line: 10 operations · 1 acting
tags:
- DeFi
- DEX
- BNB Chain
- Decentralized Exchange
- Blockchain
- Swap
- Liquidity
- Yield Farming
- NFT
- Web3
---
