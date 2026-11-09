---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 55
api_specs:
- filename: apexvol-com-account-and-index-api-openapi.yml
  format: yaml
  label: ApexVol Account and index API
  slug: apexvol-com-account-and-index-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apexvol-com/openapi/apexvol-com-account-and-index-api-openapi.yml
- filename: apexvol-com-earnings-and-expected-move-api-openapi.yml
  format: yaml
  label: ApexVol Earnings and expected move API
  slug: apexvol-com-earnings-and-expected-move-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apexvol-com/openapi/apexvol-com-earnings-and-expected-move-api-openapi.yml
- filename: apexvol-com-events-and-calendars-api-openapi.yml
  format: yaml
  label: ApexVol Events and calendars API
  slug: apexvol-com-events-and-calendars-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apexvol-com/openapi/apexvol-com-events-and-calendars-api-openapi.yml
- filename: apexvol-com-gamma-exposure-api-openapi.yml
  format: yaml
  label: ApexVol Gamma exposure API
  slug: apexvol-com-gamma-exposure-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apexvol-com/openapi/apexvol-com-gamma-exposure-api-openapi.yml
- filename: apexvol-com-implied-volatility-api-openapi.yml
  format: yaml
  label: ApexVol Implied volatility API
  slug: apexvol-com-implied-volatility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apexvol-com/openapi/apexvol-com-implied-volatility-api-openapi.yml
- filename: apexvol-com-options-chain-api-openapi.yml
  format: yaml
  label: ApexVol Options chain API
  slug: apexvol-com-options-chain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apexvol-com/openapi/apexvol-com-options-chain-api-openapi.yml
- filename: apexvol-com-options-flow-api-openapi.yml
  format: yaml
  label: ApexVol Options flow API
  slug: apexvol-com-options-flow-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apexvol-com/openapi/apexvol-com-options-flow-api-openapi.yml
- filename: apexvol-com-options-greeks-api-openapi.yml
  format: yaml
  label: ApexVol Options Greeks API
  slug: apexvol-com-options-greeks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apexvol-com/openapi/apexvol-com-options-greeks-api-openapi.yml
- filename: apexvol-com-portfolio-risk-api-openapi.yml
  format: yaml
  label: ApexVol Portfolio risk API
  slug: apexvol-com-portfolio-risk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apexvol-com/openapi/apexvol-com-portfolio-risk-api-openapi.yml
- filename: apexvol-com-screeners-api-openapi.yml
  format: yaml
  label: ApexVol Screeners API
  slug: apexvol-com-screeners-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apexvol-com/openapi/apexvol-com-screeners-api-openapi.yml
- filename: apexvol-com-stock-analytics-api-openapi.yml
  format: yaml
  label: ApexVol Stock analytics API
  slug: apexvol-com-stock-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apexvol-com/openapi/apexvol-com-stock-analytics-api-openapi.yml
- filename: apexvol-com-strategies-api-openapi.yml
  format: yaml
  label: ApexVol Strategies API
  slug: apexvol-com-strategies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apexvol-com/openapi/apexvol-com-strategies-api-openapi.yml
consequence_counts:
  read: 55
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Apexvol Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 64
overview: 'ApexVol exposes 64 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 55 read and 9 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ApexVol
provider_slug: apexvol-com
slug: apexvol-com-agentic-access
source_filename: apexvol-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/apexvol-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 64\n  by_action_class:\n    connected: 55\n    acting: 9\n  by_consequence:\n    read: 55\n    write: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /api/mcp/data/\n  method: get\n  operationId: get_root\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/analyze-strategy\n  method: post\n  operationId: post_analyze_strategy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/data/batch/expected-move\n  method: get\n  operationId: get_batch_expected_move\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/batch/gex\n  method: get\n  operationId: get_batch_gex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/batch/iv-rank\n  method: get\n  operationId: get_batch_iv_rank\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/borrow-rate/{ticker}\n  method: get\n  operationId: get_borrow_rate_by_ticker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/build-strategy\n  method: post\n  operationId: post_build_strategy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/data/chain-at-time/{ticker}\n  method: get\n  operationId: get_chain_at_time_by_ticker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/chain/{ticker}\n  method: get\n  operationId: get_chain_by_ticker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/charm/{ticker}\n  method: get\n  operationId: get_charm_by_ticker\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/cores/{ticker}\n  method: get\n  operationId: get_cores_by_ticker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/correlation/{ticker}\n  method: get\n  operationId: get_correlation_by_ticker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/correlation/{ticker}/compare/<ticker2>\n  method: get\n  operationId: get_correlation_by_ticker_compare_ticker2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/cross-index-gex\n  method: get\n  operationId: get_cross_index_gex\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/dividend/{ticker}\n  method: get\n  operationId: get_dividend_by_ticker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/earnings-calendar\n  method: get\n  operationId: get_earnings_calendar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/earnings-history/{ticker}\n  method: get\n  operationId: get_earnings_history_by_ticker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/earnings-verdict/{ticker}\n  method: get\n  operationId: get_earnings_verdict_by_ticker\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/economic-calendar\n  method: get\n  operationId: get_economic_calendar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/expected-move/{ticker}\n  method: get\n  operationId: get_expected_move_by_ticker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/expected-vs-actual/{ticker}\n  method: get\n  operationId: get_expected_vs_actual_by_ticker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/expirations/{ticker}\n  method: get\n  operationId: get_expirations_by_ticker\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/flow/{ticker}\n  method: get\n  operationId: get_flow_by_ticker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/gex/{ticker}\n  method: get\n  operationId: get_gex_by_ticker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/greeks-exposure/{ticker}\n  method: get\n  operationId: get_greeks_exposure_by_ticker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/greeks-heatmap/{ticker}\n  method: get\n  operationId: get_greeks_heatmap_by_ticker\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/hedge-recommendations\n  method: post\n  operationId: post_hedge_recommendations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/data/historical-moves/{ticker}\n  method: get\n  operationId: get_historical_moves_by_ticker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/hv-regimes/{ticker}\n  method: get\n  operationId: get_hv_regimes_by_ticker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/iv-crush/{ticker}\n\
  \  method: get\n  operationId: get_iv_crush_by_ticker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/iv-opportunities/{ticker}\n  method: get\n  operationId: get_iv_opportunities_by_ticker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/iv-rank/{ticker}\n  method: get\n  operationId: get_iv_rank_by_ticker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/market-overview\n  method: get\n  operationId: get_market_overview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/max-pain/{ticker}\n  method: get\n  operationId:\
  \ get_max_pain_by_ticker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/me/usage\n  method: get\n  operationId: get_me_usage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/mispricing-assessment/{ticker}\n  method: get\n  operationId: get_mispricing_assessment_by_ticker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/monies/{ticker}\n  method: get\n  operationId: get_monies_by_ticker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/optimize-strategy\n  method: post\n  operationId: post_optimize_strategy\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/data/options-by-delta/{ticker}\n  method: get\n  operationId: get_options_by_delta_by_ticker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/pop\n  method: post\n  operationId: post_pop\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/data/portfolio-greeks\n  method: post\n  operationId: post_portfolio_greeks\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/data/post-earnings-drift/{ticker}\n  method: get\n  operationId: get_post_earnings_drift_by_ticker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/price-context/{ticker}\n  method: get\n  operationId: get_price_context_by_ticker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/relative-value-scan\n  method: get\n  operationId: get_relative_value_scan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/relative-value/{ticker}\n\
  \  method: get\n  operationId: get_relative_value_by_ticker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/scenario-analysis\n  method: post\n  operationId: post_scenario_analysis\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/data/screen\n  method: get\n  operationId: get_screen\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/search\n  method: get\n  operationId: get_search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /api/mcp/data/seasonality/{ticker}\n  method: get\n  operationId: get_seasonality_by_ticker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/simulate-chain\n  method: post\n  operationId: post_simulate_chain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/data/skew/{ticker}\n  method: get\n  operationId: get_skew_by_ticker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/smart-money/{ticker}\n  method: get\n  operationId: get_smart_money_by_ticker\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/stock/{ticker}\n  method: get\n  operationId: get_stock_by_ticker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/stress-tests\n  method: post\n  operationId: post_stress_tests\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/data/term-structure/{ticker}\n  method: get\n  operationId: get_term_structure_by_ticker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/third-order-greeks/{ticker}\n\
  \  method: get\n  operationId: get_third_order_greeks_by_ticker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/vix\n  method: get\n  operationId: get_vix\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/vol-arb-scan\n  method: get\n  operationId: get_vol_arb_scan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/volatility-cone/{ticker}\n  method: get\n  operationId: get_volatility_cone_by_ticker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/volume-profile/{ticker}\n  method: get\n  operationId: get_volume_profile_by_ticker\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/vrp/{ticker}\n  method: get\n  operationId: get_vrp_by_ticker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/vrp/{ticker}/expirations\n  method: get\n  operationId: get_vrp_by_ticker_expirations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/vrp/{ticker}/timeseries\n  method: get\n  operationId: get_vrp_by_ticker_timeseries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/data/zero-dte/{ticker}\n  method: get\n  operationId: get_zero_dte_by_ticker\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/apexvol-com/agentic-access/apexvol-com-agentic-access.yml
summary_line: 64 operations · 9 acting
tags:
- Options
- Analytics
- Trading
- Finance
- Terminal
---
