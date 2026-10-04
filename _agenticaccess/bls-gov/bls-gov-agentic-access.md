---
acting_count: 0
action_class_counts:
  connected: 5
api_specs:
- filename: bls-gov-popular-series-api-openapi.yml
  format: yaml
  label: Bureau of Labor Statistics Popular Series API
  slug: bls-gov-popular-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bls-gov/refs/heads/main/openapi/bls-gov-popular-series-api-openapi.yml
- filename: bls-gov-surveys-api-openapi.yml
  format: yaml
  label: Bureau of Labor Statistics Surveys API
  slug: bls-gov-surveys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bls-gov/refs/heads/main/openapi/bls-gov-surveys-api-openapi.yml
- filename: bls-gov-time-series-api-openapi.yml
  format: yaml
  label: Bureau of Labor Statistics Time Series API
  slug: bls-gov-time-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bls-gov/refs/heads/main/openapi/bls-gov-time-series-api-openapi.yml
consequence_counts:
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bls Gov Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Bureau of Labor Statistics exposes 5 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bureau of Labor Statistics
provider_slug: bls-gov
slug: bls-gov-agentic-access
source_filename: bls-gov-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/bls-gov-popular-series-api-openapi.yml, openapi/bls-gov-surveys-api-openapi.yml,\n  openapi/bls-gov-time-series-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 5\n  by_consequence:\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /timeseries/popular\n  method: get\n  operationId: getPopularSeries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /surveys\n  method: get\n  operationId: listSurveys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /surveys/{surveyAbbreviation}\n  method: get\n  operationId: getSurveyDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /timeseries/data/\n  method: post\n  operationId: getMultipleTimeSeries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /timeseries/data/{seriesId}\n  method: get\n  operationId: getSingleTimeSeries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bls-gov/refs/heads/main/agentic-access/bls-gov-agentic-access.yml
summary_line: 5 operations
tags:
- Federal Government
- Labor Statistics
- Economic Data
- Consumer Price Index
- Producer Price Index
- Employment
- Unemployment
- Wages
- Productivity
- Open Data
- Time Series
- Government Data
---
