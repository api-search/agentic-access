---
acting_count: 0
action_class_counts:
  connected: 4
api_specs:
- filename: degenhedge-com-fees-api-openapi.yml
  format: yaml
  label: DegenHedge Fees API
  slug: degenhedge-com-fees-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/degenhedge-com/openapi/degenhedge-com-fees-api-openapi.yml
- filename: degenhedge-com-market-data-api-openapi.yml
  format: yaml
  label: DegenHedge market data API
  slug: degenhedge-com-market-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/degenhedge-com/openapi/degenhedge-com-market-data-api-openapi.yml
- filename: degenhedge-com-record-api-openapi.yml
  format: yaml
  label: DegenHedge Record API
  slug: degenhedge-com-record-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/degenhedge-com/openapi/degenhedge-com-record-api-openapi.yml
consequence_counts:
  read: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Degenhedge Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 4
overview: 'DegenHedge exposes 4 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: DegenHedge
provider_slug: degenhedge-com
slug: degenhedge-com-agentic-access
source_filename: degenhedge-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/degenhedge-com-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    connected: 4\n  by_consequence:\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /api/btc-window\n  method: get\n  operationId: getBtcWindow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/record\n  method: get\n  operationId: getGradedRecord\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/kalshi-fee\n  method: get\n  operationId: getKalshiFee\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /results.csv\n  method: get\n  operationId: getResultsCsv\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/degenhedge-com/agentic-access/degenhedge-com-agentic-access.yml
summary_line: 4 operations
tags:
- Company
- Prediction Markets
- Kalshi
- Bitcoin
- Trading Signals
- Telegram
- Sports Betting
- MCP
- Market Data
---
