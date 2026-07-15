---
acting_count: 0
action_class_counts:
  connected: 11
api_specs:
- filename: mobula-openapi.yml
  format: yaml
  label: Mobula Market Data API
  slug: mobula-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mobula/refs/heads/main/openapi/mobula-openapi.yml
- filename: mobula-openapi.yml
  format: yaml
  label: Mobula Multi-Data API
  slug: mobula-multi-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mobula/refs/heads/main/openapi/mobula-openapi.yml
- filename: mobula-openapi.yml
  format: yaml
  label: Mobula Market History API
  slug: mobula-market-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mobula/refs/heads/main/openapi/mobula-openapi.yml
- filename: mobula-openapi.yml
  format: yaml
  label: Mobula Pairs and OHLCV API
  slug: mobula-pairs-ohlcv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mobula/refs/heads/main/openapi/mobula-openapi.yml
- filename: mobula-openapi.yml
  format: yaml
  label: Mobula Metadata API
  slug: mobula-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mobula/refs/heads/main/openapi/mobula-openapi.yml
- filename: mobula-openapi.yml
  format: yaml
  label: Mobula Wallet Portfolio API
  slug: mobula-wallet-portfolio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mobula/refs/heads/main/openapi/mobula-openapi.yml
- filename: mobula-openapi.yml
  format: yaml
  label: Mobula Wallet History and Transactions API
  slug: mobula-wallet-history-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mobula/refs/heads/main/openapi/mobula-openapi.yml
- filename: mobula-openapi.yml
  format: yaml
  label: Mobula Search and Query API
  slug: mobula-search-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mobula/refs/heads/main/openapi/mobula-openapi.yml
- filename: mobula-openapi.yml
  format: yaml
  label: Mobula Realtime Feed API
  slug: mobula-realtime-feed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mobula/refs/heads/main/openapi/mobula-openapi.yml
consequence_counts:
  read: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Mobula Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'Mobula exposes 11 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Mobula
provider_slug: mobula
slug: mobula-agentic-access
source_filename: mobula-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/mobula-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 11\n  by_consequence:\n    read: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /market/data\n  method: get\n  operationId: getMarketData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /market/multi-data\n  method: get\n  operationId: getMarketMultiData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /market/history\n  method: get\n  operationId: getMarketHistory\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /market/pairs\n  method: get\n  operationId: getMarketPairs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /market/pair\n  method: get\n  operationId: getMarketPairOhlcv\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metadata\n  method: get\n  operationId: getMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wallet/portfolio\n  method: get\n  operationId: getWalletPortfolio\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /wallet/history\n  method: get\n  operationId: getWalletHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wallet/transactions\n  method: get\n  operationId: getWalletTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search\n  method: get\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /market/query\n  method: get\n  operationId: marketQuery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mobula/refs/heads/main/agentic-access/mobula-agentic-access.yml
summary_line: 11 operations
tags:
- Crypto
- Web3
- Market Data
- Blockchain
- Wallet
- Real Time
---
