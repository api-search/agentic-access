---
acting_count: 0
action_class_counts:
  connected: 6
api_specs:
- filename: backpow-com-coin-oracle-api-openapi.yml
  format: yaml
  label: BackPoW Coin Oracle API
  slug: backpow-com-coin-oracle-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backpow-com/openapi/backpow-com-coin-oracle-api-openapi.yml
- filename: backpow-com-coins-api-openapi.yml
  format: yaml
  label: BackPoW Coins API
  slug: backpow-com-coins-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backpow-com/openapi/backpow-com-coins-api-openapi.yml
- filename: backpow-com-cost-of-production-api-openapi.yml
  format: yaml
  label: BackPoW Cost Of Production API
  slug: backpow-com-cost-of-production-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backpow-com/openapi/backpow-com-cost-of-production-api-openapi.yml
- filename: backpow-com-hardware-api-openapi.yml
  format: yaml
  label: BackPoW Hardware API
  slug: backpow-com-hardware-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backpow-com/openapi/backpow-com-hardware-api-openapi.yml
- filename: backpow-com-news-api-openapi.yml
  format: yaml
  label: BackPoW News API
  slug: backpow-com-news-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backpow-com/openapi/backpow-com-news-api-openapi.yml
- filename: backpow-com-solo-mining-odds-api-openapi.yml
  format: yaml
  label: BackPoW Solo Mining Odds API
  slug: backpow-com-solo-mining-odds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backpow-com/openapi/backpow-com-solo-mining-odds-api-openapi.yml
consequence_counts:
  read: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Backpow Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'BackPoW exposes 6 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BackPoW
provider_slug: backpow-com
slug: backpow-com-agentic-access
source_filename: backpow-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/backpow-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 6\n  by_consequence:\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/solo-mining-odds\n  method: get\n  operationId: calculateSoloMiningOdds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cost-of-production\n  method: get\n  operationId: getCostOfProduction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/coin-oracle\n  method: get\n\
  \  operationId: getCoinOracle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/coins\n  method: get\n  operationId: listPowCoins\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/hardware\n  method: get\n  operationId: getHardwareBenchmarks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/news\n  method: get\n  operationId: getPowNews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/backpow-com/agentic-access/backpow-com-agentic-access.yml
summary_line: 6 operations
tags:
- Cryptocurrency
- Mining
- Proof of Work
- Data
---
