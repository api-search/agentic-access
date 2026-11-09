---
acting_count: 0
action_class_counts:
  connected: 44
api_specs:
- filename: xoomar-com-companies-api-openapi.yml
  format: yaml
  label: XOOMAR Companies API
  slug: xoomar-com-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xoomar-com/openapi/xoomar-com-companies-api-openapi.yml
- filename: xoomar-com-crypto-api-openapi.yml
  format: yaml
  label: XOOMAR Crypto API
  slug: xoomar-com-crypto-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xoomar-com/openapi/xoomar-com-crypto-api-openapi.yml
- filename: xoomar-com-macro-api-openapi.yml
  format: yaml
  label: XOOMAR Macro API
  slug: xoomar-com-macro-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xoomar-com/openapi/xoomar-com-macro-api-openapi.yml
consequence_counts:
  read: 44
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Xoomar Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 44
overview: 'XOOMAR exposes 44 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 44 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: XOOMAR
provider_slug: xoomar-com
slug: xoomar-com-agentic-access
source_filename: xoomar-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/xoomar-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 44\n  by_action_class:\n    connected: 44\n  by_consequence:\n    read: 44\n  human_in_the_loop_required: 0\noperations:\n- path: /api/markets/short-interest\n  method: get\n  operationId: short_interest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/markets/short-volume\n  method: get\n  operationId: short_volume\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/markets/fails-to-deliver\n  method:\
  \ get\n  operationId: fails_to_deliver\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/markets/threshold-list\n  method: get\n  operationId: threshold_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/markets/insiders\n  method: get\n  operationId: insiders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/markets/insiders/{ticker}\n  method: get\n  operationId: insiders_ticker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/markets/insiders/clusters\n  method: get\n  operationId: insiders_clusters\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/markets/planned-sales\n  method: get\n  operationId: planned_sales\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/markets/large-holders\n  method: get\n  operationId: large_holders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/markets/funds\n  method: get\n  operationId: funds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/markets/funds/{slug}\n  method: get\n  operationId: funds_slug\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/markets/financials\n\
  \  method: get\n  operationId: financials\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/markets/buybacks\n  method: get\n  operationId: buybacks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/markets/events\n  method: get\n  operationId: events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/markets/earnings\n  method: get\n  operationId: earnings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/markets/earnings/{ticker}\n  method: get\n  operationId: earnings_ticker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n   \
  \ subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/markets/structured-products\n  method: get\n  operationId: structured_products\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/markets/federal-contracts\n  method: get\n  operationId: federal_contracts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/markets/startup-funding\n  method: get\n  operationId: startup_funding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/markets/ipos\n  method: get\n  operationId: ipos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/markets/bitcoin-treasuries\n\
  \  method: get\n  operationId: bitcoin_treasuries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/markets/funding-rates\n  method: get\n  operationId: funding_rates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/markets/funding-rates/{slug}\n  method: get\n  operationId: funding_rates_slug\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/markets/open-interest/{slug}\n  method: get\n  operationId: open_interest_slug\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/markets/liquidations\n  method: get\n  operationId: liquidations\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/markets/liquidations/recent\n  method: get\n  operationId: liquidations_recent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/markets/liquidations/history\n  method: get\n  operationId: liquidations_history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/markets/options/{currency}\n  method: get\n  operationId: options_currency\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/markets/options/{currency}/dvol\n  method: get\n  operationId: options_currency_dvol\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/markets/whales\n  method: get\n  operationId: whales\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/markets/whales/{coin}\n  method: get\n  operationId: whales_coin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/markets/sentiment\n  method: get\n  operationId: sentiment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/markets/sentiment/{slug}\n  method: get\n  operationId: sentiment_slug\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/markets/signals/{slug}\n\
  \  method: get\n  operationId: signals_slug\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/markets/etf-flows\n  method: get\n  operationId: etf_flows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/markets/symbols\n  method: get\n  operationId: symbols\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/markets/cot\n  method: get\n  operationId: cot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/markets/cot/{slug}\n  method: get\n  operationId: cot_slug\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/markets/macro\n  method: get\n  operationId: macro\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/markets/fed-liquidity\n  method: get\n  operationId: fed_liquidity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/markets/treasury-auctions\n  method: get\n  operationId: treasury_auctions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/markets/rates\n  method: get\n  operationId: rates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/markets/rates/{country}\n  method: get\n  operationId:\
  \ rates_country\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/markets/calendar\n  method: get\n  operationId: calendar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/xoomar-com/agentic-access/xoomar-com-agentic-access.yml
summary_line: 44 operations
tags:
- Capital Markets
- Data
- Financial Services
- Software
---
