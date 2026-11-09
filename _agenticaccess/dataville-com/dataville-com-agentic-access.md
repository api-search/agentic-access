---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 8
api_specs:
- filename: dataville-com-connected-sheets-api-openapi.yml
  format: yaml
  label: Dataville Connected sheets API
  slug: dataville-com-connected-sheets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataville-com/openapi/dataville-com-connected-sheets-api-openapi.yml
- filename: dataville-com-data-sources-api-openapi.yml
  format: yaml
  label: Dataville Data sources API
  slug: dataville-com-data-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataville-com/openapi/dataville-com-data-sources-api-openapi.yml
- filename: dataville-com-export-and-sql-api-openapi.yml
  format: yaml
  label: Dataville Export and SQL API
  slug: dataville-com-export-and-sql-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataville-com/openapi/dataville-com-export-and-sql-api-openapi.yml
- filename: dataville-com-usage-api-openapi.yml
  format: yaml
  label: Dataville Usage API
  slug: dataville-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataville-com/openapi/dataville-com-usage-api-openapi.yml
consequence_counts:
  read: 8
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Dataville Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'Dataville exposes 9 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Dataville
provider_slug: dataville-com
slug: dataville-com-agentic-access
source_filename: dataville-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/dataville-com-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 8\n    acting: 1\n  by_consequence:\n    read: 8\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /{source}/{keywords}\n  method: get\n  operationId: searchSource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /https:/{wikipediaUrl}\n  method: get\n  operationId: fetchByUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/export\n  method:\
  \ get\n  operationId: listExports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/query\n  method: post\n  operationId: runSqlQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/query.parquet\n  method: get\n  operationId: runSqlQueryParquet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/query.csv\n  method: get\n  operationId: runSqlQueryCsv\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/datasets/{id}/query\n\
  \  method: post\n  operationId: queryDataset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/datasets/{id}/search\n  method: get\n  operationId: searchDataset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/auth/usage\n  method: get\n  operationId: getAuthUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/dataville-com/agentic-access/dataville-com-agentic-access.yml
summary_line: 9 operations · 1 acting
tags:
- Data API
- AI Applications
- Financial Filings
- Research Data
- Knowledge Attribution
---
