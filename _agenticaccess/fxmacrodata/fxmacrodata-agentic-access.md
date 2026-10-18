---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 36
api_specs:
- filename: fxmacrodata-announcements-api-openapi.yml
  format: yaml
  label: FXMacroData Announcements API
  slug: fxmacrodata-announcements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fxmacrodata/refs/heads/main/openapi/fxmacrodata-announcements-api-openapi.yml
- filename: fxmacrodata-calendar-api-openapi.yml
  format: yaml
  label: FXMacroData Calendar API
  slug: fxmacrodata-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fxmacrodata/refs/heads/main/openapi/fxmacrodata-calendar-api-openapi.yml
- filename: fxmacrodata-commodities-api-openapi.yml
  format: yaml
  label: FXMacroData Commodities API
  slug: fxmacrodata-commodities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fxmacrodata/refs/heads/main/openapi/fxmacrodata-commodities-api-openapi.yml
- filename: fxmacrodata-data-catalogue-api-openapi.yml
  format: yaml
  label: FXMacroData Data Catalogue API
  slug: fxmacrodata-data-catalogue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fxmacrodata/refs/heads/main/openapi/fxmacrodata-data-catalogue-api-openapi.yml
- filename: fxmacrodata-factors-api-openapi.yml
  format: yaml
  label: FXMacroData Factors API
  slug: fxmacrodata-factors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fxmacrodata/refs/heads/main/openapi/fxmacrodata-factors-api-openapi.yml
- filename: fxmacrodata-fx-markets-api-openapi.yml
  format: yaml
  label: FXMacroData Fx Markets API
  slug: fxmacrodata-fx-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fxmacrodata/refs/heads/main/openapi/fxmacrodata-fx-markets-api-openapi.yml
- filename: fxmacrodata-health-api-openapi.yml
  format: yaml
  label: FXMacroData Health API
  slug: fxmacrodata-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fxmacrodata/refs/heads/main/openapi/fxmacrodata-health-api-openapi.yml
- filename: fxmacrodata-monetary-policy-api-openapi.yml
  format: yaml
  label: FXMacroData Monetary Policy API
  slug: fxmacrodata-monetary-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fxmacrodata/refs/heads/main/openapi/fxmacrodata-monetary-policy-api-openapi.yml
- filename: fxmacrodata-predictions-api-openapi.yml
  format: yaml
  label: FXMacroData Predictions API
  slug: fxmacrodata-predictions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fxmacrodata/refs/heads/main/openapi/fxmacrodata-predictions-api-openapi.yml
- filename: fxmacrodata-press-releases-api-openapi.yml
  format: yaml
  label: FXMacroData Press Releases API
  slug: fxmacrodata-press-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fxmacrodata/refs/heads/main/openapi/fxmacrodata-press-releases-api-openapi.yml
- filename: fxmacrodata-settlement-api-openapi.yml
  format: yaml
  label: FXMacroData Settlement API
  slug: fxmacrodata-settlement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fxmacrodata/refs/heads/main/openapi/fxmacrodata-settlement-api-openapi.yml
consequence_counts:
  read: 36
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Fxmacrodata Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 37
overview: 'FXMacroData exposes 37 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 36 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: FXMacroData
provider_slug: fxmacrodata
slug: fxmacrodata-agentic-access
source_filename: fxmacrodata-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: generated\nsource: openapi/fxmacrodata-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 37\n  by_action_class:\n    connected: 36\n    acting: 1\n  by_consequence:\n    read: 36\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/health\n  method: get\n  operationId: ping_v1_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ping\n  method: get\n  operationId: ping_v1_ping_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/forex/{base}/{quote}\n  method:\
  \ get\n  operationId: forex_v1_forex__base___quote__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fx/reference-rates/{base}/{quote}\n  method: get\n  operationId: reference_rates_v1_fx_reference_rates__base___quote__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fx/intraday-reference-rates/{base}/{quote}\n  method: get\n  operationId: intraday_reference_rates_v1_fx_intraday_reference_rates__base___quote__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fx/session-rates/{base}/{quote}\n  method: get\n  operationId: session_rates_v1_fx_session_rates__base___quote__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fx/sources\n  method: get\n  operationId: fx_sources_v1_fx_sources_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fx/source-universe\n  method: get\n  operationId: fx_source_universe_v1_fx_source_universe_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/research/panel\n  method: post\n  operationId: research_panel_v1_research_panel_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/data_catalogue/{currency}\n  method: get\n  operationId: get_data_catalogue_v1_data_catalogue__currency__get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/calendar/{currency}\n  method: get\n  operationId: get_release_calendar_v1_calendar__currency__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/calendar/{currency}/snapshot\n  method: get\n  operationId: get_calendar_snapshot_v1_calendar__currency__snapshot_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/calendar/{currency}/events/{archive_event_id}/versions\n  method: get\n  operationId: get_calendar_versions_v1_calendar__currency__events__archive_event_id__versions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/calendar/{currency}/coverage\n  method: get\n  operationId: get_calendar_archive_coverage_v1_calendar__currency__coverage_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/market_sessions\n  method: get\n  operationId: get_market_sessions_v1_market_sessions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/rate_differentials/{base}/{quote}\n  method: get\n  operationId: get_rate_differentials_v1_rate_differentials__base___quote__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/curves/{currency}\n  method: get\n  operationId: get_curve_snapshot_v1_curves__currency__get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/financial_prices/{currency}\n  method: get\n  operationId: get_financial_prices_v1_financial_prices__currency__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/press-releases/{currency}\n  method: get\n  operationId: get_press_releases_v1_press_releases__currency__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/risk_sentiment/changes\n  method: get\n  operationId: get_risk_sentiment_changes_v1_risk_sentiment_changes_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/risk_sentiment\n  method: get\n  operationId: get_risk_sentiment_v1_risk_sentiment_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/factors/{currency}/{factor}\n  method: get\n  operationId: get_currency_factor_v1_factors__currency___factor__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/predictions/coverage\n  method: get\n  operationId: get_prediction_coverage_index_v1_predictions_coverage_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/predictions/coverage/{currency}\n  method: get\n  operationId: get_prediction_coverage_for_currency_v1_predictions_coverage__currency__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/predictions/{currency}\n\
  \  method: get\n  operationId: get_predictions_missing_indicator_v1_predictions__currency__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/predictions/{currency}/{indicator}\n  method: get\n  operationId: get_indicator_predictions_v1_predictions__currency___indicator__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/announcements/{currency}/latest\n  method: get\n  operationId: get_currency_latest_indicator_values_v1_announcements__currency__latest_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/announcements/{currency}/{indicator}\n  method: get\n  operationId: get_indicator_data_v1_announcements__currency___indicator__get\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cot/{currency}\n  method: get\n  operationId: get_cot_data_v1_cot__currency__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/commodities/latest\n  method: get\n  operationId: get_all_commodity_latest_values_v1_commodities_latest_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/commodities/{indicator}\n  method: get\n  operationId: get_commodity_indicator_data_v1_commodities__indicator__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/settlement/contracts\n  method: get\n  operationId: list_settlement_contracts_v1_settlement_contracts_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/settlement/keys\n  method: get\n  operationId: settlement_keys_v1_settlement_keys_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/settlement/contracts/{contract_id}\n  method: get\n  operationId: settle_contract_v1_settlement_contracts__contract_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/settlement/{currency}/{indicator}\n  method: get\n  operationId: settle_series_v1_settlement__currency___indicator__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/announcements/changes\n  method: get\n\
  \  operationId: get_announcement_changes_v1_announcements_changes_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stream/events\n  method: get\n  operationId: stream_events_v1_stream_events_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fxmacrodata/refs/heads/main/agentic-access/fxmacrodata-agentic-access.yml
summary_line: 37 operations · 1 acting
tags:
- Company
- Finance
- Data
- API
- FX
---
