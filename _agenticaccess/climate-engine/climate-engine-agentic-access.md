---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 10
api_specs:
- filename: climate-engine-openapi.yml
  format: yaml
  label: Climate Engine Timeseries API
  slug: climate-engine-timeseries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climate-engine/refs/heads/main/openapi/climate-engine-openapi.yml
- filename: climate-engine-openapi.yml
  format: yaml
  label: Climate Engine Zonal Statistics API
  slug: climate-engine-zonal-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climate-engine/refs/heads/main/openapi/climate-engine-openapi.yml
- filename: climate-engine-openapi.yml
  format: yaml
  label: Climate Engine Raster API
  slug: climate-engine-raster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climate-engine/refs/heads/main/openapi/climate-engine-openapi.yml
- filename: climate-engine-openapi.yml
  format: yaml
  label: Climate Engine Reports API
  slug: climate-engine-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climate-engine/refs/heads/main/openapi/climate-engine-openapi.yml
- filename: climate-engine-openapi.yml
  format: yaml
  label: Climate Engine Dataset Catalog API
  slug: climate-engine-dataset-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climate-engine/refs/heads/main/openapi/climate-engine-openapi.yml
- filename: climate-engine-openapi.yml
  format: yaml
  label: Climate Engine Account API
  slug: climate-engine-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climate-engine/refs/heads/main/openapi/climate-engine-openapi.yml
consequence_counts:
  read: 10
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Climate Engine Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 23
overview: 'Climate Engine exposes 23 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 13 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Climate Engine
provider_slug: climate-engine
slug: climate-engine-agentic-access
source_filename: climate-engine-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/climate-engine-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 10\n    acting: 13\n  by_consequence:\n    read: 10\n    write: 13\n  human_in_the_loop_required: 0\noperations:\n- path: /home/validate_key\n  method: get\n  operationId: validateKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /home/key_expiration\n  method: get\n  operationId: keyExpiration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /home/user/quotas\n\
  \  method: get\n  operationId: userQuotas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metadata/dataset_dates\n  method: get\n  operationId: metadataDatasetDates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metadata/dataset_variables\n  method: get\n  operationId: metadataDatasetVariables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metadata/county_names\n  method: get\n  operationId: metadataCountyNames\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /timeseries/native/coordinates\n  method: post\n  operationId: timeseriesNativeCoordinates\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /timeseries/native/feature_collection\n  method: post\n  operationId: timeseriesNativeFeatureCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /timeseries/native/forecasts/coordinates\n  method: post\n  operationId: timeseriesNativeForecastCoordinates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /timeseries/interannual/coordinates\n  method: post\n  operationId: timeseriesInterannualCoordinates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /timeseries/regression/coordinates\n  method: post\n  operationId: timeseriesRegressionCoordinates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /timeseries/standard_index/coordinates\n  method: post\n  operationId: timeseriesStandardIndexCoordinates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /zonal_stats/static_dataset/coordinates\n  method: post\n  operationId: zonalStatsStaticDatasetCoordinates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /zonal_stats/pixel_count/coordinates\n  method: post\n  operationId: zonalStatsPixelCountCoordinates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /zonal_stats/group_by/feature_collection\n\
  \  method: post\n  operationId: zonalStatsGroupByFeatureCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /zonal_stats/temporal_dataset/coordinates\n  method: get\n  operationId: zonalStatsTemporalDatasetCoordinates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /raster/mapid/values\n  method: get\n  operationId: rasterMapidValues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /raster/export/values\n  method: post\n  operationId: rasterExportValues\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /raster/export/task_update\n  method: get\n  operationId: rasterExportTaskUpdate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /raster/export/task_queue\n  method: get\n  operationId: rasterExportTaskQueue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/drought/coordinates\n  method: post\n  operationId: reportsDroughtCoordinates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n  \
  \    - high-value\n    audit: required\n- path: /reports/vegetation_production/coordinates\n  method: post\n  operationId: reportsVegetationProductionCoordinates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reports/site_characterization/coordinates\n  method: post\n  operationId: reportsSiteCharacterizationCoordinates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/climate-engine/refs/heads/main/agentic-access/climate-engine-agentic-access.yml
summary_line: 23 operations · 13 acting
tags:
- Climate
- Geospatial
- Remote Sensing
- Satellite
- Earth Observation
---
