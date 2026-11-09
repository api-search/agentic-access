---
acting_count: 19
action_class_counts:
  acting: 19
  connected: 21
api_specs:
- filename: regrow-ag-ogc-api-general-api-openapi.yml
  format: yaml
  label: Regrow OGC API - General API
  slug: regrow-ag-ogc-api-general-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/regrow-ag/openapi/regrow-ag-ogc-api-general-api-openapi.yml
- filename: regrow-ag-ogc-api-processes-api-openapi.yml
  format: yaml
  label: Regrow OGC API - Processes API
  slug: regrow-ag-ogc-api-processes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/regrow-ag/openapi/regrow-ag-ogc-api-processes-api-openapi.yml
- filename: regrow-ag-v0-explore-api-intervention-api-openapi.yml
  format: yaml
  label: Regrow V0 Explore API - Intervention API
  slug: regrow-ag-v0-explore-api-intervention-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/regrow-ag/openapi/regrow-ag-v0-explore-api-intervention-api-openapi.yml
- filename: regrow-ag-v0-measure-api-intervention-api-openapi.yml
  format: yaml
  label: Regrow V0 Measure API - Intervention API
  slug: regrow-ag-v0-measure-api-intervention-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/regrow-ag/openapi/regrow-ag-v0-measure-api-intervention-api-openapi.yml
- filename: regrow-ag-v0-measure-api-inventory-api-openapi.yml
  format: yaml
  label: Regrow V0 Measure API - Inventory API
  slug: regrow-ag-v0-measure-api-inventory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/regrow-ag/openapi/regrow-ag-v0-measure-api-inventory-api-openapi.yml
- filename: regrow-ag-v1-measure-api-enteric-api-openapi.yml
  format: yaml
  label: Regrow V1 Measure API - Enteric API
  slug: regrow-ag-v1-measure-api-enteric-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/regrow-ag/openapi/regrow-ag-v1-measure-api-enteric-api-openapi.yml
consequence_counts:
  read: 21
  write: 19
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Regrow Ag Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 40
overview: 'Regrow exposes 40 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read and 19 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Regrow
provider_slug: regrow-ag
slug: regrow-ag-agentic-access
source_filename: regrow-ag-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: generated\nsource: openapi/regrow-ag-measure-api-openapi.yml, openapi/regrow-ag-monitor-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 40\n  by_action_class:\n    acting: 19\n    connected: 21\n  by_consequence:\n    write: 19\n    read: 21\n  human_in_the_loop_required: 0\noperations:\n- path: /v0/explore_api/fields\n  method: post\n  operationId: upload_field_v0_explore_api_fields_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/explore_api/fields\n\
  \  method: get\n  operationId: list_fields_v0_explore_api_fields_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/explore_api/fields/{field_request_id}\n  method: get\n  operationId: get_raw_input_v0_v0_explore_api_fields__field_request_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/explore_api/fields/{field_request_id}/status\n  method: get\n  operationId: get_status_v0_explore_api_fields__field_request_id__status_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/explore_api/fields/{field_request_id}/results\n  method: get\n  operationId: get_estimates_v0_explore_api_fields__field_request_id__results_get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/api/projects/{project_name}/fields\n  method: post\n  operationId: upload_field_v0_api_projects__project_name__fields_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/api/projects/{project_name}/fields\n  method: get\n  operationId: list_fields_v0_api_projects__project_name__fields_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/api/projects/{project_name}/fields/{field_request_id}\n  method: get\n  operationId: get_raw_input_v0_api_projects__project_name__fields__field_request_id__get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/api/projects/{project_name}/fields/{field_request_id}\n  method: delete\n  operationId: delete_field_v0_api_projects__project_name__fields__field_request_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/api/protocols\n  method: get\n  operationId: list_protocols_v0_api_protocols_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/api/projects\n  method: post\n  operationId: create_project_v0_api_projects_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/api/projects\n  method: get\n  operationId: list_projects_v0_api_projects_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/api/projects/{project_name}\n  method: delete\n  operationId: delete_project_v0_api_projects__project_name__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/api/projects/{project_name}/finalize\n  method: post\n  operationId: finalize_project_v0_api_projects__project_name__finalize_post\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/api/project_level_scope_1\n  method: get\n  operationId: scope_1_results_v0_api_project_level_scope_1_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/api/project_level_scope_3\n  method: get\n  operationId: scope_3_results_v0_api_project_level_scope_3_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/inventory/projects/{project_name}/fields\n  method: post\n  operationId: upload_field_v0_inventory_projects__project_name__fields_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/inventory/projects/{project_name}/fields\n  method: get\n  operationId: list_fields_v0_inventory_projects__project_name__fields_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/inventory/projects/{project_name}/fields/{field_request_id}\n  method: get\n  operationId: get_field_v0_inventory_projects__project_name__fields__field_request_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/inventory/projects/{project_name}/fields/{field_request_id}\n  method: delete\n  operationId: delete_field_v0_inventory_projects__project_name__fields__field_request_id__delete\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/inventory/projects\n  method: post\n  operationId: create_project_v0_inventory_projects_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/inventory/projects\n  method: get\n  operationId: list_projects_v0_inventory_projects_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/inventory/projects/{project_name}/finalize\n  method: post\n  operationId: finalize_project_v0_inventory_projects__project_name__finalize_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/inventory/projects/{project_name}\n  method: delete\n  operationId: delete_project_v0_inventory_projects__project_name__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/inventory/projects/{project_name}\n  method: get\n  operationId: get_results_v0_inventory_projects__project_name__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/enteric/projects/{project_name}/ranchers\n\
  \  method: post\n  operationId: upload_rancher_v1_enteric_projects__project_name__ranchers_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/enteric/projects/{project_name}/ranchers\n  method: get\n  operationId: list_ranchers_v1_enteric_projects__project_name__ranchers_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/enteric/projects/{project_name}/ranchers/{rancher_id}\n  method: put\n  operationId: update_rancher_v1_enteric_projects__project_name__ranchers__rancher_id__put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/enteric/projects/{project_name}/ranchers/{rancher_id}\n  method: delete\n  operationId: delete_rancher_v1_enteric_projects__project_name__ranchers__rancher_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/enteric/projects/{project_name}/ranchers/{rancher_id}\n  method: get\n  operationId: get_rancher_v1_enteric_projects__project_name__ranchers__rancher_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/enteric/projects\n  method: post\n  operationId: v1_create_project_v1_enteric_projects_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/enteric/projects\n  method: get\n  operationId: v1_list_projects_v1_enteric_projects_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/enteric/projects/{project_name}/finalize\n  method: post\n  operationId: finalize_project_v1_enteric_projects__project_name__finalize_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/enteric/projects/{project_name}\n  method: get\n  operationId:\
  \ v1_get_results_v1_enteric_projects__project_name__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/enteric/projects/{project_name}\n  method: delete\n  operationId: delete_project_v1_enteric_projects__project_name__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs/{job_id}\n  method: get\n  operationId: get_job_status_jobs__job_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{job_id}/results\n  method: get\n  operationId: get_job_results_jobs__job_id__results_get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /processes/monitor-fields-boundary-id/execution\n  method: post\n  operationId: Monitor_Field_processes_monitor_fields_boundary_id_execution_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /processes/monitor-fields-geojson/execution\n  method: post\n  operationId: Monitor_Field_Geojson_processes_monitor_fields_geojson_execution_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /status\n  method: get\n  operationId:\
  \ health_check_status_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/regrow-ag/agentic-access/regrow-ag-agentic-access.yml
summary_line: 40 operations · 19 acting
tags:
- Company
- Agriculture
- Sustainability
- Greenhouse Gas Emissions
- Carbon
- Regenerative Agriculture
- Remote Sensing
- Climate
---
