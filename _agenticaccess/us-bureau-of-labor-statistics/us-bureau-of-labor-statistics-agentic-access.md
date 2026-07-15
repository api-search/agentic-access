---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 4
api_specs:
- filename: bls-public-data-api-openapi.yml
  format: yaml
  label: BLS Public Data API
  slug: bls-public-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-bureau-of-labor-statistics/refs/heads/main/openapi/bls-public-data-api-openapi.yml
consequence_counts:
  read: 4
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Us Bureau Of Labor Statistics Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'US Bureau of Labor Statistics exposes 5 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: US Bureau of Labor Statistics
provider_slug: us-bureau-of-labor-statistics
slug: us-bureau-of-labor-statistics-agentic-access
source_filename: us-bureau-of-labor-statistics-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/bls-public-data-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    acting: 1\n    connected: 4\n  by_consequence:\n    write: 1\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /timeseries/data/\n  method: post\n  operationId: getMultipleTimeSeries\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /timeseries/data/{seriesId}\n  method: get\n  operationId: getSingleTimeSeries\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /surveys\n  method: get\n  operationId: listSurveys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /surveys/{surveyAbbreviation}\n  method: get\n  operationId: getSurveyDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /timeseries/popular\n  method: get\n  operationId: getPopularSeries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/us-bureau-of-labor-statistics/refs/heads/main/agentic-access/us-bureau-of-labor-statistics-agentic-access.yml
summary_line: 5 operations · 1 acting
tags:
- Federal Government
- Labor Statistics
- Economic Data
- Open Data
---
