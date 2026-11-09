---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 15
api_specs:
- filename: coingraph-ai-agents-api-openapi.yml
  format: yaml
  label: CoinGraph Agents API
  slug: coingraph-ai-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingraph-ai/openapi/coingraph-ai-agents-api-openapi.yml
- filename: coingraph-ai-decide-api-openapi.yml
  format: yaml
  label: CoinGraph Decide API
  slug: coingraph-ai-decide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingraph-ai/openapi/coingraph-ai-decide-api-openapi.yml
- filename: coingraph-ai-discover-api-openapi.yml
  format: yaml
  label: CoinGraph Discover API
  slug: coingraph-ai-discover-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingraph-ai/openapi/coingraph-ai-discover-api-openapi.yml
- filename: coingraph-ai-trust-api-openapi.yml
  format: yaml
  label: CoinGraph Trust API
  slug: coingraph-ai-trust-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingraph-ai/openapi/coingraph-ai-trust-api-openapi.yml
- filename: coingraph-ai-understand-api-openapi.yml
  format: yaml
  label: CoinGraph Understand API
  slug: coingraph-ai-understand-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingraph-ai/openapi/coingraph-ai-understand-api-openapi.yml
- filename: coingraph-ai-watch-api-openapi.yml
  format: yaml
  label: CoinGraph Watch API
  slug: coingraph-ai-watch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingraph-ai/openapi/coingraph-ai-watch-api-openapi.yml
consequence_counts:
  physical: 2
  read: 15
  safety-critical: 1
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Coingraph Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /monitor/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /agents/trade-gatekeeper
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /agents/wallet-guard
operation_count: 25
overview: 'CoinGraph exposes 25 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read, 7 write, 2 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CoinGraph
provider_slug: coingraph-ai
slug: coingraph-ai-agentic-access
source_filename: coingraph-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/coingraph-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 25\n  by_action_class:\n    connected: 15\n    acting: 10\n  by_consequence:\n    read: 15\n    write: 7\n    safety-critical: 1\n    physical: 2\n  human_in_the_loop_required: 1\noperations:\n- path: /tokens\n  method: get\n  operationId: tokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status\n  method: get\n  operationId: status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /state/{token}\n\
  \  method: get\n  operationId: state\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /history/{token}\n  method: get\n  operationId: history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /market\n  method: get\n  operationId: market\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inspect/{chain}/{address}\n  method: get\n  operationId: inspect\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /evaluate/{token}\n  method: get\n  operationId: evaluateGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n    \
  \  max-ttl: 3600\n    audit: none\n- path: /evaluate\n  method: post\n  operationId: evaluate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /explain/{token}\n  method: get\n  operationId: explainGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /explain/{token}/{id}\n  method: get\n  operationId: explainById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /explain\n  method: post\n  operationId: explain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ask\n  method: post\n  operationId: ask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /monitor\n  method: post\n  operationId: monitorCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /monitor\n  method: get\n  operationId: monitorList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n- path: /monitor/{id}\n  method: delete\n  operationId: monitorDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /record\n  method: get\n  operationId: record\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /record/{token}\n  method: get\n  operationId: recordToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /verify/{id}\n  method: get\n  operationId: verify\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /agents\n  method: get\n  operationId: agents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/{id}\n  method: get\n  operationId: agent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/trade-gatekeeper\n  method: post\n  operationId: run_trade_gatekeeper\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents/wallet-guard\n  method: post\n  operationId: run_wallet_guard\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n   \
  \ subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents/due-diligence-analyst\n  method: post\n  operationId: run_due_diligence_analyst\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents/portfolio-checkup\n  method: post\n  operationId: run_portfolio_checkup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /agents/daily-market-brief\n  method: post\n  operationId: run_daily_market_brief\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/coingraph-ai/agentic-access/coingraph-ai-agentic-access.yml
summary_line: 25 operations · 10 acting · 1 human-in-the-loop
tags:
- Crypto Data
- AI Agents
- trading agents
- Wallets
- On-Chain Data
- Market Data
---
