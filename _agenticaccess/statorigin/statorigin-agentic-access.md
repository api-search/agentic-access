---
acting_count: 0
action_class_counts:
  connected: 17
api_specs:
- filename: statorigin-indicators-api-openapi.yml
  format: yaml
  label: StatOrigin Indicators API
  slug: statorigin-indicators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statorigin/refs/heads/main/openapi/statorigin-indicators-api-openapi.yml
- filename: statorigin-industries-api-openapi.yml
  format: yaml
  label: StatOrigin Industries API
  slug: statorigin-industries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statorigin/refs/heads/main/openapi/statorigin-industries-api-openapi.yml
- filename: statorigin-regions-api-openapi.yml
  format: yaml
  label: StatOrigin Regions API
  slug: statorigin-regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statorigin/refs/heads/main/openapi/statorigin-regions-api-openapi.yml
- filename: statorigin-search-api-openapi.yml
  format: yaml
  label: StatOrigin Search API
  slug: statorigin-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statorigin/refs/heads/main/openapi/statorigin-search-api-openapi.yml
- filename: statorigin-sources-api-openapi.yml
  format: yaml
  label: StatOrigin Sources API
  slug: statorigin-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statorigin/refs/heads/main/openapi/statorigin-sources-api-openapi.yml
- filename: statorigin-statistics-api-openapi.yml
  format: yaml
  label: StatOrigin Statistics API
  slug: statorigin-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statorigin/refs/heads/main/openapi/statorigin-statistics-api-openapi.yml
consequence_counts:
  read: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Statorigin Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'StatOrigin exposes 17 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: StatOrigin
provider_slug: statorigin
slug: statorigin-agentic-access
source_filename: statorigin-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: generated\nsource: openapi/statorigin-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    connected: 17\n  by_consequence:\n    read: 17\n  human_in_the_loop_required: 0\noperations:\n- path: /statistics\n  method: get\n  operationId: queryStatistics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /statistics/{id}\n  method: get\n  operationId: getStatistic\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /industries\n  method: get\n  operationId: listIndustries\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /industries/{slug}\n  method: get\n  operationId: getIndustry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /industries/{slug}/export.xlsx\n  method: get\n  operationId: exportIndustryXlsx\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /industries/{slug}/export.csv\n  method: get\n  operationId: exportIndustryCsv\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /indicators\n  method: get\n  operationId: listIndicators\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /indicators/{slug}\n  method: get\n  operationId: getIndicator\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /indicators/{slug}/series\n  method: get\n  operationId: getIndicatorSeries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /indicators/{slug}/export.xlsx\n  method: get\n  operationId: exportIndicatorXlsx\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /indicators/{slug}/export.csv\n  method: get\n  operationId: exportIndicatorCsv\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sources\n  method: get\n\
  \  operationId: listSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sources/{slug}\n  method: get\n  operationId: getSource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /regions\n  method: get\n  operationId: listRegions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /regions/{slug}/export.xlsx\n  method: get\n  operationId: exportRegionXlsx\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /regions/{slug}/export.csv\n  method: get\n  operationId: exportRegionCsv\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /search\n  method: get\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/statorigin/refs/heads/main/agentic-access/statorigin-agentic-access.yml
summary_line: 17 operations
tags:
- Company
- Data
- Statistics
- OpenAPI
- Free
---
