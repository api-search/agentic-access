---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 7
api_specs:
- filename: atlasyield-club-basket-api-openapi.yml
  format: yaml
  label: AtlasYield Basket API
  slug: atlasyield-club-basket-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/atlasyield-club/openapi/atlasyield-club-basket-api-openapi.yml
- filename: atlasyield-club-catalog-api-openapi.yml
  format: yaml
  label: AtlasYield Catalog API
  slug: atlasyield-club-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/atlasyield-club/openapi/atlasyield-club-catalog-api-openapi.yml
- filename: atlasyield-club-gas-api-openapi.yml
  format: yaml
  label: AtlasYield Gas API
  slug: atlasyield-club-gas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/atlasyield-club/openapi/atlasyield-club-gas-api-openapi.yml
- filename: atlasyield-club-portfolio-api-openapi.yml
  format: yaml
  label: AtlasYield Portfolio API
  slug: atlasyield-club-portfolio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/atlasyield-club/openapi/atlasyield-club-portfolio-api-openapi.yml
- filename: atlasyield-club-scores-api-openapi.yml
  format: yaml
  label: AtlasYield Scores API
  slug: atlasyield-club-scores-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/atlasyield-club/openapi/atlasyield-club-scores-api-openapi.yml
- filename: atlasyield-club-vaults-api-openapi.yml
  format: yaml
  label: AtlasYield Vaults API
  slug: atlasyield-club-vaults-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/atlasyield-club/openapi/atlasyield-club-vaults-api-openapi.yml
consequence_counts:
  read: 7
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Atlasyield Club Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'AtlasYield exposes 8 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AtlasYield
provider_slug: atlasyield-club
slug: atlasyield-club-agentic-access
source_filename: atlasyield-club-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/atlasyield-club-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 7\n    acting: 1\n  by_consequence:\n    read: 7\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /scores\n  method: get\n  operationId: getScores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog\n  method: get\n  operationId: getCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portfolio\n  method: get\n  operationId: getPortfolio\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /basket\n  method: post\n  operationId: scoreBasket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vaults/{chainId}/{address}/factors\n  method: get\n  operationId: getVaultFactors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vaults/{chainId}/{address}/metrics\n  method: get\n  operationId: getVaultMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vaults/{chainId}/{address}/route\n\
  \  method: get\n  operationId: getVaultRoute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gas\n  method: get\n  operationId: getGasRegime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/atlasyield-club/agentic-access/atlasyield-club-agentic-access.yml
summary_line: 8 operations · 1 acting
tags:
- DeFi
- Yield
- Risk Management
- Analytics
- Onchain
---
