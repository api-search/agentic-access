---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 15
api_specs:
- filename: asteroidxrpl-com-asset-api-openapi.yml
  format: yaml
  label: ASTEROID XRPL Asset API
  slug: asteroidxrpl-com-asset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asteroidxrpl-com/openapi/asteroidxrpl-com-asset-api-openapi.yml
- filename: asteroidxrpl-com-escrows-api-openapi.yml
  format: yaml
  label: ASTEROID XRPL Escrows API
  slug: asteroidxrpl-com-escrows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asteroidxrpl-com/openapi/asteroidxrpl-com-escrows-api-openapi.yml
- filename: asteroidxrpl-com-health-api-openapi.yml
  format: yaml
  label: ASTEROID XRPL Health API
  slug: asteroidxrpl-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asteroidxrpl-com/openapi/asteroidxrpl-com-health-api-openapi.yml
- filename: asteroidxrpl-com-holders-api-openapi.yml
  format: yaml
  label: ASTEROID XRPL Holders API
  slug: asteroidxrpl-com-holders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asteroidxrpl-com/openapi/asteroidxrpl-com-holders-api-openapi.yml
- filename: asteroidxrpl-com-liquidity-api-openapi.yml
  format: yaml
  label: ASTEROID XRPL Liquidity API
  slug: asteroidxrpl-com-liquidity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asteroidxrpl-com/openapi/asteroidxrpl-com-liquidity-api-openapi.yml
- filename: asteroidxrpl-com-llms-txt-api-openapi.yml
  format: yaml
  label: ASTEROID XRPL Llms.txt API
  slug: asteroidxrpl-com-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asteroidxrpl-com/openapi/asteroidxrpl-com-llms-txt-api-openapi.yml
- filename: asteroidxrpl-com-market-api-openapi.yml
  format: yaml
  label: ASTEROID XRPL Market API
  slug: asteroidxrpl-com-market-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asteroidxrpl-com/openapi/asteroidxrpl-com-market-api-openapi.yml
- filename: asteroidxrpl-com-quote-api-openapi.yml
  format: yaml
  label: ASTEROID XRPL Quote API
  slug: asteroidxrpl-com-quote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asteroidxrpl-com/openapi/asteroidxrpl-com-quote-api-openapi.yml
- filename: asteroidxrpl-com-schemas-api-openapi.yml
  format: yaml
  label: ASTEROID XRPL Schemas API
  slug: asteroidxrpl-com-schemas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asteroidxrpl-com/openapi/asteroidxrpl-com-schemas-api-openapi.yml
- filename: asteroidxrpl-com-supply-api-openapi.yml
  format: yaml
  label: ASTEROID XRPL Supply API
  slug: asteroidxrpl-com-supply-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asteroidxrpl-com/openapi/asteroidxrpl-com-supply-api-openapi.yml
- filename: asteroidxrpl-com-well-known-api-openapi.yml
  format: yaml
  label: ASTEROID XRPL .well Known API
  slug: asteroidxrpl-com-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asteroidxrpl-com/openapi/asteroidxrpl-com-well-known-api-openapi.yml
consequence_counts:
  read: 15
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Asteroidxrpl Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'ASTEROID XRPL exposes 16 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ASTEROID XRPL
provider_slug: asteroidxrpl-com
slug: asteroidxrpl-com-agentic-access
source_filename: asteroidxrpl-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/asteroidxrpl-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 15\n    acting: 1\n  by_consequence:\n    read: 15\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /.well-known/asteroid-agent.json\n  method: get\n  operationId: getDiscoveryManifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/xrpl-asset.json\n  method: get\n  operationId: getAssetManifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/v1/asset\n  method: get\n  operationId: getAssetIdentity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/asset/evidence\n  method: get\n  operationId: getAssetEvidence\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schemas/v1/index.json\n  method: get\n  operationId: getSchemaCatalogue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schemas/v1/{schema}.json\n  method: get\n  operationId: getSchema\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/market\n  method: get\n  operationId: getMarketState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/supply\n  method: get\n  operationId: getSupplyState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/liquidity\n  method: get\n  operationId: getLiquidityState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/liquidity/lock\n  method: get\n  operationId: verifyLiquidityLock\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/v1/escrows\n  method: get\n  operationId: getEscrowSchedule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/holders\n  method: get\n  operationId: getHolderDistribution\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/quote\n  method: get\n  operationId: getSwapQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/quote\n  method: post\n  operationId: postSwapQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /llms.txt\n  method: get\n  operationId: getLlmsTxt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/asteroidxrpl-com/agentic-access/asteroidxrpl-com-agentic-access.yml
summary_line: 16 operations · 1 acting
tags:
- Blockchain
- XRPL
- Tokens
- Community
- Meme
---
