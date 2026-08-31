---
acting_count: 0
action_class_counts:
  connected: 9
api_specs:
- filename: rugspull-read-api-indexer-api-openapi.yml
  format: yaml
  label: Rugspull Read API Indexer API
  slug: rugspull-read-api-indexer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rugspull-read-api/refs/heads/main/openapi/rugspull-read-api-indexer-api-openapi.yml
- filename: rugspull-read-api-market-api-openapi.yml
  format: yaml
  label: Rugspull Read API Market API
  slug: rugspull-read-api-market-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rugspull-read-api/refs/heads/main/openapi/rugspull-read-api-market-api-openapi.yml
- filename: rugspull-read-api-objects-api-openapi.yml
  format: yaml
  label: Rugspull Read API Objects API
  slug: rugspull-read-api-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rugspull-read-api/refs/heads/main/openapi/rugspull-read-api-objects-api-openapi.yml
- filename: rugspull-read-api-rugs-api-openapi.yml
  format: yaml
  label: Rugspull Read API Rugs API
  slug: rugspull-read-api-rugs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rugspull-read-api/refs/heads/main/openapi/rugspull-read-api-rugs-api-openapi.yml
- filename: rugspull-read-api-service-api-openapi.yml
  format: yaml
  label: Rugspull Read API Service API
  slug: rugspull-read-api-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rugspull-read-api/refs/heads/main/openapi/rugspull-read-api-service-api-openapi.yml
consequence_counts:
  read: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Rugspull Read Api Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'Rugspull Read API exposes 9 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Rugspull Read API
provider_slug: rugspull-read-api
slug: rugspull-read-api-agentic-access
source_filename: rugspull-read-api-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: generated\nsource: openapi/rugspull-read-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 9\n  by_consequence:\n    read: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /api/health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/config\n  method: get\n  operationId: getConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/indexer/status\n  method: get\n  operationId: getIndexerStatus\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rugs\n  method: get\n  operationId: listRugs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rugs/{chainId}/{rug}\n  method: get\n  operationId: getRug\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rugs/{chainId}/{rug}/events\n  method: get\n  operationId: listRugEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rugs/{chainId}/{rug}/market\n  method: get\n  operationId: getRugMarket\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /api/market/sparklines\n  method: get\n  operationId: listMarketSparklines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/r2/{key}\n  method: get\n  operationId: getPublicObject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rugspull-read-api/refs/heads/main/agentic-access/rugspull-read-api-agentic-access.yml
summary_line: 9 operations
tags:
- bnb-smart-chain
- bsc
- wbnb
- Read Only
- OpenAPI
- high-risk
- discovery-cache
- DeFi
- Web3
- crypto-market-data
- indexer
---
