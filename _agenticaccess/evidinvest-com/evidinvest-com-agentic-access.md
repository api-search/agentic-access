---
acting_count: 52
action_class_counts:
  acting: 52
  connected: 8
api_specs:
- filename: evidinvest-com-calculations-api-openapi.yml
  format: yaml
  label: evidinvest-com Calculations API
  slug: evidinvest-com-calculations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evidinvest-com/openapi/evidinvest-com-calculations-api-openapi.yml
- filename: evidinvest-com-financial-data-api-openapi.yml
  format: yaml
  label: evidinvest-com Financial Data API
  slug: evidinvest-com-financial-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evidinvest-com/openapi/evidinvest-com-financial-data-api-openapi.yml
- filename: evidinvest-com-machine-payments-api-openapi.yml
  format: yaml
  label: evidinvest-com Machine Payments API
  slug: evidinvest-com-machine-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evidinvest-com/openapi/evidinvest-com-machine-payments-api-openapi.yml
- filename: evidinvest-com-market-data-api-openapi.yml
  format: yaml
  label: evidinvest-com Market Data API
  slug: evidinvest-com-market-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evidinvest-com/openapi/evidinvest-com-market-data-api-openapi.yml
- filename: evidinvest-com-portfolio-api-openapi.yml
  format: yaml
  label: evidinvest-com Portfolio API
  slug: evidinvest-com-portfolio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evidinvest-com/openapi/evidinvest-com-portfolio-api-openapi.yml
- filename: evidinvest-com-sec-filings-api-openapi.yml
  format: yaml
  label: evidinvest-com SEC Filings API
  slug: evidinvest-com-sec-filings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evidinvest-com/openapi/evidinvest-com-sec-filings-api-openapi.yml
- filename: evidinvest-com-user-lists-api-openapi.yml
  format: yaml
  label: evidinvest-com User Lists API
  slug: evidinvest-com-user-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evidinvest-com/openapi/evidinvest-com-user-lists-api-openapi.yml
- filename: evidinvest-com-valuation-api-openapi.yml
  format: yaml
  label: evidinvest-com Valuation API
  slug: evidinvest-com-valuation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evidinvest-com/openapi/evidinvest-com-valuation-api-openapi.yml
consequence_counts:
  physical: 8
  read: 8
  safety-critical: 3
  write: 41
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Evidinvest Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/paid/valuation
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/tools/calculate_margin_of_safety
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/tools/get_valuation_parameters
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/paid/company_snapshot
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/paid/filing_search
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/paid/supply_chain
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/paid/thesis_check
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/tools/calculate_ddm
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/tools/get_fair_value_range
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/tools/search_earnings_transcripts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/tools/search_sec_filings
operation_count: 60
overview: 'evidinvest-com exposes 60 API operations that an AI agent could call, of which 52 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 41 write, 8 physical, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: evidinvest-com
provider_slug: evidinvest-com
slug: evidinvest-com-agentic-access
source_filename: evidinvest-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/mcp_openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 60\n  by_action_class:\n    acting: 52\n    connected: 8\n  by_consequence:\n    physical: 8\n    write: 41\n    read: 8\n    safety-critical: 3\n  human_in_the_loop_required: 3\noperations:\n- path: /v1/tools/search_sec_filings\n  method: post\n  operationId: call_search_sec_filings\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /v1/tools/search_earnings_transcripts\n  method: post\n  operationId: call_search_earnings_transcripts\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/get_company_profile\n  method: post\n  operationId: call_get_company_profile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/get_income_statement\n  method: post\n  operationId: call_get_income_statement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/get_balance_sheet\n  method: post\n  operationId: call_get_balance_sheet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/get_cash_flow\n  method: post\n  operationId: call_get_cash_flow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/get_growth_rates\n  method: post\n  operationId: call_get_growth_rates\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/get_pe_ratios\n  method: post\n  operationId: call_get_pe_ratios\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/get_segment_revenue\n  method: post\n  operationId: call_get_segment_revenue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v1/tools/get_geographic_revenue\n  method: post\n  operationId: call_get_geographic_revenue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/get_major_customers\n  method: post\n  operationId: call_get_major_customers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/get_current_price\n  method: post\n  operationId: call_get_current_price\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/get_historical_prices\n  method: post\n  operationId: call_get_historical_prices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tools/get_enterprise_value\n  method: post\n  operationId: call_get_enterprise_value\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/get_company_peers\n  method: post\n  operationId: call_get_company_peers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tools/get_trading_multiples\n\
  \  method: post\n  operationId: call_get_trading_multiples\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tools/get_peer_multiples\n  method: post\n  operationId: call_get_peer_multiples\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tools/get_industry_multiples\n  method: post\n  operationId: call_get_industry_multiples\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/calculate_wacc\n  method: post\n  operationId: call_calculate_wacc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/calculate_dcf\n  method: post\n  operationId: call_calculate_dcf\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/calculate_margin_of_safety\n  method: post\n  operationId: call_calculate_margin_of_safety\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/tools/calculate_comparables\n\
  \  method: post\n  operationId: call_calculate_comparables\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/calculate_ddm\n  method: post\n  operationId: call_calculate_ddm\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/get_company_snapshot\n  method: post\n  operationId: call_get_company_snapshot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n  \
  \  escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/get_valuation_metric\n  method: post\n  operationId: call_get_valuation_metric\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/get_fair_value_range\n  method: post\n  operationId: call_get_fair_value_range\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/get_dcf_valuation\n  method: post\n  operationId:\
  \ call_get_dcf_valuation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/get_reverse_dcf\n  method: post\n  operationId: call_get_reverse_dcf\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/compare_stocks\n  method: post\n  operationId: call_compare_stocks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/tools/get_cagr_matrix\n  method: post\n  operationId: call_get_cagr_matrix\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/get_growth_trajectory\n  method: post\n  operationId: call_get_growth_trajectory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/list_user_stock_lists\n  method: post\n  operationId: call_list_user_stock_lists\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/create_user_stock_list\n  method: post\n  operationId: call_create_user_stock_list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/add_symbols_to_user_list\n  method: post\n  operationId: call_add_symbols_to_user_list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/remove_symbols_from_user_list\n  method: post\n  operationId: call_remove_symbols_from_user_list\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/set_user_list_watched\n  method: post\n  operationId: call_set_user_list_watched\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/delete_user_stock_list\n  method: post\n  operationId: call_delete_user_stock_list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /v1/tools/get_list_items\n  method: post\n  operationId: call_get_list_items\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tools/get_watchlist_status\n  method: post\n  operationId: call_get_watchlist_status\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/optimize_portfolio\n  method: post\n  operationId: call_optimize_portfolio\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v1/tools/portfolio_risk_decomposition\n  method: post\n  operationId: call_portfolio_risk_decomposition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/sec_get_profile\n  method: post\n  operationId: call_sec_get_profile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/sec_get_supply_chain\n  method: post\n  operationId: call_sec_get_supply_chain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/tools/sec_get_risks\n  method: post\n  operationId: call_sec_get_risks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/sec_find_chokepoints\n  method: post\n  operationId: call_sec_find_chokepoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tools/sec_search\n  method: post\n  operationId: call_sec_search\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/sec_compare\n\
  \  method: post\n  operationId: call_sec_compare\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/run_valuation\n  method: post\n  operationId: call_run_valuation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/get_implied_assumptions\n  method: post\n  operationId: call_get_implied_assumptions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/get_valuation_parameters\n  method: post\n  operationId: call_get_valuation_parameters\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/tools/save_valuation\n  method: post\n  operationId: call_save_valuation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/list_saved_valuations\n  method: post\n  operationId: call_list_saved_valuations\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/get_saved_valuation\n  method: post\n  operationId: call_get_saved_valuation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/delete_saved_valuation\n  method: post\n  operationId: call_delete_saved_valuation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/quote\n  method: get\n\
  \  operationId: get_price_quote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/paid/filing_search\n  method: post\n  operationId: paid_filing_search\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/paid/company_snapshot\n  method: post\n  operationId: paid_company_snapshot\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v1/paid/valuation\n  method: post\n  operationId: paid_valuation\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/paid/supply_chain\n  method: post\n  operationId: paid_supply_chain\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/paid/thesis_check\n  method: post\n  operationId: paid_thesis_check\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/evidinvest-com/agentic-access/evidinvest-com-agentic-access.yml
summary_line: 60 operations · 52 acting · 3 human-in-the-loop
tags:
- Company
- Finance
- Valuation
- Data
---
