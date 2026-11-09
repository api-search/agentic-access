---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 13
api_specs:
- filename: vertex-documents-api-openapi.yml
  format: yaml
  label: Vertex Documents API
  slug: vertex-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vertex/openapi/vertex-documents-api-openapi.yml
- filename: vertex-problems-api-openapi.yml
  format: yaml
  label: Vertex Problems API
  slug: vertex-problems-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vertex/openapi/vertex-problems-api-openapi.yml
- filename: vertex-project-api-openapi.yml
  format: yaml
  label: Vertex Project API
  slug: vertex-project-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vertex/openapi/vertex-project-api-openapi.yml
- filename: vertex-reports-api-openapi.yml
  format: yaml
  label: Vertex Reports API
  slug: vertex-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vertex/openapi/vertex-reports-api-openapi.yml
- filename: vertex-schedules-api-openapi.yml
  format: yaml
  label: Vertex Schedules API
  slug: vertex-schedules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vertex/openapi/vertex-schedules-api-openapi.yml
- filename: vertex-templates-api-openapi.yml
  format: yaml
  label: Vertex Templates API
  slug: vertex-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vertex/openapi/vertex-templates-api-openapi.yml
- filename: vertex-vertex-api-api-openapi.yml
  format: yaml
  label: Vertex Vertex API
  slug: vertex-vertex-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vertex/openapi/vertex-vertex-api-api-openapi.yml
- filename: vertex-vertex-ws-api-openapi.yml
  format: yaml
  label: Vertex Vertex Ws API
  slug: vertex-vertex-ws-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vertex/openapi/vertex-vertex-ws-api-openapi.yml
consequence_counts:
  read: 13
  safety-critical: 1
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Vertex Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/schedules/{scheduleid}
operation_count: 23
overview: 'Vertex exposes 23 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read, 9 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Vertex
provider_slug: vertex
slug: vertex-agentic-access
source_filename: vertex-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/vertex-documents-api-openapi.yml, openapi/vertex-problems-api-openapi.yml, openapi/vertex-project-api-openapi.yml,\n  openapi/vertex-reports-api-openapi.yml, openapi/vertex-schedules-api-openapi.yml, openapi/vertex-templates-api-openapi.yml,\n  openapi/vertex-vertex-api-api-openapi.yml, openapi/vertex-vertex-ws-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 13\n    acting: 10\n  by_consequence:\n    read: 13\n    write: 9\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /documents/url\n  method: get\n  operationId: get_documents_url\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /problems/{problemid}\n  method: get\n  operationId: get_problems_problemid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /project/solutionreporting/v1.0/docs/using-the-solution-reporting-api\n  method: get\n  operationId: get_project_solutionreporting_v1_0_docs_using_the_solution_reporting_api\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /project/vat-compliance/v1.0/docs/upload-customer-data-files\n  method: get\n  operationId: get_project_vat_compliance_v1_0_docs_upload_customer_data_files\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/reports/results/{reportresultid}\n\
  \  method: delete\n  operationId: delete_api_v1_reports_results_reportresultid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/reports/results/{reportresultid}\n  method: get\n  operationId: get_api_v1_reports_results_reportresultid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/reports/results/{reportresultid}/cancel\n  method: post\n  operationId: post_api_v1_reports_results_reportresultid_cancel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/v1/reports/{definitionid}/results/{reportresultid}\n  method: get\n  operationId: get_api_v1_reports_definitionid_results_reportresultid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/reports/{reportid}\n  method: delete\n  operationId: delete_api_v1_reports_reportid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/reports/{reportid}\n  method: get\n  operationId: get_api_v1_reports_reportid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/reports/{reportid}\n  method:\
  \ put\n  operationId: put_api_v1_reports_reportid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/reports/{reportid}/results\n  method: post\n  operationId: post_api_v1_reports_reportid_results\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/reports/{reportid}/schedules\n  method: delete\n  operationId: delete_api_v1_reports_reportid_schedules\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/reports/{reportid}/schedules/{scheduleid}\n  method: delete\n  operationId: delete_api_v1_reports_reportid_schedules_scheduleid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/reports/{reportid}/{id}\n  method: get\n  operationId: get_api_v1_reports_reportid_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/schedules/{scheduleid}\n  method: delete\n  operationId: delete_api_v1_schedules_scheduleid\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/schedules/{scheduleid}\n  method: get\n  operationId: get_api_v1_schedules_scheduleid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/schedules/{scheduleid}\n  method: put\n  operationId: put_api_v1_schedules_scheduleid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/templates/{templateid}\n  method: get\n  operationId: get_api_v1_templates_templateid\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/{v1id}\n  method: get\n  operationId: get_api_v1_v1id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/{v1id}\n  method: post\n  operationId: post_api_v1_v1id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vertex-ws/v2/supplies\n  method: get\n  operationId: get_vertex_ws_v2_supplies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/vertex/agentic-access/vertex-agentic-access.yml
summary_line: 23 operations · 10 acting · 1 human-in-the-loop
tags:
- Company
- Tax
- Compliance
- Automation
---
