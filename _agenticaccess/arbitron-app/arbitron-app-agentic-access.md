---
acting_count: 0
action_class_counts:
  connected: 20
api_specs:
- filename: arbitron-app-account-api-openapi.yml
  format: yaml
  label: Arbitron Account API
  slug: arbitron-app-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arbitron-app/openapi/arbitron-app-account-api-openapi.yml
- filename: arbitron-app-funding-api-openapi.yml
  format: yaml
  label: Arbitron Funding API
  slug: arbitron-app-funding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arbitron-app/openapi/arbitron-app-funding-api-openapi.yml
- filename: arbitron-app-platform-api-openapi.yml
  format: yaml
  label: Arbitron Platform API
  slug: arbitron-app-platform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arbitron-app/openapi/arbitron-app-platform-api-openapi.yml
- filename: arbitron-app-reference-data-api-openapi.yml
  format: yaml
  label: Arbitron Reference data API
  slug: arbitron-app-reference-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arbitron-app/openapi/arbitron-app-reference-data-api-openapi.yml
- filename: arbitron-app-spreads-api-openapi.yml
  format: yaml
  label: Arbitron Spreads API
  slug: arbitron-app-spreads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arbitron-app/openapi/arbitron-app-spreads-api-openapi.yml
consequence_counts:
  read: 20
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Arbitron App Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 20
overview: 'Arbitron exposes 20 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Arbitron
provider_slug: arbitron-app
slug: arbitron-app-agentic-access
source_filename: arbitron-app-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/arbitron-app-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    connected: 20\n  by_consequence:\n    read: 20\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1\n  method: get\n  operationId: discover\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/funding\n  method: get\n  operationId: listFunding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/funding/{coin}\n  method: get\n  operationId: getCoinFunding\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/funding/history\n  method: get\n  operationId: getFundingHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/spreads\n  method: get\n  operationId: listSpreads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/spreads/backtest\n  method: get\n  operationId: listSpreadBacktest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/exchanges\n  method: get\n  operationId: listExchanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/v1/coins\n  method: get\n  operationId: listCoins\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/listings\n  method: get\n  operationId: listListings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/usage\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/me\n  method: get\n  operationId: getMyAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/me/cards\n  method: get\n  operationId: listMyCards\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/me/cards/{card_ref}\n  method: get\n  operationId: getMyCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/me/trades\n  method: get\n  operationId: listMyTrades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/me/pnl\n  method: get\n  operationId: getMyPnl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/me/balances\n  method: get\n  operationId: getMyBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/me/balance-history\n\
  \  method: get\n  operationId: getMyBalanceHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/me/exchange-accounts\n  method: get\n  operationId: listMyExchangeAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/me/leaderboard\n  method: get\n  operationId: getMyLeaderboard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/me/subscription\n  method: get\n  operationId: getMySubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/arbitron-app/agentic-access/arbitron-app-agentic-access.yml
summary_line: 20 operations
tags:
- Cryptocurrency
- Arbitrage
- Finance
- Platform
---
