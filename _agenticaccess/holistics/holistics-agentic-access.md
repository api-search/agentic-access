---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 9
api_specs:
- filename: holistics-openapi.yml
  format: yaml
  label: Holistics Data Schedules & Jobs API
  slug: holistics-data-schedules-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/holistics/refs/heads/main/openapi/holistics-openapi.yml
- filename: holistics-openapi.yml
  format: yaml
  label: Holistics Dashboards & Reports API
  slug: holistics-dashboards-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/holistics/refs/heads/main/openapi/holistics-openapi.yml
- filename: holistics-openapi.yml
  format: yaml
  label: Holistics Export API
  slug: holistics-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/holistics/refs/heads/main/openapi/holistics-openapi.yml
- filename: holistics-openapi.yml
  format: yaml
  label: Holistics Users & Permissions API
  slug: holistics-users-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/holistics/refs/heads/main/openapi/holistics-openapi.yml
- filename: holistics-openapi.yml
  format: yaml
  label: Holistics Embedded Analytics API
  slug: holistics-embedded-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/holistics/refs/heads/main/openapi/holistics-openapi.yml
consequence_counts:
  read: 9
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Holistics Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'Holistics exposes 13 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Holistics
provider_slug: holistics
slug: holistics-agentic-access
source_filename: holistics-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/holistics-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 9\n    acting: 4\n  by_consequence:\n    read: 9\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /data_sets\n  method: get\n  operationId: listDataSets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data_sets/{id}\n  method: get\n  operationId: getDataSet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data_sets/{id}/submit_query\n  method: post\n\
  \  operationId: submitDataSetQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data_sets/{id}/generate_sql\n  method: post\n  operationId: generateDataSetSql\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /queries/{report_id}/submit_query.json\n  method: get\n  operationId: submitReportQuery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /queries/get_query_results.json\n  method: get\n  operationId: getQueryResults\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /queries/{report_id}/submit_export.{format}\n  method: get\n  operationId: submitReportExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /queries/get_export_results.json\n  method: get\n  operationId: getExportResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exports/download\n  method: get\n  operationId: downloadExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data_imports/{data_import_id}/execute.json\n  method: post\n  operationId: executeDataImport\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data_transforms/{data_transform_id}/execute.json\n  method: post\n  operationId: executeDataTransform\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs/{job_id}/logs.json\n  method: get\n  operationId: getJobLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/last_run_jobs.json\n  method: get\n  operationId: getLastRunJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/holistics/refs/heads/main/agentic-access/holistics-agentic-access.yml
summary_line: 13 operations · 4 acting
tags:
- Business Intelligence
- Analytics
- Self-Service BI
- Data Modeling
- Embedded Analytics
---
