---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 21
api_specs:
- filename: solcast-openapi.yml
  format: yaml
  label: Solcast API
  slug: solcast
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solcast/refs/heads/main/openapi/solcast-openapi.yml
consequence_counts:
  read: 21
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Solcast Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 25
overview: 'Solcast exposes 25 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Solcast
provider_slug: solcast
slug: solcast-agentic-access
source_filename: solcast-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/solcast-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 25\n  by_action_class:\n    connected: 21\n    acting: 4\n  by_consequence:\n    read: 21\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /data/live/radiation_and_weather\n  method: get\n  operationId: getLiveRadiationAndWeather\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/live/rooftop_pv_power\n  method: get\n  operationId: getLiveRooftopPvPower\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /data/live/advanced_pv_power\n  method: get\n  operationId: getLiveAdvancedPvPower\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/live/soiling/kimber\n  method: get\n  operationId: getLiveSoilingKimber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/live/soiling/hsu\n  method: get\n  operationId: getLiveSoilingHsu\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/forecast/radiation_and_weather\n  method: get\n  operationId: getForecastRadiationAndWeather\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/forecast/rooftop_pv_power\n\
  \  method: get\n  operationId: getForecastRooftopPvPower\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/forecast/advanced_pv_power\n  method: get\n  operationId: getForecastAdvancedPvPower\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/forecast/soiling/kimber\n  method: get\n  operationId: getForecastSoilingKimber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/forecast/soiling/hsu\n  method: get\n  operationId: getForecastSoilingHsu\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/forecast/aggregations\n  method: get\n  operationId: getForecastAggregations\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/historic/radiation_and_weather\n  method: get\n  operationId: getHistoricRadiationAndWeather\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/historic/rooftop_pv_power\n  method: get\n  operationId: getHistoricRooftopPvPower\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/historic/advanced_pv_power\n  method: get\n  operationId: getHistoricAdvancedPvPower\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/historic/soiling/kimber\n  method: get\n  operationId: getHistoricSoilingKimber\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/historic/soiling/hsu\n  method: get\n  operationId: getHistoricSoilingHsu\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/tmy/radiation_and_weather\n  method: get\n  operationId: getTmyRadiationAndWeather\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/tmy/rooftop_pv_power\n  method: get\n  operationId: getTmyRooftopPvPower\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/live/aggregations\n  method: get\n  operationId: getLiveAggregations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n   \
  \ subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resources/pv_power_sites\n  method: get\n  operationId: listPvPowerSites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resources/pv_power_site\n  method: get\n  operationId: getPvPowerSite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resources/pv_power_site\n  method: post\n  operationId: createPvPowerSite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /resources/pv_power_site\n  method: patch\n  operationId: patchPvPowerSite\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /resources/pv_power_site\n  method: put\n  operationId: updatePvPowerSite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /resources/pv_power_site\n  method: delete\n  operationId: deletePvPowerSite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solcast/refs/heads/main/agentic-access/solcast-agentic-access.yml
summary_line: 25 operations · 4 acting
tags:
- Solar
- Energy
- Forecasting
- Irradiance
- Weather
- Renewable Energy
- PV Power
---
