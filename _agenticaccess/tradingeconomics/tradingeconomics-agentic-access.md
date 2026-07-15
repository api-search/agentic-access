---
acting_count: 0
action_class_counts:
  connected: 30
api_specs:
- filename: tradingeconomics-openapi.yml
  format: yaml
  label: Trading Economics Indicators API
  slug: tradingeconomics-indicators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradingeconomics/refs/heads/main/openapi/tradingeconomics-openapi.yml
- filename: tradingeconomics-openapi.yml
  format: yaml
  label: Trading Economics Economic Calendar API
  slug: tradingeconomics-economic-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradingeconomics/refs/heads/main/openapi/tradingeconomics-openapi.yml
- filename: tradingeconomics-openapi.yml
  format: yaml
  label: Trading Economics Markets API
  slug: tradingeconomics-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradingeconomics/refs/heads/main/openapi/tradingeconomics-openapi.yml
- filename: tradingeconomics-openapi.yml
  format: yaml
  label: Trading Economics Forecasts API
  slug: tradingeconomics-forecasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradingeconomics/refs/heads/main/openapi/tradingeconomics-openapi.yml
- filename: tradingeconomics-openapi.yml
  format: yaml
  label: Trading Economics Historical API
  slug: tradingeconomics-historical-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradingeconomics/refs/heads/main/openapi/tradingeconomics-openapi.yml
- filename: tradingeconomics-openapi.yml
  format: yaml
  label: Trading Economics Financials API
  slug: tradingeconomics-financials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradingeconomics/refs/heads/main/openapi/tradingeconomics-openapi.yml
- filename: tradingeconomics-asyncapi.yml
  format: yaml
  label: Trading Economics Streaming API
  slug: tradingeconomics-streaming-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradingeconomics/refs/heads/main/asyncapi/tradingeconomics-asyncapi.yml
consequence_counts:
  read: 30
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tradingeconomics Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 30
overview: 'Trading Economics exposes 30 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 30 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Trading Economics
provider_slug: tradingeconomics
slug: tradingeconomics-agentic-access
source_filename: tradingeconomics-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/tradingeconomics-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 30\n  by_action_class:\n    connected: 30\n  by_consequence:\n    read: 30\n  human_in_the_loop_required: 0\noperations:\n- path: /country/{country}\n  method: get\n  operationId: getIndicatorsByCountry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /country/all/{indicator}\n  method: get\n  operationId: getCountriesByIndicator\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /country/ticker/{ticker}\n\
  \  method: get\n  operationId: getIndicatorByTicker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /credit-ratings\n  method: get\n  operationId: getCreditRatings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /credit-ratings/country/{country}\n  method: get\n  operationId: getCreditRatingsByCountry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calendar\n  method: get\n  operationId: getCalendar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calendar/country/{countries}/{startDate}/{endDate}\n  method: get\n  operationId: getCalendarByCountryAndDate\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calendar/events/country/{countries}\n  method: get\n  operationId: getCalendarEventsByCountry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calendar/calendarid/{ids}\n  method: get\n  operationId: getCalendarEventsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calendar/updates\n  method: get\n  operationId: getCalendarUpdates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/commodities\n  method: get\n  operationId: getMarketsCommodities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/currency\n  method: get\n  operationId: getMarketsCurrencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/index\n  method: get\n  operationId: getMarketsIndexes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/crypto\n  method: get\n  operationId: getMarketsCrypto\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/bond\n  method: get\n  operationId: getMarketsBonds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/symbol/{symbols}\n  method: get\n  operationId:\
  \ getMarketsBySymbol\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/historical/{symbols}\n  method: get\n  operationId: getMarketsHistorical\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/intraday/{symbols}\n  method: get\n  operationId: getMarketsIntraday\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/search/{term}\n  method: get\n  operationId: searchMarkets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /forecast/country/{countries}\n  method: get\n  operationId: getForecastsByCountry\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /forecast/indicator/{indicators}\n  method: get\n  operationId: getForecastsByIndicator\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /forecast/country/{countries}/indicator/{indicators}\n  method: get\n  operationId: getForecastsByCountryAndIndicator\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /forecast/ticker/{tickers}\n  method: get\n  operationId: getForecastsByTicker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /historical/country/{countries}/indicator/{indicators}\n  method: get\n  operationId: getHistoricalByCountryAndIndicator\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /historical/country/{countries}/indicator/{indicators}/{startDate}/{endDate}\n  method: get\n  operationId: getHistoricalByCountryIndicatorAndDates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /historical/ticker/{ticker}/{startDate}\n  method: get\n  operationId: getHistoricalByTicker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /historical/latest\n  method: get\n  operationId: getHistoricalLatest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /historical/updates\n  method: get\n  operationId: getHistoricalUpdates\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /financials/category/{category}\n  method: get\n  operationId: getFinancialsByCategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /financials/symbol/{symbol}\n  method: get\n  operationId: getFinancialsBySymbol\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tradingeconomics/refs/heads/main/agentic-access/tradingeconomics-agentic-access.yml
summary_line: 30 operations
tags:
- Economic Indicators
- Interest Rates
- Macroeconomics
- Financial Data
- Economic Calendar
- Forecasts
- Markets
---
