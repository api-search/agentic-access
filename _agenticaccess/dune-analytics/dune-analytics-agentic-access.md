---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 3
api_specs:
- filename: dune-analytics-execution-api-openapi.yml
  format: yaml
  label: Dune Analytics Execution API
  slug: dune-analytics-execution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dune-analytics/openapi/dune-analytics-execution-api-openapi.yml
- filename: dune-analytics-query-api-openapi.yml
  format: yaml
  label: Dune Analytics Query API
  slug: dune-analytics-query-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dune-analytics/openapi/dune-analytics-query-api-openapi.yml
- filename: dune-analytics-contracts-api-openapi.yml
  format: yaml
  label: Dune Analytics Contracts API
  slug: dune-analytics-contracts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dune-analytics/openapi/dune-analytics-contracts-api-openapi.yml
- filename: dune-analytics-dashboards-api-openapi.yml
  format: yaml
  label: Dune Analytics Dashboards API
  slug: dune-analytics-dashboards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dune-analytics/openapi/dune-analytics-dashboards-api-openapi.yml
- filename: dune-analytics-datasets-api-openapi.yml
  format: yaml
  label: Dune Analytics Datasets API
  slug: dune-analytics-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dune-analytics/openapi/dune-analytics-datasets-api-openapi.yml
- filename: dune-analytics-endpoints-api-openapi.yml
  format: yaml
  label: Dune Analytics Endpoints API
  slug: dune-analytics-endpoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dune-analytics/openapi/dune-analytics-endpoints-api-openapi.yml
- filename: dune-analytics-materialized-views-api-openapi.yml
  format: yaml
  label: Dune Analytics Materialized Views API
  slug: dune-analytics-materialized-views-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dune-analytics/openapi/dune-analytics-materialized-views-api-openapi.yml
- filename: dune-analytics-pipelines-api-openapi.yml
  format: yaml
  label: Dune Analytics Pipelines API
  slug: dune-analytics-pipelines-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dune-analytics/openapi/dune-analytics-pipelines-api-openapi.yml
- filename: dune-analytics-queries-api-openapi.yml
  format: yaml
  label: Dune Analytics Queries API
  slug: dune-analytics-queries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dune-analytics/openapi/dune-analytics-queries-api-openapi.yml
- filename: dune-analytics-sql-api-openapi.yml
  format: yaml
  label: Dune Analytics Sql API
  slug: dune-analytics-sql-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dune-analytics/openapi/dune-analytics-sql-api-openapi.yml
- filename: dune-analytics-uploads-api-openapi.yml
  format: yaml
  label: Dune Analytics Uploads API
  slug: dune-analytics-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dune-analytics/openapi/dune-analytics-uploads-api-openapi.yml
- filename: dune-analytics-usage-api-openapi.yml
  format: yaml
  label: Dune Analytics Usage API
  slug: dune-analytics-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dune-analytics/openapi/dune-analytics-usage-api-openapi.yml
- filename: dune-analytics-visualizations-api-openapi.yml
  format: yaml
  label: Dune Analytics Visualizations API
  slug: dune-analytics-visualizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dune-analytics/openapi/dune-analytics-visualizations-api-openapi.yml
consequence_counts:
  read: 3
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Dune Analytics Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Dune Analytics exposes 5 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Dune Analytics
provider_slug: dune-analytics
slug: dune-analytics-agentic-access
source_filename: dune-analytics-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/dune-analytics-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    acting: 2\n    connected: 3\n  by_consequence:\n    write: 2\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /query/{query_id}/execute\n  method: post\n  operationId: executeQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /execution/{execution_id}/status\n  method: get\n  operationId: getExecutionStatus\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /execution/{execution_id}/results\n  method: get\n  operationId: getExecutionResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /execution/{execution_id}/cancel\n  method: post\n  operationId: cancelExecution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /query/{query_id}/results\n  method: get\n  operationId: getLatestQueryResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/dune-analytics/agentic-access/dune-analytics-agentic-access.yml
summary_line: 5 operations · 2 acting
tags:
- Web3
- Analytics
- SQL
- Dashboards
- Blockchain
- Onchain
- Multi-Chain
- Ethereum
---
