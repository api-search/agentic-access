---
acting_count: 0
action_class_counts:
  connected: 37
api_specs:
- filename: aikstockdata-data-api-openapi.yml
  format: yaml
  label: 한국주식데이터 (aikstockdata) Data API
  slug: aikstockdata-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aikstockdata/refs/heads/main/openapi/aikstockdata-data-api-openapi.yml
consequence_counts:
  read: 37
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Aikstockdata Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 37
overview: '한국주식데이터 (aikstockdata) exposes 37 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 37 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: 한국주식데이터 (aikstockdata)
provider_slug: aikstockdata
slug: aikstockdata-agentic-access
source_filename: aikstockdata-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: generated\nsource: openapi/aikstockdata-data-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 37\n  by_action_class:\n    connected: 37\n  by_consequence:\n    read: 37\n  human_in_the_loop_required: 0\noperations:\n- path: /data/public/dart_receipt_times.json\n  method: get\n  operationId: getDataPublicDartReceiptTimesJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/public/dart_receipt_times_min.json\n  method: get\n  operationId: getDataPublicDartReceiptTimesMinJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /data/public/disclosures.csv\n  method: get\n  operationId: getDataPublicDisclosuresCsv\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/public/disclosures_intraday.json\n  method: get\n  operationId: getDataPublicDisclosuresIntradayJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/public/disclosures_intraday_min.json\n  method: get\n  operationId: getDataPublicDisclosuresIntradayMinJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/public/earnings_calendar.json\n  method: get\n  operationId: getDataPublicEarningsCalendarJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/public/earnings_calendar_summary.json\n  method: get\n  operationId: getDataPublicEarningsCalendarSummaryJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/public/market_index_history.json\n  method: get\n  operationId: getDataPublicMarketIndexHistoryJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/public/new_since_yesterday.json\n  method: get\n  operationId: getDataPublicNewSinceYesterdayJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/public/press_owl_filings.csv\n  method: get\n  operationId: getDataPublicPressOwlFilingsCsv\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/public/press_turnaround.csv\n  method: get\n  operationId: getDataPublicPressTurnaroundCsv\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/public/quotes.csv\n  method: get\n  operationId: getDataPublicQuotesCsv\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/public/quotes_en.csv\n  method: get\n  operationId: getDataPublicQuotesEnCsv\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/public/quotes_min.json\n  method: get\n  operationId: getDataPublicQuotesMinJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/public/screen.json\n  method: get\n  operationId: getDataPublicScreenJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/public/screen_top300.json\n  method: get\n  operationId: getDataPublicScreenTop300Json\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/public/search_index.json\n  method: get\n  operationId: getDataPublicSearchIndexJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/public/search_index_aliases.json\n  method: get\n  operationId: getDataPublicSearchIndexAliasesJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/public/search_index_rows.json\n  method: get\n  operationId: getDataPublicSearchIndexRowsJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/public/index.json\n  method: get\n  operationId: getDataPublicIndexJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/public/today.json\n  method: get\n  operationId: getDataPublicTodayJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/public/s/{code}.json\n  method: get\n  operationId: getDataPublicS{code}Json\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /data/public/s/{code}_history.json\n  method: get\n  operationId: getDataPublicS{code}HistoryJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/public/quotes_top300.json\n  method: get\n  operationId: getDataPublicQuotesTop300Json\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/public/quotes_slim.json\n  method: get\n  operationId: getDataPublicQuotesSlimJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/public/quotes.json\n  method: get\n  operationId: getDataPublicQuotesJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/public/disclosures_top100.json\n\
  \  method: get\n  operationId: getDataPublicDisclosuresTop100Json\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/public/disclosures.json\n  method: get\n  operationId: getDataPublicDisclosuresJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/public/rankings.json\n  method: get\n  operationId: getDataPublicRankingsJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/public/earnings.json\n  method: get\n  operationId: getDataPublicEarningsJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/public/earnings_recent60.json\n  method: get\n  operationId:\
  \ getDataPublicEarningsRecent60Json\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/public/disclosure_impact.json\n  method: get\n  operationId: getDataPublicDisclosureImpactJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/public/disclosure_impact_summary.json\n  method: get\n  operationId: getDataPublicDisclosureImpactSummaryJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/public/search_index_min.json\n  method: get\n  operationId: getDataPublicSearchIndexMinJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/public/daily/today_{date}.json\n\
  \  method: get\n  operationId: getDataPublicDailyToday{date}Json\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/public/notices.json\n  method: get\n  operationId: getDataPublicNoticesJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/public/excluded.json\n  method: get\n  operationId: getDataPublicExcludedJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aikstockdata/refs/heads/main/agentic-access/aikstockdata-agentic-access.yml
summary_line: 37 operations
tags:
- South Korea
- Stock Market
- Financial Data
- Open Data
- Dart
- kospi
- kosdaq
- konex
- Filings
- Stocks
- MCP
- llms-txt
- OpenAPI
---
