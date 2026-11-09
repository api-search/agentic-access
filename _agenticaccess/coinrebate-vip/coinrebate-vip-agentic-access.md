---
acting_count: 0
action_class_counts:
  connected: 8
api_specs:
- filename: coinrebate-vip-agent-route-api-openapi.yml
  format: yaml
  label: CoinRebate Agent Route API
  slug: coinrebate-vip-agent-route-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinrebate-vip/openapi/coinrebate-vip-agent-route-api-openapi.yml
- filename: coinrebate-vip-ai-stats-api-openapi.yml
  format: yaml
  label: CoinRebate Ai Stats API
  slug: coinrebate-vip-ai-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinrebate-vip/openapi/coinrebate-vip-ai-stats-api-openapi.yml
- filename: coinrebate-vip-guides-search-api-openapi.yml
  format: yaml
  label: CoinRebate Guides Search API
  slug: coinrebate-vip-guides-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinrebate-vip/openapi/coinrebate-vip-guides-search-api-openapi.yml
- filename: coinrebate-vip-health-api-openapi.yml
  format: yaml
  label: CoinRebate Health API
  slug: coinrebate-vip-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinrebate-vip/openapi/coinrebate-vip-health-api-openapi.yml
- filename: coinrebate-vip-link-evidence-api-openapi.yml
  format: yaml
  label: CoinRebate Link Evidence API
  slug: coinrebate-vip-link-evidence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinrebate-vip/openapi/coinrebate-vip-link-evidence-api-openapi.yml
- filename: coinrebate-vip-perp-stats-api-openapi.yml
  format: yaml
  label: CoinRebate Perp Stats API
  slug: coinrebate-vip-perp-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinrebate-vip/openapi/coinrebate-vip-perp-stats-api-openapi.yml
- filename: coinrebate-vip-referral-check-api-openapi.yml
  format: yaml
  label: CoinRebate Referral Check API
  slug: coinrebate-vip-referral-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinrebate-vip/openapi/coinrebate-vip-referral-check-api-openapi.yml
- filename: coinrebate-vip-tradfi-perps-api-openapi.yml
  format: yaml
  label: CoinRebate Tradfi Perps API
  slug: coinrebate-vip-tradfi-perps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinrebate-vip/openapi/coinrebate-vip-tradfi-perps-api-openapi.yml
consequence_counts:
  read: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Coinrebate Vip Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'CoinRebate exposes 8 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CoinRebate
provider_slug: coinrebate-vip
slug: coinrebate-vip-agentic-access
source_filename: coinrebate-vip-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/coinrebate-vip-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 8\n  by_consequence:\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v4/agent-route\n  method: get\n  operationId: getExchangeRoute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/ai-stats\n  method: get\n  operationId: getAiStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/health\n  method: get\n  operationId: healthCheck\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/tradfi-perps\n  method: get\n  operationId: listTradfiPerps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/perp-stats\n  method: get\n  operationId: getPerpStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/referral-check\n  method: get\n  operationId: checkReferralLink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/link-evidence\n  method: get\n  operationId: inspectExchangeLink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/v4/guides-search\n  method: get\n  operationId: searchGuides\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/coinrebate-vip/agentic-access/coinrebate-vip-agentic-access.yml
summary_line: 8 operations
tags:
- Cryptocurrency
- Finance
- Rebate
- Exchange
- Affiliates
---
