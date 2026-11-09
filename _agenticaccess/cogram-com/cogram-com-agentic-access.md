---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 15
api_specs:
- filename: cogram-com-action-items-api-openapi.yml
  format: yaml
  label: Cogram Action Items API
  slug: cogram-com-action-items-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cogram-com/openapi/cogram-com-action-items-api-openapi.yml
- filename: cogram-com-audit-log-api-openapi.yml
  format: yaml
  label: Cogram Audit Log API
  slug: cogram-com-audit-log-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cogram-com/openapi/cogram-com-audit-log-api-openapi.yml
- filename: cogram-com-backup-runs-api-openapi.yml
  format: yaml
  label: Cogram Backup Runs API
  slug: cogram-com-backup-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cogram-com/openapi/cogram-com-backup-runs-api-openapi.yml
- filename: cogram-com-board-items-api-openapi.yml
  format: yaml
  label: Cogram Board Items API
  slug: cogram-com-board-items-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cogram-com/openapi/cogram-com-board-items-api-openapi.yml
- filename: cogram-com-data-exports-api-openapi.yml
  format: yaml
  label: Cogram Data Exports API
  slug: cogram-com-data-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cogram-com/openapi/cogram-com-data-exports-api-openapi.yml
- filename: cogram-com-directory-api-openapi.yml
  format: yaml
  label: Cogram Directory API
  slug: cogram-com-directory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cogram-com/openapi/cogram-com-directory-api-openapi.yml
- filename: cogram-com-project-templates-api-openapi.yml
  format: yaml
  label: Cogram Project Templates API
  slug: cogram-com-project-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cogram-com/openapi/cogram-com-project-templates-api-openapi.yml
- filename: cogram-com-project-types-api-openapi.yml
  format: yaml
  label: Cogram Project Types API
  slug: cogram-com-project-types-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cogram-com/openapi/cogram-com-project-types-api-openapi.yml
- filename: cogram-com-projects-api-openapi.yml
  format: yaml
  label: Cogram Projects API
  slug: cogram-com-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cogram-com/openapi/cogram-com-projects-api-openapi.yml
- filename: cogram-com-users-api-openapi.yml
  format: yaml
  label: Cogram Users API
  slug: cogram-com-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cogram-com/openapi/cogram-com-users-api-openapi.yml
consequence_counts:
  read: 15
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cogram Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 30
overview: 'Cogram exposes 30 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read and 15 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cogram
provider_slug: cogram-com
slug: cogram-com-agentic-access
source_filename: cogram-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/api.cogram.com-v1-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 30\n  by_action_class:\n    connected: 15\n    acting: 15\n  by_consequence:\n    read: 15\n    write: 15\n  human_in_the_loop_required: 0\noperations:\n- path: /action-items\n  method: get\n  operationId: external_list_action_items_route_action_items_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /audit-log\n  method: get\n  operationId: external_list_audit_log_route_audit_log_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n- path: /backup-runs\n  method: post\n  operationId: external_create_backup_run_route_backup_runs_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /board-items\n  method: get\n  operationId: external_list_board_items_route_board_items_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /board-items/{item_id}\n  method: get\n  operationId: external_get_board_item_route_board_items__item_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /project-types\n  method: get\n  operationId: external_list_project_types_route_project_types_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /project-types\n  method: post\n  operationId: external_create_project_type_route_project_types_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /project-types/{type_id}\n  method: get\n  operationId: external_get_project_type_route_project_types__type_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /project-types/{type_id}\n  method: patch\n  operationId: external_update_project_type_route_project_types__type_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /project-types/{type_id}\n  method: delete\n  operationId: external_delete_project_type_route_project_types__type_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /project-templates\n  method: get\n  operationId: external_list_project_templates_route_project_templates_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /project-templates\n  method: post\n  operationId: external_create_project_template_route_project_templates_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /project-templates/{template_id}\n  method: get\n  operationId: external_get_project_template_route_project_templates__template_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /project-templates/{template_id}\n  method: put\n  operationId: external_update_project_template_route_project_templates__template_id__put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /projects\n  method: get\n  operationId: external_list_projects_route_projects_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects\n  method: post\n  operationId: external_create_project_route_projects_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}\n  method: get\n  operationId: external_get_project_route_projects__project_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}\n  method: patch\n  operationId: external_update_project_route_projects__project_id__patch\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}\n  method: delete\n  operationId: external_delete_project_route_projects__project_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/members\n  method: get\n  operationId: external_list_project_members_route_projects__project_id__members_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/members/{user_id}\n  method:\
  \ put\n  operationId: external_set_project_member_route_projects__project_id__members__user_id__put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/members/{user_id}\n  method: delete\n  operationId: external_remove_project_member_route_projects__project_id__members__user_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data-exports\n  method: post\n  operationId: external_create_data_export_route_data_exports_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data-exports\n  method: get\n  operationId: external_list_data_exports_route_data_exports_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data-exports/{data_export_id}\n  method: get\n  operationId: external_get_data_export_route_data_exports__data_export_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data-exports/{data_export_id}/cancel\n  method: post\n  operationId: external_cancel_data_export_route_data_exports__data_export_id__cancel_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /directory/contact-company-links\n  method: get\n  operationId: external_list_contact_company_links_route_directory_contact_company_links_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /directory/contact-company-links\n  method: post\n  operationId: external_apply_contact_company_links_route_directory_contact_company_links_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users\n  method: get\n  operationId: external_list_users_route_users_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{user_id}\n  method: patch\n  operationId: external_update_user_route_users__user_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/cogram-com/agentic-access/cogram-com-agentic-access.yml
summary_line: 30 operations · 15 acting
tags:
- Artificial Intelligence
- Architecture
- Engineering
- Documentation
- Collaboration
---
