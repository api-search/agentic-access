---
acting_count: 0
action_class_counts:
  connected: 9
api_specs:
- filename: openapi.yaml
  format: yaml
  label: NOAA ERDDAP REST API
  slug: noaa-erddap-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa-erddap/refs/heads/main/openapi/openapi.yaml
consequence_counts:
  read: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Noaa Erddap Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'NOAA ERDDAP exposes 9 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: NOAA ERDDAP
provider_slug: noaa-erddap
slug: noaa-erddap-agentic-access
source_filename: noaa-erddap-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 9\n  by_consequence:\n    read: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /search/index.{fileType}\n  method: get\n  operationId: searchDatasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/advanced.{fileType}\n  method: get\n  operationId: searchDatasetsAdvanced\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /info/index.{fileType}\n  method: get\n\
  \  operationId: listAllDatasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /categorize/{attribute}/index.{fileType}\n  method: get\n  operationId: listAttributeValues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /categorize/{attribute}/{value}/index.{fileType}\n  method: get\n  operationId: listDatasetsByAttribute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /info/{datasetID}/index.{fileType}\n  method: get\n  operationId: getDatasetInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tabledap/{datasetID}.{fileType}\n  method: get\n  operationId: getTabledapData\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /griddap/{datasetID}.{fileType}\n  method: get\n  operationId: getGriddapData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/{datasetID}\n  method: get\n  operationId: listDatasetFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/noaa-erddap/refs/heads/main/agentic-access/noaa-erddap-agentic-access.yml
summary_line: 9 operations
tags:
- oceanography
- meteorology
- climate
- environmental data
- gridded data
- tabular data
- scientific data
- government
- NOAA
- open data
---
