---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 5
api_specs:
- filename: centers-for-disease-control-and-prevention-openapi.yml
  format: yaml
  label: CDC Socrata Open Data API (data.cdc.gov)
  slug: cdc-socrata-open-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centers-for-disease-control-and-prevention/refs/heads/main/openapi/centers-for-disease-control-and-prevention-openapi.yml
consequence_counts:
  read: 5
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Centers For Disease Control And Prevention Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Centers for Disease Control and Prevention exposes 6 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Centers for Disease Control and Prevention
provider_slug: centers-for-disease-control-and-prevention
slug: centers-for-disease-control-and-prevention-agentic-access
source_filename: centers-for-disease-control-and-prevention-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/centers-for-disease-control-and-prevention-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 5\n    acting: 1\n  by_consequence:\n    read: 5\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /resource/{dataset_id}.json\n  method: get\n  operationId: queryDatasetJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource/{dataset_id}.csv\n  method: get\n  operationId: queryDatasetCsv\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /resource/{dataset_id}.geojson\n  method: get\n  operationId: queryDatasetGeoJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/views/{dataset_id}/query.json\n  method: get\n  operationId: queryDatasetV3Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/views/{dataset_id}/query.json\n  method: post\n  operationId: queryDatasetV3Post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v3/views/{dataset_id}/export.{format}\n  method: get\n  operationId: exportDatasetV3\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/centers-for-disease-control-and-prevention/refs/heads/main/agentic-access/centers-for-disease-control-and-prevention-agentic-access.yml
summary_line: 6 operations · 1 acting
tags:
- CDC
- Environmental Health
- Epidemiology
- Federal Government
- Healthcare
- Open Data
- Public Health
- Socrata
- Surveillance
- WONDER
---
