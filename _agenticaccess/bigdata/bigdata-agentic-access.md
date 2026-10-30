---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 25
api_specs:
- filename: bigdata-analyst-estimates-api-openapi.yml
  format: yaml
  label: RavenPack Analyst Estimates API
  slug: bigdata-analyst-estimates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigdata/refs/heads/main/openapi/bigdata-analyst-estimates-api-openapi.yml
- filename: bigdata-company-events-api-openapi.yml
  format: yaml
  label: RavenPack Company & Events API
  slug: bigdata-company-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigdata/refs/heads/main/openapi/bigdata-company-events-api-openapi.yml
- filename: bigdata-financials-ratios-api-openapi.yml
  format: yaml
  label: RavenPack Financials & Ratios API
  slug: bigdata-financials-ratios-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigdata/refs/heads/main/openapi/bigdata-financials-ratios-api-openapi.yml
- filename: bigdata-fixed-income-api-openapi.yml
  format: yaml
  label: RavenPack Fixed Income API
  slug: bigdata-fixed-income-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigdata/refs/heads/main/openapi/bigdata-fixed-income-api-openapi.yml
- filename: bigdata-fund-holdings-api-openapi.yml
  format: yaml
  label: RavenPack Fund Holdings API
  slug: bigdata-fund-holdings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigdata/refs/heads/main/openapi/bigdata-fund-holdings-api-openapi.yml
- filename: bigdata-market-data-api-openapi.yml
  format: yaml
  label: RavenPack Market Data API
  slug: bigdata-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigdata/refs/heads/main/openapi/bigdata-market-data-api-openapi.yml
- filename: bigdata-private-markets-api-openapi.yml
  format: yaml
  label: RavenPack Private Markets API
  slug: bigdata-private-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigdata/refs/heads/main/openapi/bigdata-private-markets-api-openapi.yml
consequence_counts:
  read: 25
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bigdata Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 31
overview: 'RavenPack exposes 31 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 25 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: RavenPack
provider_slug: bigdata
slug: bigdata-agentic-access
source_filename: bigdata-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: generated\nsource: openapi/bigdata-structured_data.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 31\n  by_action_class:\n    connected: 25\n    acting: 6\n  by_consequence:\n    read: 25\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/price/daily/query\n  method: post\n  operationId: query_daily_prices_v1_price_daily_query_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/price/intraday/query\n  method: post\n  operationId: query_intraday_prices_v1_price_intraday_query_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/price/aftermarket/query\n  method: post\n  operationId: query_aftermarket_v1_price_aftermarket_query_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/dividends/query\n  method: post\n  operationId: query_dividends_v1_dividends_query_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/price/changes/query\n  method: post\n  operationId: query_price_changes_v1_price_changes_query_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/quote/query\n  method: post\n  operationId: query_company_quote_v1_quote_query_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/analyst-estimates/query\n  method: post\n  operationId: query_analyst_estimates_v1_analyst_estimates_query_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/analyst-ratings/query\n  method: post\n  operationId: query_analyst_ratings_v1_analyst_ratings_query_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/latest-surprise/query\n  method: post\n  operationId: query_latest_surprise_v1_latest_surprise_query_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/price/target/query\n  method: post\n  operationId: query_target_price_v1_target_price_query_post\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/balance-sheet/query\n  method: post\n  operationId: query_balance_sheet_v1_balance_sheet_query_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cash-flow-statement/query\n  method: post\n  operationId: query_cash_flow_statement_v1_cash_flow_statement_query_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/company-ratios-ttm/query\n  method: post\n  operationId: query_company_ratios_ttm_v1_company_ratios_ttm_query_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/income-statement/query\n  method: post\n  operationId: query_income_statement_v1_income_statement_query_post\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/key-metrics-ttm/query\n  method: post\n  operationId: query_key_metrics_TTM_v1_key_metrics_ttm_query_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/company-revenue-geographic-segments/query\n  method: post\n  operationId: query_company_revenue_geographic_v1_company_revenue_geographic_segments_query_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/company-revenue-product-segments/query\n  method: post\n  operationId: query_company_revenue_product_v1_company_revenue_product_segments_query_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n  \
  \    max-ttl: 3600\n    audit: none\n- path: /v1/company-profile/query\n  method: post\n  operationId: query_company_profile_v1_company_profile_query_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/company-screener/query\n  method: post\n  operationId: query_company_screener_v1_company_screener_query_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/events-calendar/query\n  method: post\n  operationId: query_events_calendar_v1_events_calendar_query_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/holdings/funds/stocks/\n  method: post\n  operationId: Holdings_v1_holdings_funds_stocks_post\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/holdings/stocks/funds\n  method: post\n  operationId: Stock_Funds_Holdings_v1_holdings_stocks_funds_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/holdings/funds/trends/\n  method: post\n  operationId: Fund_Position_Signals_v1_holdings_funds_trends__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/entity-sentiment/\n  method: post\n  operationId: query_entity_sentiment_v1_entity_sentiment__post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/esg-performance-score/query\n  method: post\n  operationId: query_esg_performance_score_v1_esg_performance_score__post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/economic-calendar/query\n  method: post\n  operationId: query_economic_calendar_v1_economic_calendar_query__post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/private-companies/query\n  method: post\n  operationId: Private_Company_Overview_v1_private_companies_query_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/funding-rounds/query\n  method: post\n  operationId: Private_Company_Funding_Rounds_v1_funding_rounds_query_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/fixed-income/corporate/issuer/query\n  method: post\n  operationId: query_bonds_by_issuer_v1_fixed_income_corporate_issuer_query__post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/private-company-people/query\n  method: post\n  operationId: Private_Company_People_v1_private_company_people_query_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/fixed-income/corporate/isin/query\n  method: post\n  operationId: query_bond_by_isin_v1_fixed_income_corporate_isin_query__post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bigdata/refs/heads/main/agentic-access/bigdata-agentic-access.yml
summary_line: 31 operations · 6 acting
tags:
- Company
- Finance
- Artificial Intelligence
- Data Analytics
- Market Insights
---
