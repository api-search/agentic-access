---
acting_count: 0
action_class_counts:
  connected: 17
api_specs:
- filename: energy-charts-api-openapi.yml
  format: yaml
  label: Energy Charts API
  slug: energy-charts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-charts-api/refs/heads/main/openapi/energy-charts-api-openapi.yml
consequence_counts:
  read: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Energy Charts Api Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'Energy Charts API exposes 17 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Energy Charts API
provider_slug: energy-charts-api
slug: energy-charts-api-agentic-access
source_filename: energy-charts-api-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/energy-charts-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    connected: 17\n  by_consequence:\n    read: 17\n  human_in_the_loop_required: 0\noperations:\n- path: /public_power\n  method: get\n  operationId: public_power_public_power_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public_power_forecast\n  method: get\n  operationId: public_power_forecast_public_power_forecast_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /total_power\n  method: get\n  operationId: total_power_total_power_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /installed_power\n  method: get\n  operationId: installed_power_installed_power_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /price\n  method: get\n  operationId: day_ahead_price_price_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cbet\n  method: get\n  operationId: cross_border_electricity_trading_cbet_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cbpf\n  method: get\n  operationId: cross_border_physical_flows_cbpf_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /signal\n  method: get\n  operationId: traffic_signal_signal_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ren_share_forecast\n  method: get\n  operationId: renewable_share_forecast_ren_share_forecast_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ren_share_daily_avg\n  method: get\n  operationId: ren_share_daily_avg_ren_share_daily_avg_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /solar_share\n  method: get\n  operationId: solar_share_solar_share_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /solar_share_daily_avg\n  method: get\n  operationId: solar_share_daily_avg_solar_share_daily_avg_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wind_onshore_share\n  method: get\n  operationId: wind_onshore_share_wind_onshore_share_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wind_onshore_share_daily_avg\n  method: get\n  operationId: wind_onshore_share_daily_avg_wind_onshore_share_daily_avg_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wind_offshore_share\n  method: get\n  operationId: wind_offshore_share_wind_offshore_share_get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wind_offshore_share_daily_avg\n  method: get\n  operationId: wind_offshore_share_daily_avg_wind_offshore_share_daily_avg_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /frequency\n  method: get\n  operationId: frequency_frequency_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/energy-charts-api/refs/heads/main/agentic-access/energy-charts-api-agentic-access.yml
summary_line: 17 operations
tags:
- Energy
- Electricity
- Renewables
- Grid
- Europe
- Power
- Pricing
- Forecasts
---
