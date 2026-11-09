---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 9
api_specs:
- filename: clay953f-credits-api-openapi.yml
  format: yaml
  label: Clay953f Credits API
  slug: clay953f-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clay953f/openapi/clay953f-credits-api-openapi.yml
- filename: clay953f-me-api-openapi.yml
  format: yaml
  label: Clay953f Me API
  slug: clay953f-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clay953f/openapi/clay953f-me-api-openapi.yml
- filename: clay953f-routines-api-openapi.yml
  format: yaml
  label: Clay953f Routines API
  slug: clay953f-routines-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clay953f/openapi/clay953f-routines-api-openapi.yml
- filename: clay953f-search-api-openapi.yml
  format: yaml
  label: Clay953f Search API
  slug: clay953f-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clay953f/openapi/clay953f-search-api-openapi.yml
- filename: clay953f-tables-api-openapi.yml
  format: yaml
  label: Clay953f Tables API
  slug: clay953f-tables-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clay953f/openapi/clay953f-tables-api-openapi.yml
- filename: clay953f-workflowsruns-api-openapi.yml
  format: yaml
  label: Clay953f Workflows Runs API
  slug: clay953f-workflowsruns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clay953f/openapi/clay953f-workflowsruns-api-openapi.yml
consequence_counts:
  read: 9
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Clay953F Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'Clay953f exposes 16 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Clay953f
provider_slug: clay953f
slug: clay953f-agentic-access
source_filename: clay953f-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/clay953f-credits-api-openapi.yml, openapi/clay953f-me-api-openapi.yml, openapi/clay953f-routines-api-openapi.yml,\n  openapi/clay953f-search-api-openapi.yml, openapi/clay953f-tables-api-openapi.yml, openapi/clay953f-workflowsruns-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 9\n    acting: 7\n  by_consequence:\n    read: 9\n    write: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /credits/balance\n  method: get\n  operationId: getCreditBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me\n  method: get\n\
  \  operationId: getPublicApiMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /routines/run-batch/{routine_run_id}/results\n  method: get\n  operationId: getRoutineRunBatchResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /routines/run/{routine_run_id}/results\n  method: get\n  operationId: getRunResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /routines/{routine_id}/run\n  method: post\n  operationId: runRoutine\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /routines/{routine_id}/run-batch/start\n  method: post\n  operationId: startRoutineRunBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /routines/{routine_id}/run-batch/upload-url\n  method: post\n  operationId: runRoutineBatchUploadUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /search/filters-mode\n  method: post\n  operationId: createFilters\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /search/filters-mode/fields\n  method: get\n  operationId: fields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/filters-mode/{search_id}/run\n  method: post\n  operationId: run\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /search/query-mode\n  method: post\n  operationId: createQueryMode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n    \
  \  triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /search/query-mode/reference\n  method: get\n  operationId: queryModeReference\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/query-mode/{search_id}/run\n  method: post\n  operationId: runQueryMode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tables/query\n  method: post\n  operationId: query\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workflows/runs/query\n  method: post\n  operationId: runQuery\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workflows/runs/query/reference\n  method: get\n  operationId: queryReference\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/clay953f/agentic-access/clay953f-agentic-access.yml
summary_line: 16 operations · 7 acting
tags:
- Data Marketplace
- CRM Enrichment
- AI Agents
---
