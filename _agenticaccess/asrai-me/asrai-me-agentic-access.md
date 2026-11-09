---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 42
api_specs:
- filename: asrai-me-ai-api-openapi.yml
  format: yaml
  label: Asrai AI API
  slug: asrai-me-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asrai-me/openapi/asrai-me-ai-api-openapi.yml
- filename: asrai-me-cashflow-api-openapi.yml
  format: yaml
  label: Asrai Cashflow API
  slug: asrai-me-cashflow-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asrai-me/openapi/asrai-me-cashflow-api-openapi.yml
- filename: asrai-me-market-data-api-openapi.yml
  format: yaml
  label: Asrai Market Data API
  slug: asrai-me-market-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asrai-me/openapi/asrai-me-market-data-api-openapi.yml
- filename: asrai-me-screeners-api-openapi.yml
  format: yaml
  label: Asrai Screeners API
  slug: asrai-me-screeners-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asrai-me/openapi/asrai-me-screeners-api-openapi.yml
- filename: asrai-me-technical-api-openapi.yml
  format: yaml
  label: Asrai Technical API
  slug: asrai-me-technical-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asrai-me/openapi/asrai-me-technical-api-openapi.yml
consequence_counts:
  read: 42
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Asrai Me Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 43
overview: 'Asrai exposes 43 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 42 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Asrai
provider_slug: asrai-me
slug: asrai-me-agentic-access
source_filename: asrai-me-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/asrai-me-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 43\n  by_action_class:\n    acting: 1\n    connected: 42\n  by_consequence:\n    write: 1\n    read: 42\n  human_in_the_loop_required: 0\noperations:\n- path: /ai\n  method: post\n  operationId: ask_ai\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/signal/{symbol}/{interval}\n  method: get\n  operationId: get_signal\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/alsat/{symbol}/{interval}\n  method: get\n  operationId: get_alsat\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/superalsat/{symbol}\n  method: get\n  operationId: get_superalsat\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/alphatrend/{symbol}/{interval}\n  method: get\n  operationId: get_alphatrend\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/td/{symbol}/{interval}\n  method: get\n  operationId: get_td\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/psar/{symbol}/{interval}\n  method: get\n  operationId: get_psar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/macd-dema/{symbol}/{interval}\n  method: get\n  operationId: get_macd_dema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ichimoku/{symbol}/{interval}\n  method: get\n  operationId: get_ichimoku\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ew/{symbol}/{interval}\n  method: get\n  operationId: get_elliott_wave\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/smartmoney/{symbol}/{interval}\n  method: get\n  operationId: get_smart_money\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/support-resistance/{symbol}/{interval}\n  method: get\n  operationId: get_support_resistance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/cashflow/market\n  method: get\n  operationId: get_cashflow_market\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/cashflow/coin/{symbol}\n  method: get\n  operationId: get_cashflow_coin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/cashflow/group/{symbols}\n  method: get\n  operationId: get_cashflow_group\n  x-agentic-access:\n    action-class: connected\n \
  \   consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/cmcai/\n  method: get\n  operationId: get_cmcai\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/cmcai/{symbol}\n  method: get\n  operationId: get_cmcai_symbol\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/coinstats/{symbol}\n  method: get\n  operationId: get_coinstats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/info/{symbol}\n  method: get\n  operationId: get_info\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/price/{symbol}\n  method:\
  \ get\n  operationId: get_price\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/dexscreener/{symbol}\n  method: get\n  operationId: get_dexscreener\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/dexscreener/{chain}/{address}\n  method: get\n  operationId: get_dexscreener_token\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/chain/{chain}/{max_mcap}\n  method: get\n  operationId: get_chain_tokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/portfolio/\n  method: get\n  operationId: get_portfolio\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ath/\n  method: get\n  operationId: get_ath\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rsi/\n  method: get\n  operationId: get_rsi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rsi-heatmap/\n  method: get\n  operationId: get_rsi_heatmap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/top-bottom/\n  method: get\n  operationId: get_top_bottom\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/galaxyscore/\n  method: get\n  operationId:\
  \ get_galaxyscore\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/socialdominance/\n  method: get\n  operationId: get_socialdominance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/highvolumelowcap/\n  method: get\n  operationId: get_highvolumelowcap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/bounce-dip/\n  method: get\n  operationId: get_bounce_dip\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/stronger-weaker-coins/\n  method: get\n  operationId: get_stronger_weaker_coins\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/sar-coins/\n  method: get\n  operationId: get_sar_coins\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/macd-coins/\n  method: get\n  operationId: get_macd_coins\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/techrating/\n  method: get\n  operationId: get_techrating\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/volume/\n  method: get\n  operationId: get_volume\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/vwap/\n  method: get\n  operationId: get_vwap\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/late-unlocked-coins/\n  method: get\n  operationId: get_late_unlocked\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/channel-summary/\n  method: get\n  operationId: get_channel_summary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/trending\n  method: get\n  operationId: get_trending\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gainers-losers\n  method: get\n  operationId: get_gainers_losers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/cbbi\n  method: get\n  operationId: get_cbbi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/asrai-me/agentic-access/asrai-me-agentic-access.yml
summary_line: 43 operations · 1 acting
tags:
- Cryptocurrency
- Artificial Intelligence
- Trading
- Signals
- Telegram
- Analytics
---
