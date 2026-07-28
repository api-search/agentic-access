---
acting_count: 0
action_class_counts:
  connected: 9
api_specs:
- filename: western-power-outage-openapi.yml
  format: yaml
  label: Western Power Outage Web API
  slug: western-power-outage-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/western-power/refs/heads/main/openapi/western-power-outage-openapi.yml
- filename: western-power-corporate-web-openapi.yml
  format: yaml
  label: Western Power Corporate Web API
  slug: western-power-corporate-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/western-power/refs/heads/main/openapi/western-power-corporate-web-openapi.yml
- filename: western-power-arcgis-outage-openapi.yml
  format: yaml
  label: Western Power Outage Areas Feature Service
  slug: western-power-outage-areas-feature-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/western-power/refs/heads/main/openapi/western-power-arcgis-outage-openapi.yml
consequence_counts:
  read: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Western Power Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'Western Power exposes 9 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Western Power
provider_slug: western-power
slug: western-power-agentic-access
source_filename: western-power-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: generated\nsource: openapi/western-power-arcgis-outage-openapi.yml, openapi/western-power-corporate-web-openapi.yml,\n  openapi/western-power-outage-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 9\n  by_consequence:\n    read: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: getFeatureServerMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /0\n  method: get\n  operationId: getOutageAreasLayerMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /0/query\n  method: get\n  operationId: queryOutageAreas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search\n  method: get\n  operationId: searchSite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /corp/newsarticles\n  method: get\n  operationId: listNewsArticles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /corp/vacancies\n  method: get\n  operationId: listVacancies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /all-outages\n  method: get\n  operationId: listAllOutages\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /details/{outageId}\n  method: get\n  operationId: getOutageDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status/{suburb}\n  method: get\n  operationId: getSuburbOutageStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/western-power/refs/heads/main/agentic-access/western-power-agentic-access.yml
summary_line: 9 operations
tags:
- Energy
- Australia
- Utilities
- Electricity
- Grid
- Network Distribution
- Smart Metering
- Open Data
- GIS
- Outages
---
