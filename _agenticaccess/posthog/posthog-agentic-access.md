---
acting_count: 927
action_class_counts:
  acting: 927
  connected: 640
api_specs:
- filename: posthog-openapi.yml
  format: yaml
  label: PostHog API
  slug: posthog
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/posthog/refs/heads/main/openapi/posthog-openapi.yml
consequence_counts:
  physical: 17
  read: 640
  safety-critical: 18
  write: 892
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 18
kind: agentic-access
layout: agentic-access
method: generated
name: Posthog Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/environments/{environment_id}/data_warehouse/reset-password/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/environments/{environment_id}/logs/alerts/{id}/reset/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/environments/{environment_id}/persons/reset_person_distinct_id/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/environments/{project_id}/llm_skills/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/environments/{project_id}/llm_skills/name/{skill_name}/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/environments/{project_id}/llm_skills/name/{skill_name}/archive/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/environments/{project_id}/llm_skills/name/{skill_name}/duplicate/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/environments/{project_id}/llm_skills/name/{skill_name}/files-rename/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/environments/{project_id}/llm_skills/name/{skill_name}/files/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/environments/{project_id}/llm_skills/name/{skill_name}/files/{file_path}/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/organizations/{organization_id}/projects/{id}/reset_token/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/projects/{project_id}/data_warehouse/reset-password/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/projects/{project_id}/environments/{id}/reset_token/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/projects/{project_id}/experiments/{id}/reset/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/projects/{project_id}/logs/alerts/{id}/reset/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/projects/{project_id}/notebooks/{short_id}/kernel/stop/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/projects/{project_id}/persons/reset_person_distinct_id/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/users/{uuid}/two_factor_disable/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/environments/{environment_id}/dashboards/{id}/reorder_tiles/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/environments/{environment_id}/data_warehouse/deprovision/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/environments/{environment_id}/data_warehouse/provision/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/environments/{environment_id}/file_system_shortcut/reorder/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/environments/{environment_id}/logs/sampling_rules/reorder/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/environments/{project_id}/error_tracking/assignment_rules/reorder/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/environments/{project_id}/error_tracking/grouping_rules/reorder/
operation_count: 1567
overview: 'PostHog exposes 1567 API operations that an AI agent could call, of which 927 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 640 read, 892 write, 17 physical, and 18 safety-critical.


  18 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: PostHog
provider_slug: posthog
slug: posthog-agentic-access
source_filename: posthog-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/posthog-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 1567\n  by_action_class:\n    connected: 640\n    acting: 927\n  by_consequence:\n    read: 640\n    write: 892\n    physical: 17\n    safety-critical: 18\n  human_in_the_loop_required: 18\noperations:\n- path: /api/code/invites/check-access/\n  method: get\n  operationId: code_invites_check_access_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/code/invites/redeem/\n  method: post\n  operationId: code_invites_redeem_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n \
  \   subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/environments/{environment_id}/alerts/\n  method: get\n  operationId: environments_alerts_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - alert:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/environments/{environment_id}/alerts/\n  method: post\n  operationId: environments_alerts_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - alert:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/environments/{environment_id}/alerts/{id}/\n  method: get\n  operationId: environments_alerts_retrieve\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - alert:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/environments/{environment_id}/alerts/{id}/\n  method: put\n  operationId: environments_alerts_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - alert:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/environments/{environment_id}/alerts/{id}/\n  method: patch\n  operationId: environments_alerts_partial_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - alert:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /api/environments/{environment_id}/alerts/{id}/\n  method: delete\n  operationId: environments_alerts_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - alert:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/environments/{environment_id}/alerts/simulate/\n  method: post\n  operationId: environments_alerts_simulate_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - alert:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/environments/{environment_id}/batch_exports/\n  method: get\n  operationId: environments_batch_exports_list\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - batch_export:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/environments/{environment_id}/batch_exports/\n  method: post\n  operationId: environments_batch_exports_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - batch_export:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/environments/{environment_id}/batch_exports/{batch_export_id}/backfills/\n  method: get\n  operationId: environments_batch_exports_backfills_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - batch_export:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/environments/{environment_id}/batch_exports/{batch_export_id}/backfills/\n\
  \  method: post\n  operationId: environments_batch_exports_backfills_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - batch_export:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/environments/{environment_id}/batch_exports/{batch_export_id}/backfills/{id}/\n  method: get\n  operationId: environments_batch_exports_backfills_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - batch_export:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/environments/{environment_id}/batch_exports/{batch_export_id}/backfills/{id}/cancel/\n  method: post\n  operationId: environments_batch_exports_backfills_cancel_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n  \
  \  subject: required\n    scope:\n    - batch_export:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/environments/{environment_id}/batch_exports/{batch_export_id}/runs/\n  method: get\n  operationId: environments_batch_exports_runs_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - batch_export:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/environments/{environment_id}/batch_exports/{batch_export_id}/runs/{id}/\n  method: get\n  operationId: environments_batch_exports_runs_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - batch_export:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/environments/{environment_id}/batch_exports/{batch_export_id}/runs/{id}/cancel/\n\
  \  method: post\n  operationId: environments_batch_exports_runs_cancel_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - batch_export:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/environments/{environment_id}/batch_exports/{batch_export_id}/runs/{id}/logs/\n  method: get\n  operationId: environments_batch_exports_runs_logs_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/environments/{environment_id}/batch_exports/{batch_export_id}/runs/{id}/retry/\n  method: post\n  operationId: environments_batch_exports_runs_retry_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - batch_export:write\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/environments/{environment_id}/batch_exports/{id}/\n  method: get\n  operationId: environments_batch_exports_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - batch_export:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/environments/{environment_id}/batch_exports/{id}/\n  method: put\n  operationId: environments_batch_exports_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - batch_export:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/environments/{environment_id}/batch_exports/{id}/\n\
  \  method: patch\n  operationId: environments_batch_exports_partial_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - batch_export:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/environments/{environment_id}/batch_exports/{id}/\n  method: delete\n  operationId: environments_batch_exports_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - batch_export:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/environments/{environment_id}/batch_exports/{id}/logs/\n  method: get\n  operationId: environments_batch_exports_logs_retrieve\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/environments/{environment_id}/batch_exports/{id}/pause/\n  method: post\n  operationId: environments_batch_exports_pause_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - batch_export:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/environments/{environment_id}/batch_exports/{id}/run_test_step/\n  method: post\n  operationId: environments_batch_exports_run_test_step_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - batch_export:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n  \
  \    - abnormal\n      - high-value\n    audit: required\n- path: /api/environments/{environment_id}/batch_exports/{id}/unpause/\n  method: post\n  operationId: environments_batch_exports_unpause_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - batch_export:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/environments/{environment_id}/batch_exports/run_test_step_new/\n  method: post\n  operationId: environments_batch_exports_run_test_step_new_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - batch_export:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /api/environments/{environment_id}/batch_exports/test/\n  method: get\n  operationId: environments_batch_exports_test_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - batch_export:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/environments/{environment_id}/dashboards/\n  method: get\n  operationId: environments_dashboards_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - dashboard:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/environments/{environment_id}/dashboards/\n  method: post\n  operationId: environments_dashboards_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - dashboard:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/environments/{environment_id}/dashboards/{dashboard_id}/collaborators/\n  method: get\n  operationId: environments_dashboards_collaborators_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - dashboard:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/environments/{environment_id}/dashboards/{dashboard_id}/collaborators/\n  method: post\n  operationId: environments_dashboards_collaborators_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - dashboard:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/environments/{environment_id}/dashboards/{dashboard_id}/collaborators/{user__uuid}/\n  method: delete\n  operationId: environments_dashboards_collaborators_destroy\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - dashboard:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/environments/{environment_id}/dashboards/{dashboard_id}/sharing/\n  method: get\n  operationId: environments_dashboards_sharing_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - sharing_configuration:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/environments/{environment_id}/dashboards/{dashboard_id}/sharing/passwords/\n  method: post\n  operationId: environments_dashboards_sharing_passwords_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - sharing_configuration:write\n    audience: null\n    token:\n    \
  \  max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/environments/{environment_id}/dashboards/{dashboard_id}/sharing/passwords/{password_id}/\n  method: delete\n  operationId: environments_dashboards_sharing_passwords_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - sharing_configuration:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/environments/{environment_id}/dashboards/{dashboard_id}/sharing/refresh/\n  method: post\n  operationId: environments_dashboards_sharing_refresh_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - sharing_configuration:write\n    audience: null\n    token:\n \
  \     max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/environments/{environment_id}/dashboards/{id}/\n  method: get\n  operationId: environments_dashboards_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - dashboard:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/environments/{environment_id}/dashboards/{id}/\n  method: put\n  operationId: environments_dashboards_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - dashboard:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/environments/{environment_id}/dashboards/{id}/\n  method: patch\n  operationId: environments_dashboards_partial_update\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - dashboard:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/environments/{environment_id}/dashboards/{id}/\n  method: delete\n  operationId: environments_dashboards_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - dashboard:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/environments/{environment_id}/dashboards/{id}/analyze_refresh_result/\n  method: post\n  operationId: environments_dashboards_analyze_refresh_result_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/environments/{environment_id}/dashboards/{id}/copy_tile/\n  method: post\n  operationId: environments_dashboards_copy_tile_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - dashboard:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/environments/{environment_id}/dashboards/{id}/move_tile/\n  method: patch\n  operationId: environments_dashboards_move_tile_partial_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/environments/{environment_id}/dashboards/{id}/reorder_tiles/\n  method: post\n  operationId: environments_dashboards_reorder_tiles_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - dashboard:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/environments/{environment_id}/dashboards/{id}/run_insights/\n  method: get\n  operationId: environments_dashboards_run_insights_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - query:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/environments/{environment_id}/dashboards/{id}/snapshot/\n  method:\
  \ post\n  operationId: environments_dashboards_snapshot_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/environments/{environment_id}/dashboards/{id}/stream_tiles/\n  method: get\n  operationId: environments_dashboards_stream_tiles_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/environments/{environment_id}/dashboards/bulk_update_tags/\n  method: post\n  operationId: environments_dashboards_bulk_update_tags_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/environments/{environment_id}/dashboards/create_from_template_json/\n  method: post\n  operationId: environments_dashboards_create_from_template_json_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/environments/{environment_id}/dashboards/create_unlisted_dashboard/\n  method: post\n  operationId: environments_dashboards_create_unlisted_dashboard_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/environments/{environment_id}/data_color_themes/\n\
  \  method: get\n  operationId: environments_data_color_themes_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - project:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/environments/{environment_id}/data_color_themes/\n  method: post\n  operationId: environments_data_color_themes_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - project:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/environments/{environment_id}/data_color_themes/{id}/\n  method: get\n  operationId: environments_data_color_themes_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - project:read\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/environments/{environment_id}/data_color_themes/{id}/\n  method: put\n  operationId: environments_data_color_themes_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - project:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/environments/{environment_id}/data_color_themes/{id}/\n  method: patch\n  operationId: environments_data_color_themes_partial_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - project:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/environments/{environment_id}/data_color_themes/{id}/\n  method: delete\n \
  \ operationId: environments_data_color_themes_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - project:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/environments/{environment_id}/data_modeling_jobs/\n  method: get\n  operationId: environments_data_modeling_jobs_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - warehouse_view:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/environments/{environment_id}/data_modeling_jobs/{id}/\n  method: get\n  operationId: environments_data_modeling_jobs_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - warehouse_view:read\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/environments/{environment_id}/data_modeling_jobs/recent/\n  method: get\n  operationId: environments_data_modeling_jobs_recent_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/environments/{environment_id}/data_modeling_jobs/running/\n  method: get\n  operationId: environments_data_modeling_jobs_running_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/environments/{environment_id}/data_warehouse/check-database-name/\n  method: get\n  operationId: environments_data_warehouse_check_database_name_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/environments/{environment_id}/data_warehouse/completed_activity/\n  method:\
  \ get\n  operationId: environments_data_warehouse_completed_activity_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/environments/{environment_id}/data_warehouse/data_health_issues/\n  method: get\n  operationId: environments_data_warehouse_data_health_issues_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/environments/{environment_id}/data_warehouse/data_ops_dashboard/\n  method: get\n  operationId: environments_data_warehouse_data_ops_dashboard_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - warehouse_view:write\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/environments/{environment_id}/data_warehouse/deprovision/\n  method: post\n  operationId: environments_data_warehouse_deprovision_create\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - warehouse_view:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/environments/{environment_id}/data_warehouse/job_stats/\n  method: get\n  operationId: environments_data_warehouse_job_stats_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/environments/{environment_id}/data_warehouse/property_values/\n  method: get\n  operationId: environments_data_warehouse_property_values_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - query:read\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/environments/{environment_id}/data_warehouse/provision/\n  method: post\n  operationId: environments_data_warehouse_provision_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - warehouse_view:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/environments/{environment_id}/data_warehouse/reset-password/\n  method: post\n  operationId: environments_data_warehouse_reset_password_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - warehouse_view:write\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n\
  \    audit: required\n- path: /api/environments/{environment_id}/data_warehouse/running_activity/\n  method: get\n  operationId: environments_data_warehouse_running_activity_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/environments/{environment_id}/data_warehouse/total_rows_stats/\n  method: get\n  operationId: environments_data_warehouse_total_rows_stats_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/environments/{environment_id}/data_warehouse/warehouse_status/\n  method: get\n  operationId: environments_data_warehouse_warehouse_status_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/environments/{environment_id}/dataset_items/\n\
  \  method: get\n  operationId: environments_dataset_items_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - dataset:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/environments/{environment_id}/dataset_items/\n  method: post\n  operationId: environments_dataset_items_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - dataset:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/environments/{environment_id}/dataset_items/{id}/\n  method: get\n  operationId: environments_dataset_items_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - dataset:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/environments/{environment_id}/dataset_items/{id}/\n\
  \  method: put\n  operationId: environments_dataset_items_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - dataset:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/environments/{environment_id}/dataset_items/{id}/\n  method: patch\n  operationId: environments_dataset_items_partial_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - dataset:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/environments/{environment_id}/dataset_items/{id}/\n  method: delete\n  operationId: environments_dataset_items_destroy\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    scope:\n    - dataset:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/environments/{environment_id}/datasets/\n  method: get\n  operationId: environments_datasets_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - dataset:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/environments/{environment_id}/datasets/\n  method: post\n  operationId: environments_datasets_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - dataset:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/environments/{environment_id}/datasets/{id}/\n\
  \  method: get\n  operationId: environments_datasets_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - dataset:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/environments/{environment_id}/datasets/{id}/\n  method: put\n  operationId: environments_datasets_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - dataset:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/environments/{environment_id}/datasets/{id}/\n\n# --- truncated at 32 KB (567 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/posthog/refs/heads/main/agentic-access/posthog-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/posthog/refs/heads/main/agentic-access/posthog-agentic-access.yml
summary_line: 1567 operations · 927 acting · 18 human-in-the-loop
tags:
- A/B Testing
- Analytics
- Feature Flags
- Open Source
- Product Analytics
- Session Recording
---
