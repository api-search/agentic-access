---
acting_count: 0
action_class_counts:
  connected: 15
api_specs:
- filename: united-states-department-of-agriculture-data-api-openapi.yml
  format: yaml
  label: United States Department of Agriculture Data API
  slug: united-states-department-of-agriculture-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-department-of-agriculture/refs/heads/main/openapi/united-states-department-of-agriculture-data-api-openapi.yml
- filename: united-states-department-of-agriculture-foods-api-openapi.yml
  format: yaml
  label: United States Department of Agriculture Foods API
  slug: united-states-department-of-agriculture-foods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-department-of-agriculture/refs/heads/main/openapi/united-states-department-of-agriculture-foods-api-openapi.yml
- filename: united-states-department-of-agriculture-forecasts-api-openapi.yml
  format: yaml
  label: United States Department of Agriculture Forecasts API
  slug: united-states-department-of-agriculture-forecasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-department-of-agriculture/refs/heads/main/openapi/united-states-department-of-agriculture-forecasts-api-openapi.yml
- filename: united-states-department-of-agriculture-metadata-api-openapi.yml
  format: yaml
  label: United States Department of Agriculture Metadata API
  slug: united-states-department-of-agriculture-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-department-of-agriculture/refs/heads/main/openapi/united-states-department-of-agriculture-metadata-api-openapi.yml
- filename: united-states-department-of-agriculture-nutrients-api-openapi.yml
  format: yaml
  label: United States Department of Agriculture Nutrients API
  slug: united-states-department-of-agriculture-nutrients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-department-of-agriculture/refs/heads/main/openapi/united-states-department-of-agriculture-nutrients-api-openapi.yml
- filename: united-states-department-of-agriculture-stations-api-openapi.yml
  format: yaml
  label: United States Department of Agriculture Stations API
  slug: united-states-department-of-agriculture-stations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-department-of-agriculture/refs/heads/main/openapi/united-states-department-of-agriculture-stations-api-openapi.yml
- filename: united-states-department-of-agriculture-statistics-api-openapi.yml
  format: yaml
  label: United States Department of Agriculture Statistics API
  slug: united-states-department-of-agriculture-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-department-of-agriculture/refs/heads/main/openapi/united-states-department-of-agriculture-statistics-api-openapi.yml
- filename: united-states-department-of-agriculture-survey-data-api-openapi.yml
  format: yaml
  label: United States Department of Agriculture Survey Data API
  slug: united-states-department-of-agriculture-survey-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-department-of-agriculture/refs/heads/main/openapi/united-states-department-of-agriculture-survey-data-api-openapi.yml
consequence_counts:
  read: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: United States Department Of Agriculture Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'United States Department of Agriculture exposes 15 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: United States Department of Agriculture
provider_slug: united-states-department-of-agriculture
slug: united-states-department-of-agriculture-agentic-access
source_filename: united-states-department-of-agriculture-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/usda-ers-arms-openapi.yml, openapi/usda-fooddata-central-openapi.yml, openapi/usda-nass-quickstats-openapi.yml,\n  openapi/usda-nrcs-awdb-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 15\n  by_consequence:\n    read: 15\n  human_in_the_loop_required: 0\noperations:\n- path: /year\n  method: get\n  operationId: getAvailableYears\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /state\n  method: get\n  operationId: getAvailableStates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /report\n  method: get\n  operationId: getAvailableReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /variable\n  method: get\n  operationId: getAvailableVariables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /surveydata\n  method: get\n  operationId: getSurveyData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /foods/search\n  method: get\n  operationId: searchFoods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /food/{fdcId}\n  method: get\n  operationId: getFoodById\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /foods\n  method: get\n  operationId: getFoodsByIds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nutrients\n  method: get\n  operationId: getNutrients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api_GET/\n  method: get\n  operationId: getAgriculturalStatistics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get_param_values/\n  method: get\n  operationId: getParameterValues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get_counts/\n  method:\
  \ get\n  operationId: getRecordCount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stations\n  method: get\n  operationId: getStations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data\n  method: get\n  operationId: getStationData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /forecasts\n  method: get\n  operationId: getWaterSupplyForecasts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/united-states-department-of-agriculture/refs/heads/main/agentic-access/united-states-department-of-agriculture-agentic-access.yml
summary_line: 15 operations
tags:
- Federal Government
- Agriculture
- Food Safety
- Nutrition
- Rural Development
- Climate
---
